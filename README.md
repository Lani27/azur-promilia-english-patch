# Azur Promilia English — v0.5.3 Pre-Launch

CPDD community English patcher for the **Japanese PC client**. Community testers have successfully applied English and launched the game. This is a pre-release build; corrections and coverage updates will continue as launch content arrives.

## Download

Download **[AzurPromiliaEnglish.exe](https://github.com/Lani27/azur-promilia-english-patch/releases/download/patcher-v0.5.3/AzurPromiliaEnglish.exe)** from the [v0.5.3 Pre-Launch release](https://github.com/Lani27/azur-promilia-english-patch/releases/tag/patcher-v0.5.3).

1. Finish updates through the official launcher, including any download on the game's first screen. Close the game.
2. Open the patcher and select the folder containing `AzurPromiliaJP.exe`.
3. Select **Apply English**.
4. Select **Launch game**. The patcher checks for updates first and prompts when newer English/news data or a patcher release is available. It uses the game's normal graphics mode.

The current data contains **72,216 matching game/interface translation entries** and **17 news article bodies**. This includes 109 existing messages in the separate update-screen language file; loading tooltips have been confirmed in English in-game. News list/header titles and Japanese lettering inside images remain untranslated. Changed or unknown source strings remain untouched until matching English is available. Not every scene or text layout has been tested.

## Updates

English corrections, glossary changes, compatible new tables/IDs, supported interface locations and news articles can arrive as **data updates**, without downloading another executable. Updates are translated and prepared by maintainers; users apply them locally.

**v0.5.3 removes the DirectX 12 option and supports menu-label line breaks.** “Garden of Star-Source” keeps its full name and displays on two lines. Successful launch and the corrected menu layout have been confirmed in-game. Required executable updates open a download dialog as soon as the update check finishes, and important controls remain visible without scrolling. Download this executable once if you are using an older version; compatible future label-layout changes can arrive through data updates.

The update-screen language file is supported. Future compatible translation and glossary updates continue to arrive as data updates, without another executable download.

Before launch, **Update and launch** applies changed game data or refreshes news data. A newer optional executable offers a download; a required compatibility/fix release blocks launch until updated. If the online check cannot finish, the patcher asks before using verified saved data.

New binary formats or unsupported decoder changes may require another executable. Data packages cannot install executable code. Each translation must match the current Japanese source and context; old English is never selected by ID alone. News bodies are checked against fresh official article content before use.

Before official launcher updates or repairs, use **Restore Japanese**, finish the game update, then apply English again. **Recover interrupted patch** handles interrupted operations while preserving recovery records.

## Help

If an error occurs, use **Copy log** or **Open log** and send the sanitized patcher log through **[Get help on Discord](https://discord.gg/yyds)**. Errors include a specific next step. Share the patcher's log, rather than the game's account or launcher logs.

The patcher verifies the Japanese client's identity before checking compatibility. Automatic discovery uses local fixed drives and skips network paths and junctions. The Rust interface sleeps between events, uses VSync and caps redraws at 30 FPS.

## Distribution

This repository contains only this README and the update channel. Releases contain the executable, checksums and English/mapping/news data, never complete game archives or maintainer source, API tools, credentials or translation memory. Original game files and recovery records stay on each user's computer.

Downloads use this repository's HTTPS channel and release assets with SHA-256 and size verification. The channel is not separately signed; the publishing GitHub account is the update trust boundary. Game-content checks compare installed manifests with the published verified build and do not claim live authenticated server freshness.
