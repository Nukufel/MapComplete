<script lang="ts">
  import TagRenderingConfig from "../../../Models/ThemeConfig/TagRenderingConfig"
  import { ImmutableStore, Store, UIEventSource } from "../../../Logic/UIEventSource"
  import type { Feature } from "geojson"
  import type { SpecialVisualizationState } from "../../SpecialVisualization"
  import TagRenderingAnswer from "./TagRenderingAnswer.svelte"
  import TagRenderingQuestion from "./TagRenderingQuestion.svelte"
  import { onDestroy } from "svelte"
  import Tr from "../../Base/Tr.svelte"
  import Translations from "../../i18n/Translations.js"
  import LayerConfig from "../../../Models/ThemeConfig/LayerConfig"
  import { Utils } from "../../../Utils"
  import { twMerge } from "tailwind-merge"
  import EditButton from "./EditButton.svelte"

  export let config: TagRenderingConfig
  export let tags: UIEventSource<Record<string, string>>
  export let selectedElement: Feature | undefined
  export let state: SpecialVisualizationState
  export let layer: LayerConfig = undefined

  export let editingEnabled: Store<boolean> | undefined = state?.featureSwitchUserbadge

  export let highlightedRendering: UIEventSource<string> = undefined
  export let clss = undefined
  /**
   * Indicates if this tagRendering currently shows the attribute or asks the question to _change_ the property
   */
  export let editMode = !config.IsKnown(tags.data)
  if (tags) {
    onDestroy(
      tags.addCallbackD((tags) => {
        editMode = !config.IsKnown(tags)
      })
    )
  }

  let htmlElem: HTMLDivElement
  $: {
    if (editMode && htmlElem !== undefined && config.IsKnown($tags)) {
      // EditMode switched to true yet the answer is already known, so the person wants to make a change
      // Make sure that the question is in the scrollview!

      // Some delay is applied to give Svelte the time to render the _question_
      window.setTimeout(() => {
        Utils.scrollIntoView(<any>htmlElem)
      }, 50)
    }
  }

  const _htmlElement = new UIEventSource<HTMLElement>(undefined)
  $: _htmlElement.setData(htmlElem)

  function setHighlighting() {
    if (highlightedRendering === undefined) {
      return
    }
    if (htmlElem === undefined) {
      return
    }
    const highlighted = highlightedRendering.data
    if (config.id === highlighted) {
      htmlElem.classList.add("focus")
      htmlElem.tabIndex = -1
      htmlElem.scrollIntoView({ behavior: "smooth" })
      Utils.focusOnFocusableChild(htmlElem)
    } else {
      htmlElem.classList.remove("focus")
    }
  }

  if (highlightedRendering) {
    onDestroy(highlightedRendering?.addCallbackAndRun(() => setHighlighting()))
    onDestroy(_htmlElement.addCallbackAndRun(() => setHighlighting()))
  }
  let answerId = "answer-" + Utils.randomString(5)
  let debug = state?.featureSwitches?.featureSwitchIsDebugging ?? new ImmutableStore(false)
</script>

<div bind:this={htmlElem} class={twMerge(clss, "tr-" + config.id)}>
  {#if $debug}
    <span class="subtle">
      {config.id}
    </span>
  {/if}
  {#if config.question}
    {#if editMode}
      <TagRenderingQuestion
        {config}
        {tags}
        {selectedElement}
        {state}
        {layer}
        on:saved={() => (editMode = false)}
        allowDeleteOfFreeform={true}
      >
        <button
          slot="cancel"
          class="secondary"
          on:click={() => {
            editMode = false
          }}
        >
          <Tr t={Translations.t.general.cancel} />
        </button>
      </TagRenderingQuestion>
    {:else}
      <div class="low-interaction flex items-center justify-between overflow-hidden rounded pl-2">
        <TagRenderingAnswer
          id={answerId}
          {config}
          {tags}
          {selectedElement}
          {state}
          {layer}
          extraClasses="my-2"
        />
        {#if !editingEnabled || $editingEnabled}
          <EditButton
            arialabel={config.editButtonAriaLabel}
            ariaLabelledBy={answerId}
            on:click={() => {
              editMode = true
            }}
          />
        {/if}
      </div>
    {/if}
  {:else}
    <TagRenderingAnswer {config} {tags} {selectedElement} {state} {layer} />
  {/if}
</div>
