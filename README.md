# Azur Promilia English — v0.6.13

CPDD community English patcher for the **Japanese PC client**. Community testers have successfully applied English and launched the game. Corrections and coverage updates will continue as the game updates.

## Download

Download **[AzurPromiliaEnglish.exe](https://github.com/Lani27/azur-promilia-english-patch/releases/download/patcher-v0.6.13/AzurPromiliaEnglish.exe)** from the [v0.6.13 release](https://github.com/Lani27/azur-promilia-english-patch/releases/tag/patcher-v0.6.13).

1. Install any client/executable update through the official launcher, then close the game and official launcher. The patcher can download supported in-game content updates.
2. Open the patcher and select the folder containing `AzurPromiliaJP.exe`.
3. For English, select **Apply English**. For another language, choose **Settings → Game language → Français / Bahasa Indonesia / Español / Português (Brasil)**, wait for its download, then select **Apply translation**.
4. Apply automatically handles supported content downloads and repairs, restores recognized patches, then reapplies your language and mods. Select **Launch game**; it checks live game content again before starting and prompts if a content update is needed, alongside translation/news and patcher updates. It uses the game's normal graphics mode.

**Broken installation after an update or repair?** Update to v0.6.13, close the game and official launcher, then press **Apply English / Apply translation**. The patcher automatically repairs supported missing or damaged files, rebuilds verified Japanese backups when available and resumes recognized interrupted patches before continuing. Keep the patcher's recovery files; do not delete AppData. If something cannot be repaired safely, the patcher explains the problem and next step.

The [published English data](https://github.com/Lani27/azur-promilia-english-patch/releases/tag/data-content-3273853-spacing-artwork-20261128) contains **72,190 supported game/interface translations** and **25 news article bodies**. It retains the previously reviewed **234 new and 2,122 changed strings** for game content **3273853**, adds spacing corrections in **388 entries**, and includes **89 approved English graphics** with the five previously excluded larger replacements. All 72,190 supported strings validate and match the verified source, with zero missing translations in that set. This data requires **patcher 0.6.13 or newer** for the additional graphics and downloads separately from the executable. News is unchanged in this release; loading tooltips have been confirmed in English in-game, while news list/header titles remain Japanese. Unsupported image lettering and new or changed source strings remain untranslated until matching English is available. Not every scene or text layout has been tested.

## Game languages

Indonesian contributor: **rukathebest (Discord)**.
French contributors: **tonax. (Discord) / [TonySanchezD](https://github.com/TonySanchezD) (GitHub)** and **[pedrokarim](https://github.com/pedrokarim) (GitHub)**.
Brazilian Portuguese contributor: **reinhardwq**.
Spanish contributor: **[KarloZ7715](https://github.com/KarloZ7715) (GitHub)**.

English, Français, Bahasa Indonesia, Español and Português (Brasil) use the same patcher. Version 0.6.0 and newer download the selected community language from this repository; later translation revisions arrive through the normal update and pre-launch checks. No separate language-specific patcher or manual JSON installation is needed.

Community pack coverage against the **content-3273853-20261128** English catalog (72,190 entries):

| Language | Translated | English fallback |
| --- | ---: | ---: |
| Bahasa Indonesia | 69,512 | 2,678 |
| Français | 72,190 | 0 |
| Español | 72,190 | 0 |
| Português (Brasil) | 70,013 | 2,177 |

The table above counts exact matches against the named `content-3273853-20261128` baseline. The contributor kits still use that 72,190-entry English base and have not been regenerated for this spacing update. Community entries with changed references use matching English until each language is updated.

The latest Brazilian Portuguese update from reinhardwq adds 941 translated entries and corrects 6,829 existing targets. Formatting was corrected in 442 entries; 2,177 entries without supplied translations continue to use English.

French [#13](https://github.com/Lani27/azur-promilia-english-patch/issues/13) completes 2,388 pending entries. Spanish [#15](https://github.com/Lani27/azur-promilia-english-patch/issues/15) completes 2,678 pending entries and corrects 55 existing targets. Both now cover all 72,190 entries in the current kit. These Windows updates require patcher **v0.6.11 or newer**. Missing or outdated community translations fall back to matching English. Changed Japanese source text stays Japanese until matching English is available; catalog coverage is not a guarantee of current-game coverage.

The same French, Spanish and Brazilian Portuguese submissions are available as [Android data updates](https://github.com/Lani27/azur-promilia-english-patch/releases/tag/android-data-3273851-20261128.2). Use Android patcher **0.4.1 or newer**, select the language and tap **Apply**. Android coverage depends on exact matches with its own game resources.

**Thai translation withdrawn:** The Thai packs, contributor files and update-channel entry have been removed following the redistribution report and submitter's acknowledgement in [issue #8](https://github.com/Lani27/azur-promilia-english-patch/issues/8#issuecomment-7229327535). Older patcher builds may still list Thai or retain previously downloaded copies. If Thai is installed, select English or another supported language and apply, or use **Restore Japanese**.

News stays English; English-specific graphics and layout overrides are excluded from community-language text.

Downloads verify size, SHA-256 and language identity. A previously verified compatible pack remains usable offline. Downloading never changes game files until **Apply translation** or an accepted pre-launch update. Select English and apply to switch back, or use **Restore Japanese** for exact originals.

**Import language pack** is available for local testing and pauses online updates for that language. **Use online language updates** resumes the hosted releases.

## Contribute translations

Download the **[translation kits and editable Japanese → English → target JSON files](CONTRIBUTING.md)** for a new language, Indonesian, French, Spanish or Brazilian Portuguese. **English is the maintained base**, updated by the maintainer; contributors translate or correct the target fields. Keep Japanese, English, context and entry IDs unchanged.

The refreshed **[72,190-entry contributor kits](https://github.com/Lani27/azur-promilia-english-patch/releases/tag/translator-files-20261128.7)** use the published `content-3273853-20261128` English base. Existing translations carry over where references match. Every language ZIP includes `REVIEW.html` and `review.json`, highlighting new or changed entries and preserving previous wording for review.

Send a completed or partial file as a ZIP through **[Translation submission on GitHub](https://github.com/Lani27/azur-promilia-english-patch/issues/new?template=translation.yml)**. Small corrections can be submitted directly in the form. Include your language and kit version so changes can be merged without overwriting other work. Submissions are reviewed before a patcher language update is published.

## Updates

English corrections, community translations, glossary changes, compatible new tables/IDs, supported interface locations, supported graphics and news articles can arrive as **data updates**, without downloading another executable. Each community language has independent releases. Updates are translated and prepared by maintainers; users apply them locally.

**New in v0.6.13:**

- **Faster content updates:** compares official release manifests so unchanged archives need presence/size checks instead of a complete reread. This also covers fresh installations that still need their first in-game update. Changed archives, recorded patch files and invalidated saved checks still receive checksum verification.
- **No second full scan after an update:** verified downloads continue directly to applying English. Later Apply and Launch checks skip the full scan while content versions and recorded sources remain unchanged. Genuine repair, unfinished downloads or unavailable update history can still require broader verification.
- **Resumable checks and a quieter journal:** saves verified checks during scanning and on cancellation; progress counters update in place without filling the journal every second.
- **Five more English graphics:** all 89 approved images are supported, including the larger replacements previously excluded. Native image dimensions and approved artwork are preserved. Enable **English Graphic Replacement** in Mods; existing selections update when you apply English. Use **Launch game** in the patcher to preserve the selected language and mods.
- **English spacing fixes:** corrects missing spaces around glossary names and unusual apostrophe spacing in 388 entries, while preserving lore-link identifiers and formatting. Future English exports apply the same checks.

Update the patcher, close the game and official launcher, then select **Apply English / Apply translation**. The English catalog, graphics and news remain a separate data download; no translation catalog is bundled in the EXE. Community packs and contributor kits retain their stated releases.

Validation: 340 Rust tests and 74 Python tests passed; 41 opt-in Rust tests and two Python tests were skipped by those suites. Separate checks verified the exact executable, offline data upgrade, and temporary-copy installation, reapplication, mod toggles and byte-exact Japanese restoration for all 72,190 strings and 89 graphics. No live game or cache files were changed. In-game rendering of these changes has not yet been visually checked.

**Included from v0.6.12:**

Broken installation? Update the patcher, close the game and official launcher, then press **Apply English** (or **Apply translation** for your selected language). Supported repairs now run automatically and continue into patching. Keep your patcher recovery files; there is no need to delete AppData.

- **Automatic repair and recovery:** downloads checksum-verified official files for missing or damaged archives, including same-size corruption. Restores verified surviving patches after game updates and resumes recognized interrupted patches.
- **Japanese backup recovery:** rebuilds missing or damaged backups from verified local originals or the official CDN when the saved original is available. Restore Japanese and Recover use this recovery too.
- **Faster checks:** complete, up-to-date fresh installations and unchanged installations skip unnecessary full archive scans. Required repeat scans reuse verified unchanged files; changed files still receive checksum checks.
- **More efficient patch and mod archives:** preserves native archive blocks where possible and reuses unchanged compressed data. This reduces rebuilding and decompression work; gameplay FPS has not been measured.
- **Clearer operation feedback:** automatic download retries, specific file/permission/disk-space errors and a **Cancel operation** button. Optional news-cache failures no longer block game-file recovery.

**Launch game** still checks for content updates before starting and asks before downloading a new update. Client/executable updates use the official launcher. New or changed Japanese text stays untranslated until a matching translation is available.

Translation data remains a separate download. This patcher release does not replace the current English data, community language packs or translation kits.

Validation: 329 Rust tests and 39 publication/update Python tests passed. The exact 0.6.12 executable passed its read-only audit, temporary-copy installation/reapplication/exact restoration of 72,190 translations, and the 0.6.11 → 0.6.12 self-update restart check. Forty optional Rust tests were skipped in this release run; separate official-CDN recovery and process-guard checks passed during development. No live game files were changed by verification.

**Also included from v0.6.11:**

- Faster full archive verification with up to four readers, with progress showing bytes checked and scan speed. Checksum checks still catch same-size corruption.
- Mod checkboxes with **Install selected / Uninstall selected** buttons. Selected changes run together, preserving translated text and unselected mods.
- A fix for validating equivalent compound numeric quantities in translations.
- A separate English data update: **234 new and 2,122 changed translations**, all **72,190 supported strings** validated, and refreshed news. The executable contains no bundled translation catalog.

Use **Check for updates → Update and restart**, then **Apply English / Apply translation**. Version 0.6.12 handles supported repairs automatically.

Validation: 299 Rust tests and 69 Python tests passed; 36 optional Rust tests were skipped. The packaged executable passed its read-only audit and temporary-copy installation, batch mod changes, reapplication and exact restoration. These checks did not modify the live game.

**Also included from v0.6.10:**

- Recovers updates installed while English was still applied. Restore and recovery skip retired paths, restore verified surviving patches and preserve newer game files.
- **Apply English** and **Launch game** check the live public JP content service. Approved content updates restore recognized patches, download verified official files, then reapply the selected language and mods.
- Detects damaged archives by checksum, including corruption with the correct file size. The repair prompt downloads clean copies directly from the official CDN; repeating a size-only launcher repair is unnecessary.
- Interrupted downloads retain verified files and resume on the next Apply or Launch. Debug reports identify pending stages and individual file/checksum problems.
- Download and repair prompts appear inside the patcher above other controls, with explicit continue/cancel buttons. They cannot be hidden behind the patcher window.
- Missing translations and new or changed Japanese strings remain untranslated until matching translations are available. Unsupported file formats still stop with an error.

Use **Check for updates → Update and restart**, then **Apply English / Apply translation**. You do not need to restore manually before a content update handled by the patcher. If the game already updated while patched, use Apply; v0.6.12 handles supported repairs automatically. Client/executable updates still use the official launcher. This release contains recovery and update-handling fixes; translation coverage is unchanged.

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

Use **Check for updates → Update and restart**. If recovery is pending, close the game and official launcher and select **Apply English / Apply translation**. Version 0.6.12 resumes recognized interrupted patches automatically; **Recover interrupted patch** remains available separately. Keep recovery files; share **Copy log** or **Settings → Debug** if it still fails. Current languages, camera data and mod selections are retained.

**Also included from v0.6.6:**

- Thai font support was added in this version; the hosted Thai translation has since been withdrawn.
- Spanish is now hosted alongside French and Indonesian; French gains 1,104 interface translations.
- Refreshed contributor kits preserve pending translations and highlight formatting errors or changed English references. Submit fixes through the GitHub translation form.

Select **Check for updates → Update and restart**, then choose a supported language and **Apply translation**.

**Changes since v0.6.3:**

- Fixed startup and data-folder errors caused by a lone `GameAssembly.dll` above AppData, such as in a drive root or user-profile folder. The DLL does not need to be removed.
- Actual game folders remain blocked as patcher data locations. The private fix was confirmed working on an affected user's PC.

On v0.6.3, select **Check for updates → Update and restart**. If the error prevents startup, close the old patcher and open the current download above. This storage fix does not require reapplying translations; language packs, news, graphics and mods are unchanged.

**Changes since v0.6.2:**

- **Update and restart** downloads, verifies and replaces the patcher, then reopens it. Users on v0.6.2 or older download the current executable manually once; subsequent executable updates can use this button. Settings, recovery data and mods stay in place.
- **Apply** automatically refreshes missing or damaged translation data once before changing game files. Failed recovery reports a specific, sanitized data error.
- Missing patcher data folders are recreated automatically. **Change folder** and **Use default location** also work when the previous folder or drive is gone. Version 0.6.12 can rebuild missing Japanese backups when a valid recovery record identifies an exact verified original; keep those records.
- Recognized leftover CPDD full-text/UID helpers can be backed up and recreated without the old game folder or receipt; v0.6.12 handles this automatically during Apply. Unknown or official hotfix packages remain protected. Other game copies sharing the helper cache may need their patch reapplied.
- **291 reviewed dialogue corrections** preserve separate text variants, fixing repeated/merged dialogue in affected entries. Future scans check the same separators.
- **Français** is available under **Settings → Game language**. Missing or outdated French entries use current English.

For the v0.6.3 dialogue corrections, close the game and launcher, then select **Apply English** or **Apply translation**. These corrections also arrive as compatible data updates for v0.6.2. Existing mods, graphics and news are preserved. The corrected dialogue scene still needs in-game visual confirmation.

**Changes since v0.6.0:**

- 79 additional approved English graphics in **English Graphic Replacement**, for 84 total.
- A new **Hide HUD UID** method that keeps ping and signal bars visible. Applying English repairs the old method even when the option is now off, then retains the selected state.
- Better fitting gacha, gift and mission/dialogue-button text, with layout corrections across 26 interface assets.
- Clearer instructions for missing or empty resources: finish the remaining downloads using the **wrench-and-hammer icon on the title screen**, then close the game and launcher before applying again.

Select **Apply English** to update an existing installation. Enabled English graphics update automatically; otherwise, use **Mods → tick English Graphic Replacement → Install selected**. The v0.6.2 artwork support required an executable update once; later compatible artwork updates can be delivered as data.

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

**Restore Japanese** remains available for returning to native files. If an official update or repair already ran while patched, use **Apply English / Apply translation**; v0.6.12 handles supported repairs automatically. **Recover interrupted patch** handles interrupted patch transactions while preserving recovery records.

## Mods

Open the **Mods** tab, tick the features you want to change, then choose **Install selected** or **Uninstall selected** at the bottom. Checkboxes select the action's targets; installed status is shown separately. Selected changes run together while preserving translated text and unselected mods. Mods can be used before or after applying English and start off by default.

The **motion-sickness mods** group contains three independent options:

- **Disable Motion Blur:** disables the shared camera-motion-blur volume; separate combat blur can remain.
- **Disable Radial Blur:** disables radial and scan blur in the supported effect/story volumes; separate or runtime-controlled blur may remain.
- **Disable Shared Camera Shake:** disables the shared shake profile; other camera-shake effects may remain.

The other mods remain separate:

- **English Graphic Replacement:** 89 English UI graphics, including the five achievement-book titles and five additional larger replacements. Uninstall restores the original graphics.
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
