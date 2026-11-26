# Azur Promilia English — v0.5.9

CPDD community English patcher for the **Japanese PC client**. Community testers have successfully applied English and launched the game. This is a pre-release build; corrections and coverage updates will continue as the game updates.

## Download

Download **[AzurPromiliaEnglish.exe](https://github.com/Lani27/azur-promilia-english-patch/releases/download/patcher-v0.5.9/AzurPromiliaEnglish.exe)** from the [v0.5.9 release](https://github.com/Lani27/azur-promilia-english-patch/releases/tag/patcher-v0.5.9).

1. Finish updates through the official launcher, including any download on the game's first screen. Close the game and official launcher.
2. Open the patcher and select the folder containing `AzurPromiliaJP.exe`.
3. Select **Apply English**.
4. Select **Launch game**. The patcher checks for updates first and prompts when newer English/news data or a patcher release is available. It uses the game's normal graphics mode.

The current data contains **72,216 matching game/interface translation entries** and **23 news article bodies**. This includes 109 existing messages in the separate update-screen language file; loading tooltips have been confirmed in English in-game. News list/header titles remain Japanese. Optional English graphics cover the five achievement-book titles; other Japanese image lettering remains unchanged. Changed or unknown source strings remain untouched until matching English is available. Not every scene or text layout has been tested.

## Updates

English corrections, glossary changes, compatible new tables/IDs, supported interface locations and news articles can arrive as **data updates**, without downloading another executable. Updates are translated and prepared by maintainers; users apply them locally.

**Changes since v0.5.3:** 3,551 corrected English entries, reviewed terminology and ruby annotations, layout corrections across 22 interface assets, six additional news bodies and five optional achievement-book title graphics. Layout changes cover comparison/recommendation buttons, Kibo labels and values, role badges, Journey tasks, event rewards and observation banners. Some native dialogue choices still have the game's character-limit truncation.

Download v0.5.9 once for these new layout and optional-mod capabilities. Compatible future translation, news, layout and graphic changes remain data updates.

Before launch, **Update and launch** applies changed game data or refreshes news data. A newer optional executable offers a download; a required compatibility/fix release blocks launch until updated. If the online check cannot finish, the patcher asks before using verified saved data.

New binary formats or unsupported decoder changes may require another executable. Data packages cannot install executable code. Each translation must match the current Japanese source and context; old English is never selected by ID alone. News bodies are checked against fresh official article content before use.

Before official launcher updates or repairs, use **Restore Japanese**, finish the game update, then apply English again. **Recover interrupted patch** handles interrupted operations while preserving recovery records.

## Mods

Open the **Mods** tab and use each feature's **Install** or **Uninstall** button. Mods can be used before or after applying English and start off by default.

- **English Graphic Replacement:** English artwork for five achievement-book titles.
- **Disable Motion Blur:** disables the shared camera-motion-blur volume; separate combat blur can remain.
- **Disable TAA:** changes the last-used anti-aliasing profile, leaving DLSS/FSR/XeSS and FPS settings alone.
- **Async shaders (DX11):** experimental; uninstall if graphical errors appear.
- **No zoomed-in character fade:** keeps the character visible when the overworld camera is close.

Mod actions update only affected files, preserving English and other mods. **Remove all mods / Restore defaults** removes optional mods and graphics while keeping English text. **Restore Japanese** also restores owned mod files and saved anti-aliasing values. Close the game and official launcher before installing or uninstalling mods.

## Help

If an error occurs, use **Copy log** or **Open log** and send the sanitized patcher log through **[Get help on Discord](https://discord.gg/yyds)**. Errors include a specific next step. Share the patcher's log, rather than the game's account or launcher logs.

The patcher verifies the Japanese client's identity before checking compatibility. Automatic discovery uses local fixed drives and skips network paths and junctions. The Rust interface sleeps between events, uses VSync and caps redraws at 30 FPS.

## Distribution

This repository contains only this README and the update channel. Releases contain the executable, checksums and English/mapping/news data, never complete game archives or maintainer source, API tools, credentials or translation memory. Original game files and recovery records stay on each user's computer.

Downloads use this repository's HTTPS channel and release assets with SHA-256 and size verification. The channel is not separately signed; the publishing GitHub account is the update trust boundary. Game-content checks compare installed manifests with the published verified build and do not claim live authenticated server freshness.
