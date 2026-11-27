# Azur Promilia English — v0.6.3

CPDD community English patcher for the **Japanese PC client**. Community testers have successfully applied English and launched the game. This is a pre-release build; corrections and coverage updates will continue as the game updates.

## Download

Download **[AzurPromiliaEnglish.exe](https://github.com/Lani27/azur-promilia-english-patch/releases/download/patcher-v0.6.3/AzurPromiliaEnglish.exe)** from the [v0.6.3 release](https://github.com/Lani27/azur-promilia-english-patch/releases/tag/patcher-v0.6.3).

1. Finish updates through the official launcher, including any download on the game's first screen. Close the game and official launcher.
2. Open the patcher and select the folder containing `AzurPromiliaJP.exe`.
3. For English, select **Apply English**. For French or Indonesian, choose **Settings → Game language → Français / Bahasa Indonesia**, wait for its download, then select **Apply translation**.
4. Select **Launch game**. The patcher checks for updates first and prompts when newer translation/news data or a patcher release is available. It uses the game's normal graphics mode.

The current data contains **72,216 matching game/interface translation entries** and **23 news article bodies**. This includes 109 existing messages in the separate update-screen language file; loading tooltips have been confirmed in English in-game. News list/header titles remain Japanese. Optional English graphics now cover **84 approved images**, including five achievement-book titles and 79 additional UI graphics. Five larger approved replacements and other unsupported Japanese image lettering remain unchanged. Changed or unknown source strings remain untouched until matching English is available. Not every scene or text layout has been tested.

## Game languages

English, Français and Bahasa Indonesia use the same patcher. Version 0.6.0 and newer download the selected community language from this repository; later translation revisions arrive through the normal update and pre-launch checks. No separate language-specific patcher or manual JSON installation is needed.

The current French pack supplies **69,682 entries**. With the v0.6.3 English corrections, **69,391 match and 2,825 use English fallback**, including 291 entries whose English references changed. The Indonesian pack supplies **72,216 validated entries**; the 334 previously rejected entries have been corrected. Changed Japanese text or English references fall back to current English until the community translation is updated. News stays English; English-specific graphics and layout overrides are excluded from community-language text. Translation quality, fonts and layout still need in-game review.

Downloads verify size, SHA-256 and language identity. A previously verified compatible pack remains usable offline. Downloading never changes game files until **Apply translation** or an accepted pre-launch update. Select English and apply to switch back, or use **Restore Japanese** for exact originals.

**Import language pack** is available for local testing and pauses online updates for that language. **Use online language updates** resumes the hosted releases.

## Updates

English corrections, community translations, glossary changes, compatible new tables/IDs, supported interface locations, supported graphics and news articles can arrive as **data updates**, without downloading another executable. Each community language has independent releases. Updates are translated and prepared by maintainers; users apply them locally.

**Changes since v0.6.2:**

- **Update and restart** downloads, verifies and replaces the patcher, then reopens it. Install v0.6.3 manually once; subsequent executable updates can use this button. Settings, recovery data and mods stay in place.
- **Apply** automatically refreshes missing or damaged translation data once before changing game files. Failed recovery reports a specific, sanitized data error.
- Missing patcher data folders are recreated automatically. **Change folder** and **Use default location** also work when the previous folder or drive is gone. Deleted recovery backups cannot be recreated.
- Recognized leftover CPDD full-text/UID helpers can be backed up and recreated after confirmation, without the old game folder or receipt. Unknown or official hotfix packages remain protected. Other game copies sharing the helper cache may need their patch reapplied.
- **291 reviewed dialogue corrections** preserve separate text variants, fixing repeated/merged dialogue in affected entries. Future scans check the same separators.
- **Français** is available under **Settings → Game language**. Missing or outdated French entries use current English.

Download v0.6.3, close the game and launcher, then select **Apply English** or **Apply translation**. The dialogue corrections also arrive as compatible data updates for v0.6.2. Existing mods, graphics and news are preserved. The corrected dialogue scene still needs in-game visual confirmation.

**Changes since v0.6.0:**

- 79 additional approved English graphics in **English Graphic Replacement**, for 84 total.
- A new **Hide HUD UID** method that keeps ping and signal bars visible. Applying English repairs the old method even when the option is now off, then retains the selected state.
- Better fitting gacha, gift and mission/dialogue-button text, with layout corrections across 26 interface assets.
- Clearer instructions for missing or empty resources: finish the remaining downloads using the **wrench-and-hammer icon on the title screen**, then close the game and launcher before applying again.

Select **Apply English** to update an existing installation. Enabled English graphics update automatically; otherwise, use **Mods → English Graphic Replacement → Install**. The v0.6.2 artwork support required an executable update once; later compatible artwork updates can be delivered as data.

**Changes since v0.5.3:** 3,551 corrected English entries, reviewed terminology and ruby annotations, layout corrections across 22 interface assets, six additional news bodies and five optional achievement-book title graphics. Layout changes cover comparison/recommendation buttons, Kibo labels and values, role badges, Journey tasks, event rewards and observation banners.

**Changes since v0.5.9:**

- Settings to change the patcher's data location, including downloads, recovery files and logs.
- Full dialogue choices, interaction names and HUD quest titles on the supported game build, removing their fixed-length truncation.
- Independent Disable Radial Blur and Disable Shared Camera Shake mods, grouped with the existing Motion Blur control.
- Camera-fade coverage extended to both photo-mode cameras and distance-based fading/hiding.
- Stronger source validation and independent restoration for mod assets.

**Changes since v0.5.12:**

- A large highlighted notice explains how to finish missing title-screen downloads, with a **Check game again** button.
- Missing or unverified optional camera content no longer blocks an otherwise valid English installation. The patcher explains when full dialogue/interaction/quest text could not be enabled. Required translation files and recovery conflicts still receive strict checks.
- Camera errors include the failing stage, asset identifier, expected/observed checksums and safe game-relative locations in the shared log.
- Recognizes the reviewed external **AzurPromiliaJP-NoCameraFade Direct 1.0.0** modification and explains how to restore it with the original tool. External files and backups are not removed automatically.
- Reviewed camera compatibility rules can arrive through data updates when the existing engine supports them.
- New optional **Hide HUD UID** mod, off by default, with independent Install/Uninstall controls.

Download v0.6.3 and apply the selected language to use the current patcher. If full-text support is skipped, follow the reported recovery steps and apply again. Compatible future translation, news, layout and graphic changes remain data updates. English translation and news counts are unchanged from v0.5.9.

Automated checks cover archive readback, temporary-copy install/reapply, independent mod removal, byte-exact restoration and missing/modified camera scenarios. The new HUD UID option still needs an in-game check across scene changes; not every long title is guaranteed to fit every resolution.

Before launch, **Update and launch** applies changed game data or refreshes news data. A newer executable offers **Update and restart**; a required compatibility/fix release blocks launch until updated. If the online check cannot finish, the patcher asks before using verified saved data.

New binary formats or unsupported decoder changes may require another executable. Data packages cannot install executable code. Each translation must match the current Japanese source and context; old English is never selected by ID alone. News bodies are checked against fresh official article content before use.

Before official launcher updates or repairs, use **Restore Japanese**, finish the game update, then apply English again. **Recover interrupted patch** handles interrupted operations while preserving recovery records.

## Mods

Open the **Mods** tab and use each feature's **Install** or **Uninstall** button. Mods can be used before or after applying English and start off by default.

The **motion-sickness mods** group contains three independent options:

- **Disable Motion Blur:** disables the shared camera-motion-blur volume; separate combat blur can remain.
- **Disable Radial Blur:** disables radial and scan blur in the supported effect/story volumes; separate or runtime-controlled blur may remain.
- **Disable Shared Camera Shake:** disables the shared shake profile; other camera-shake effects may remain.

The other mods remain separate:

- **English Graphic Replacement:** 84 English UI graphics, including the five achievement-book titles. Uninstall restores the original graphics.
- **Disable TAA:** changes the last-used anti-aliasing profile, leaving DLSS/FSR/XeSS and FPS settings alone.
- **Async shaders (DX11):** experimental; uninstall if graphical errors appear.
- **No zoomed-in character fade:** disables angle and distance fading/hiding in overworld and photo cameras. Special runtime-controlled fades may remain.
- **Hide HUD UID:** hides the HUD identifier through opacity while preserving ping and signal bars. Apply English also repairs the previous method, including when the option is now off. This does not cover identifiers separately stamped into exported photos.

Mod actions update only affected files, preserving English and other mods. **Remove all mods / Restore defaults** removes optional mods and graphics while keeping English text. **Restore Japanese** also restores owned mod files and saved anti-aliasing values. Close the game and official launcher before installing or uninstalling mods.

## Data location

Use **Settings → Change folder** to move the patcher's downloads, recovery files, preferences and logs to a dedicated folder on another local drive. **Use default location** moves them back. The default location is unchanged, and this setting does not move the game installation.

## Help

If an error occurs, use **Copy log** or **Open log** and send the sanitized patcher log through **[Get help on Discord](https://discord.gg/yyds)**. Errors include a specific next step. Share the patcher's log, rather than the game's account or launcher logs.

The patcher verifies the Japanese client's identity before checking compatibility. Automatic discovery uses local fixed drives and skips network paths and junctions. The Rust interface sleeps between events, uses VSync and caps redraws at 30 FPS.

## Distribution

This repository contains only this README, the update channel and the community-language index. Releases contain the executable, checksums, English/mapping/news data and prepared community-language packs, never complete game archives or maintainer source, API tools, credentials or translation memory. Original game files and recovery records stay on each user's computer.

Downloads use this repository's HTTPS channel and release assets with SHA-256 and size verification. The channel is not separately signed; the publishing GitHub account is the update trust boundary. Game-content checks compare installed manifests with the published verified build and do not claim live authenticated server freshness.
