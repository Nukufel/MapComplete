<script lang="ts">
  import { OsmConnectionFeatureSwitches } from "../Logic/State/FeatureSwitchState"
  import { OsmConnection } from "../Logic/Osm/OsmConnection"
  import { QueryParameters } from "../Logic/Web/QueryParameters"
  import UserRelatedState from "../Logic/State/UserRelatedState"
  import LanguagePicker from "./InputElement/LanguagePicker.svelte"
  import Translations from "./i18n/Translations"
  import Logo from "../assets/svg/Logo.svelte"
  import Tr from "./Base/Tr.svelte"
  import MoreScreen from "./BigComponents/MoreScreen"
  import LoginToggle from "./Base/LoginToggle.svelte"
  import Pencil from "../assets/svg/Pencil.svelte"
  import Constants from "../Models/Constants"
  import { Store, UIEventSource } from "../Logic/UIEventSource"
  import { placeholder } from "../Utils/placeholder"
  import { SearchIcon } from "@rgossiaux/svelte-heroicons/solid"
  import ThemesList from "./BigComponents/ThemesList.svelte"
  import { LayoutInformation } from "../Models/ThemeConfig/LayoutConfig"
  import * as themeOverview from "../assets/generated/theme_overview.json"
  import UnofficialThemeList from "./BigComponents/UnofficialThemeList.svelte"
  import Eye from "../assets/svg/Eye.svelte"
  import LoginButton from "./Base/LoginButton.svelte"
  import ChevronDoubleRight from "@babeard/svelte-heroicons/mini/ChevronDoubleRight"
  import Mastodon from "../assets/svg/Mastodon.svelte"
  import Liberapay from "../assets/svg/Liberapay.svelte"
  import Bug from "../assets/svg/Bug.svelte"
  import Github from "../assets/svg/Github.svelte"
  import { Utils } from "../Utils"
  import { ArrowTrendingUp } from "@babeard/svelte-heroicons/solid/ArrowTrendingUp"

  const featureSwitches = new OsmConnectionFeatureSwitches()
  const osmConnection = new OsmConnection({
    fakeUser: featureSwitches.featureSwitchFakeUser.data,
    oauth_token: QueryParameters.GetQueryParameter(
      "oauth_token",
      undefined,
      "Used to complete the login"
    ),
  })
  const state = new UserRelatedState(osmConnection)
  const t = Translations.t.index
  const tr = Translations.t.general.morescreen

  let userLanguages = osmConnection.userDetails.map((ud) => ud.languages)
  let themeSearchText: UIEventSource<string | undefined> = new UIEventSource<string>(undefined)

  document.addEventListener("keydown", function (event) {
    if (event.ctrlKey && event.code === "KeyF") {
      document.getElementById("theme-search")?.focus()
      event.preventDefault()
    }
  })

  let visitedHiddenThemes: Store<LayoutInformation[]>
  const hiddenThemes: LayoutInformation[] =
    (themeOverview["default"] ?? themeOverview)?.filter((layout) => layout.hideFromOverview) ?? []
  {
    const prefix = "mapcomplete-hidden-theme-"
    const userPreferences = state.osmConnection.preferencesHandler.preferences
    visitedHiddenThemes = userPreferences.map((preferences) => {
      const knownIds = new Set<string>(
        Object.keys(preferences)
          .filter((key) => key.startsWith(prefix))
          .map((key) => key.substring(prefix.length, key.length - "-enabled".length))
      )
      return hiddenThemes.filter(
        (theme) =>
          knownIds.has(theme.id) ||
          state.osmConnection.userDetails.data.name === "Pieter Vander Vennet"
      )
    })
  }
</script>

<main>
  <div class="m-4 flex flex-col">
    <LanguagePicker
      clss="self-end max-w-full"
      assignTo={state.language}
      availableLanguages={t.title.SupportedLanguages()}
      preferredLanguages={userLanguages}
    />

    <div class="mt-4 flex">
      <div class="m-3 flex-none">
        <Logo alt="MapComplete Logo" class="h-12 w-12 sm:h-24 sm:w-24" />
      </div>

      <div class="link-underline flex flex-col">
        <h1 class="m-0 font-extrabold tracking-tight md:text-6xl">
          <Tr t={t.title} />
        </h1>
        <Tr
          cls="mr-4 text-base font-semibold sm:text-lg md:mt-5 md:text-xl lg:mx-0"
          t={Translations.t.index.intro}
        />
        <a href="#about">
          <Tr t={Translations.t.index.learnMore} />
          <ChevronDoubleRight class="inline h-4 w-4" />
        </a>
      </div>
    </div>

    <form
      class="flex justify-center"
      on:submit|preventDefault={(_) => MoreScreen.applySearch(themeSearchText.data)}
    >
      <label
        class="neutral-label my-2 flex w-full items-center rounded-full border-2 border-black sm:w-1/2"
      >
        <SearchIcon aria-hidden="true" class="h-8 w-8" />
        <input
          autofocus
          bind:value={$themeSearchText}
          class="mr-4 w-full outline-none"
          id="theme-search"
          type="search"
          use:placeholder={tr.searchForATheme}
        />
      </label>
    </form>

    <ThemesList search={themeSearchText} {state} themes={MoreScreen.officialThemes} />

    <LoginToggle {state}>
      <ThemesList
        hideThemes={false}
        isCustom={false}
        search={themeSearchText}
        {state}
        themes={$visitedHiddenThemes}
      >
        <svelte:fragment slot="title">
          <h3>
            <Tr t={tr.previouslyHiddenTitle} />
          </h3>
          <p>
            <Tr
              t={tr.hiddenExplanation.Subs({
                hidden_discovered: $visitedHiddenThemes.length.toString(),
                total_hidden: hiddenThemes.length.toString(),
              })}
            />
          </p>
        </svelte:fragment>
      </ThemesList>

      <UnofficialThemeList search={themeSearchText} {state} />
    </LoginToggle>

    <a
      class="button flex"
      href={window.location.protocol + "//" + window.location.host + "/studio.html"}
    >
      <Pencil class="mr-2 h-6 w-6" />
      <Tr t={Translations.t.general.morescreen.createYourOwnTheme} />
    </a>

    <h3 id="about">
      <Tr t={Translations.t.index.about} />
    </h3>
    <Tr cls="link-underline" t={Translations.t.general.aboutMapComplete.intro} />

    <span class="link-underline flex flex-col gap-y-1">
      <a class="flex" href="https://github.com/pietervdvn/MapComplete/" target="_blank">
        <Github class="mr-2 h-6 w-6" />
        <Tr t={Translations.t.general.attribution.gotoSourceCode} />
      </a>
      <a class="flex" href="https://github.com/pietervdvn/MapComplete/issues" target="_blank">
        <Bug class="mr-2 h-6 w-6" />
        <Tr t={Translations.t.general.attribution.openIssueTracker} />
      </a>

      <a class="flex" href={Utils.OsmChaLinkFor(7)} target="_blank">
        <ArrowTrendingUp class="mr-2 h-6 w-6" />
        <Tr t={Translations.t.general.attribution.openOsmchaLastWeek} />
      </a>

      <a class="flex" href="https://en.osm.town/@MapComplete" target="_blank">
        <Mastodon class="mr-2 h-6 w-6" />
        <Tr t={Translations.t.general.attribution.followOnMastodon} />
      </a>

      <a class="flex" href="https://liberapay.com/pietervdvn/" target="_blank">
        <Liberapay class="mr-2 h-6 w-6" />
        <Tr t={Translations.t.general.attribution.donate} />
      </a>

      <a
        class="flex"
        href={window.location.protocol + "//" + window.location.host + "/privacy.html"}
      >
        <Eye class="mr-2 h-6 w-6" />
        <Tr t={Translations.t.privacy.title} />
      </a>
    </span>

    <Tr t={tr.streetcomplete} />

    <div class="subtle mb-16 self-end">
      v{Constants.vNumber}
    </div>
  </div>
</main>
