<script lang="ts">
  /**
   * Shows an 'upload'-button which will start the upload for this feature
   */

  import type { SpecialVisualizationState } from "../SpecialVisualization"
  import { ImmutableStore, UIEventSource } from "../../Logic/UIEventSource"
  import type { OsmTags } from "../../Models/OsmFeature"
  import LoginToggle from "../Base/LoginToggle.svelte"
  import Translations from "../i18n/Translations"
  import Tr from "../Base/Tr.svelte"
  import UploadingImageCounter from "./UploadingImageCounter.svelte"
  import FileSelector from "../Base/FileSelector.svelte"
  import LoginButton from "../Base/LoginButton.svelte"
  import { Translation } from "../i18n/Translation"
  import Camera from "@babeard/svelte-heroicons/solid/Camera"

  export let state: SpecialVisualizationState

  export let tags: UIEventSource<OsmTags>
  export let targetKey: string = undefined
  /**
   * Image to show in the button
   * NOT the image to upload!
   */
  export let image: string = undefined
  if (image === "") {
    image = undefined
  }
  export let labelText: string = undefined
  const t = Translations.t.image

  let licenseStore = state?.userRelatedState?.imageLicense ?? new ImmutableStore("CC0")

  let errors = new UIEventSource<Translation[]>([])

  function handleFiles(files: FileList) {
    const errs = []
    for (let i = 0; i < files.length; i++) {
      const file = files.item(i)
      console.log("Got file", file.name)
      try {
        const canBeUploaded = state?.imageUploadManager?.canBeUploaded(file)
        if (canBeUploaded !== true) {
          errs.push(canBeUploaded.error)
          continue
        }
        state?.imageUploadManager.uploadImageAndApply(file, tags, targetKey)
      } catch (e) {
        alert(e)
      }
    }
    errors.setData(errs)
  }
</script>

<LoginToggle {state}>
  <LoginButton clss="small w-full" osmConnection={state.osmConnection} slot="not-logged-in">
    <Tr t={Translations.t.image.pleaseLogin} />
  </LoginButton>
  <div class="my-4 flex flex-col">
    <UploadingImageCounter {state} {tags} />
    {#each $errors as error}
      <Tr t={error} cls="alert" />
    {/each}
    <FileSelector
      accept="image/*"
      cls="button border-2 text-2xl"
      multiple={true}
      on:submit={(e) => handleFiles(e.detail)}
    >
      <div class="flex items-center">
        {#if image !== undefined}
          <img src={image} aria-hidden="true" />
        {:else}
          <Camera class="h-12 w-12 p-1" aria-hidden="true" />
        {/if}
        {#if labelText}
          {labelText}
        {:else}
          <Tr t={t.addPicture} />
        {/if}
      </div>
    </FileSelector>
    <div class="text-sm">
      <button
        class="as-link"
        style="margin: 0; padding: 0"
        on:click={() => {
          state.guistate.openUsersettings("picture-license")
        }}
      >
        <Tr t={t.currentLicense.Subs({ license: $licenseStore })} />
      </button>
      <br />
      <Tr cls="subtle italic" t={t.respectPrivacy} />
    </div>
  </div>
</LoginToggle>
