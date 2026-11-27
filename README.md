# Azur Promilia English — v0.6.10

CPDD community English patcher for the **Japanese PC client**. Community testers have successfully applied English and launched the game. Corrections and coverage updates will continue as the game updates.

## Download

Download **[AzurPromiliaEnglish.exe](https://github.com/Lani27/azur-promilia-english-patch/releases/download/patcher-v0.6.10/AzurPromiliaEnglish.exe)** from the [v0.6.10 release](https://github.com/Lani27/azur-promilia-english-patch/releases/tag/patcher-v0.6.10).

1. Install any client/executable update through the official launcher, then close the game and official launcher. The patcher can download supported in-game content updates.
2. Open the patcher and select the folder containing `AzurPromiliaJP.exe`.
3. For English, select **Apply English**. For another language, choose **Settings → Game language → Français / Bahasa Indonesia / Español / Thai / Português (Brasil)**, wait for its download, then select **Apply translation**.
4. Accept any game download or repair prompt. The patcher restores recognized patches, verifies official downloads, then reapplies your language and mods. Select **Launch game**; it checks live game content again before starting, alongside translation/news and patcher updates. It uses the game's normal graphics mode.

**Corrupted files after a game update?** With v0.6.10, close the game and launcher, press **Apply English / Apply translation**, then accept **Repair and continue**. Keep the patcher's recovery files. If it specifically reports an interrupted patch transaction, use **Recover interrupted patch** first, then Apply again.

The published data contains **72,216 game/interface translation entries** and **23 news article bodies**. On verified game build **3273853**, **69,834 translations match** and **2,356 new or changed strings remain Japanese** until matching translations are published. This includes 109 existing messages in the separate update-screen language file; loading tooltips have been confirmed in English in-game. News list/header titles remain Japanese. Optional English graphics now cover **84 approved images**, including five achievement-book titles and 79 additional UI graphics. Five larger approved replacements and other unsupported Japanese image lettering remain unchanged. Changed or unknown source strings remain untouched until matching English is available. Not every scene or text layout has been tested.

## Game languages

Community translation contributors (Discord): **Indonesian (rukathebest)** and **French (tonax.)**.
Brazilian Portuguese contributor: **reinhardwq**.
Additional GitHub contributors: **French [pedrokarim](https://github.com/pedrokarim) and [TonySanchezD](https://github.com/TonySanchezD)**, **Spanish [KarloZ7715](https://github.com/KarloZ7715)** and **Thai [CXZP](https://github.com/CXZP)**.

English, Français, Bahasa Indonesia, Español, ไทย and Português (Brasil) use the same patcher. Thai requires **v0.6.6 or newer** for its included font support. Version 0.6.0 and newer download the selected community language from this repository; later translation revisions arrive through the normal update and pre-launch checks. No separate language-specific patcher or manual JSON installation is needed.

Community pack coverage against the published English catalog (72,216 entries):

| Language | Translated | English fallback |
| --- | ---: | ---: |
| Bahasa Indonesia | 71,925 | 291 |
| Français | 72,216 | 0 |
| Español | 71,925 | 291 |
| ไทย | 71,603 | 613 |
| Português (Brasil) | 71,445 | 771 |

Brazilian Portuguese adds 71,445 accepted translations from reinhardwq; 291 changed English references and 480 formatting conflicts are retained in its contributor review kit.

The latest French update completes 1,721 remaining targets and corrects 991 existing translations. Overlapping submissions in [#9](https://github.com/Lani27/azur-promilia-english-patch/issues/9) and [#11](https://github.com/Lani27/azur-promilia-english-patch/issues/11) were reviewed together; the validated #11 wording is used where they differ. Spanish has 291 lines awaiting review after English changes. The corrected Thai submission in [#8](https://github.com/Lani27/azur-promilia-english-patch/issues/8) adds 7,917 accepted entries; 613 still need formatting corrections, with the submitted wording retained for review. Missing or outdated community translations fall back to matching English. Changed Japanese source text stays Japanese until matching English is available; catalog coverage is not a guarantee of current-game coverage.

Thai includes glyph additions generated from **LINE Seed Sans TH**, under the [SIL Open Font License 1.1](FONT-LICENSES.md). They extend the gameplay and startup fallback atlases while preserving existing glyphs. Use v0.6.6 or newer to switch languages or restore after applying Thai. Installation, switching languages and restoration are verified on a temporary game copy; Thai combining marks, wrapping and translation quality still need in-game review. News stays English; English-specific graphics and layout overrides are excluded from community-language text.

Downloads verify size, SHA-256 and language identity. A previously verified compatible pack remains usable offline. Downloading never changes game files until **Apply translation** or an accepted pre-launch update. Select English and apply to switch back, or use **Restore Japanese** for exact originals.

**Import language pack** is available for local testing and pauses online updates for that language. **Use online language updates** resumes the hosted releases.

## Contribute translations

Download the **[translation kits and editable Japanese → English → target JSON files](CONTRIBUTING.md)** for a new language, Indonesian, French, Spanish, Thai or Brazilian Portuguese. **English is the maintained base**, updated by the maintainer; contributors translate or correct the target fields. Keep Japanese, English, context and entry IDs unchanged.

Send a completed or partial file as a ZIP through **[Translation submission on GitHub](https://github.com/Lani27/azur-promilia-english-patch/issues/new?template=translation.yml)**. Small corrections can be submitted directly in the form. Include your language and kit version so changes can be merged without overwriting other work. Submissions are reviewed before a patcher language update is published.

## Updates

English corrections, community translations, glossary changes, compatible new tables/IDs, supported interface locations, supported graphics and news articles can arrive as **data updates**, without downloading another executable. Each community language has independent releases. Updates are translated and prepared by maintainers; users apply them locally.

**New in v0.6.10:**

- Recovers updates installed while English was still applied. Restore and recovery skip retired paths, restore verified surviving patches and preserve newer game files.
- **Apply English** and **Launch game** check the live public JP content service. Approved content updates restore recognized patches, download verified official files, then reapply the selected language and mods.
- Detects damaged archives by checksum, including corruption with the correct file size. The repair prompt downloads clean copies directly from the official CDN; repeating a size-only launcher repair is unnecessary.
- Interrupted downloads retain verified files and resume on the next Apply or Launch. Debug reports identify pending stages and individual file/checksum problems.
- Download and repair prompts appear inside the patcher above other controls, with explicit continue/cancel buttons. They cannot be hidden behind the patcher window.
- Missing translations and new or changed Japanese strings remain untranslated until matching translations are available. Unsupported file formats still stop with an error.

Use **Check for updates → Update and restart**, then **Apply English / Apply translation**. You do not need to restore manually before a content update handled by the patcher. If the game already updated while patched, use Apply and accept the repair prompt. Client/executable updates still use the official launcher. This release contains recovery and update-handling fixes; translation coverage is unchanged.

Validation: 294 Rust tests and nine release checks passed, including prompt visibility and cancellation. Official-CDN repair of same-size corruption passed on a temporary copy; the rebuilt executable passed install/reapply/restore checks. The new automatic update-through-launch flow has not yet been tested in live gameplay.

**Also included from v0.6.8:**

- Fixes the missing-file error when reapplying translations after Restore Japanese and an official game update.
- Discovers the current archives without requiring retired files from a completed restore receipt. New, changed or missing translations keep the original Japanese text until exact source/context matches are available.
- Saves the updated Japanese originals for recovery. Temporary-copy apply, reapply and exact restoration passed; a local game launch in English was confirmed.

Use **Check for updates → Update and restart**, close the game and official launcher, then **Apply English / Apply translation**. This was a patcher compatibility update; no new translations were included.

**Also included from v0.6.7:**

- Interrupted-patch recovery accepts exact original game files already restored by the official launcher.
- Recovery logs and **Settings → Debug** identify the failing file, stage, expected/actual checksums and Windows error where available, without personal paths.
- Unrecognized files and recovery records are preserved; installation status is rechecked after recovery. The private recovery build resolved the reported issue on an affected user's PC.

Use **Check for updates → Update and restart**. If recovery is pending, close the game and official launcher, select **Recover interrupted patch**, then **Apply English / Apply translation**. Keep recovery files; share **Copy log** or **Settings → Debug** if it still fails. Current languages, camera data and mod selections are retained.

**Also included from v0.6.6:**

- Thai font support and a hosted Thai translation under **Settings → Game language → Thai**.
- Spanish is now hosted alongside French and Indonesian; French gains 1,104 interface translations.
- Refreshed contributor kits preserve pending translations and highlight formatting errors or changed English references. Submit fixes through the GitHub translation form.

Select **Check for updates → Update and restart**, then choose your language and **Apply translation**. Thai font support requires this executable update; later compatible Thai translation updates download normally.

**Changes since v0.6.3:**

- Fixed startup and data-folder errors caused by a lone `GameAssembly.dll` above AppData, such as in a drive root or user-profile folder. The DLL does not need to be removed.
- Actual game folders remain blocked as patcher data locations. The private fix was confirmed working on an affected user's PC.

On v0.6.3, select **Check for updates → Update and restart**. If the error prevents startup, close the old patcher and open the current download above. This storage fix does not require reapplying translations; language packs, news, graphics and mods are unchanged.

**Changes since v0.6.2:**

- **Update and restart** downloads, verifies and replaces the patcher, then reopens it. Users on v0.6.2 or older download the current executable manually once; subsequent executable updates can use this button. Settings, recovery data and mods stay in place.
- **Apply** automatically refreshes missing or damaged translation data once before changing game files. Failed recovery reports a specific, sanitized data error.
- Missing patcher data folders are recreated automatically. **Change folder** and **Use default location** also work when the previous folder or drive is gone. Deleted recovery backups cannot be recreated.
- Recognized leftover CPDD full-text/UID helpers can be backed up and recreated after confirmation, without the old game folder or receipt. Unknown or official hotfix packages remain protected. Other game copies sharing the helper cache may need their patch reapplied.
- **291 reviewed dialogue corrections** preserve separate text variants, fixing repeated/merged dialogue in affected entries. Future scans check the same separators.
- **Français** is available under **Settings → Game language**. Missing or outdated French entries use current English.

For the v0.6.3 dialogue corrections, close the game and launcher, then select **Apply English** or **Apply translation**. These corrections also arrive as compatible data updates for v0.6.2. Existing mods, graphics and news are preserved. The corrected dialogue scene still needs in-game visual confirmation.

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

Download the current patcher and apply the selected language to use these features. If full-text support is skipped, follow the reported recovery steps and apply again. Compatible future translation, news, layout and graphic changes remain data updates. English translation and news counts are unchanged from v0.5.9.

Automated checks cover archive readback, temporary-copy install/reapply, independent mod removal, byte-exact restoration and missing/modified camera scenarios. The new HUD UID option still needs an in-game check across scene changes; not every long title is guaranteed to fit every resolution.

Before launch, **Update and launch** applies changed translation data or refreshes news data. A newer executable offers **Update and restart**; a required compatibility/fix release blocks launch until updated. Saved translation data may be used after a failed translation check, but **Launch game** requires a successful live game-content check. Apply can use verified local content when the game service is unreachable and no game download is pending, with an explicit notice.

New binary formats or unsupported decoder changes may require another executable. Data packages cannot install executable code. Each translation must match the current Japanese source and context; old English is never selected by ID alone. News bodies are checked against fresh official article content before use.

**Restore Japanese** remains available for returning to native files. If an official update or repair already ran while patched, use **Apply English / Apply translation** and accept any repair prompt. **Recover interrupted patch** handles interrupted patch transactions while preserving recovery records.

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

This repository contains player instructions, contribution instructions, the translation submission form, the update channel, the community-language index and the font license. Player releases contain the executable, checksums, English/mapping/news data and prepared community-language packs. Separate contributor releases contain editable Japanese/English/target JSON files, review reports and instructions. No complete game archives, maintainer source, API tools, credentials or translation memory are published. Original game files and recovery records stay on each user's computer.

Downloads use this repository's HTTPS channel and release assets with SHA-256 and size verification. The channel is not separately signed; the publishing GitHub account is the update trust boundary. Version 0.6.10 also checks the live public JP game-content service without an account login. Official manifest MD5 and archive size/CRC checks must pass before downloaded content is activated.
