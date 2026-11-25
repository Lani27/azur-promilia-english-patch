# Azur Promilia English patcher

CPDD community English patcher for the Japanese Azur Promilia client. Get help and updates in [CPDD Discord](https://discord.gg/yyds).

**Development preview:** the desktop updater and local patching/recovery tools are available. Full English translation is still being generated. In-game loading and layout have not yet been verified. The preview will download English data when a validated release is published; it will not apply an incomplete catalog.

## Download

Download `AzurPromiliaEnglish.exe` from the [Rust patcher preview](https://github.com/Lani27/azur-promilia-english-patch/releases/tag/patcher-v0.2.0).

1. Open the patcher and select the folder containing `AzurPromiliaJP.exe`.
2. Let it check for the latest English data.
3. Finish any launcher update, then launch the game and finish its first-screen download. Close the game before choosing **Apply English**.
4. Use **Restore Japanese** to restore the exact locally backed-up files. Use **Recover interrupted patch** if an operation was interrupted.

The preview currently displays **English translation is in progress** until the complete catalog is available.

The Rust app uses an Azur Promilia theme and the CPDD icon. Automatic detection checks local fixed drives and Windows installation records; network drives and junctions are skipped. You can browse to another local installation. The UI sleeps between events, enables VSync, and caps redraws at 30 FPS.

## Help and recovery

Errors show a short explanation and the next step. Use **Open log** or **Copy log**, then [Get help on Discord](https://discord.gg/yyds). Logs are stored under `%LOCALAPPDATA%\AzurPromiliaEnglish\logs`.

**In-game update required** means your content packages are older than the published verified build. Open the game through its official launcher, let the title-screen download finish, then close it and reopen the patcher. This check is separate from English-data and executable updates. It compares against published game-content requirements; it does not query the game's authenticated version service or claim live server freshness. If no comparison is available, the app says the content version is unverified.

## Updates

English translations, glossary corrections and supported mapping changes are published as separate data packages. Existing users receive those through the patcher without another executable download.

An executable-update notice appears only when a data release requires a newer engine capability or a necessary patcher fix. A merely newer executable does not cause a notice.

Every build discovers the installed Japanese tables and row IDs again. English must match the exact current Japanese text and logical context. Changed or unknown strings stay Japanese until maintainers translate the new source. No old translation is selected by ID alone.

Players rebuild game files locally. Releases contain the patcher and English/mapping data, never complete game archives. Local originals and recovery records remain on the player's computer under `%LOCALAPPDATA%\AzurPromiliaEnglish`.

The updater uses this repository's HTTPS channel and release assets, verifies SHA-256 and file sizes, and retains compatible cached data for offline use. Packages cannot install scripts or executables. The current channel is not separately signed; the publishing GitHub account is the update trust boundary.

This is the distribution repository. Its Git tree contains only this README and the small update pointer. The executable and English data are GitHub Release downloads. Local extraction data, translation memory, credentials, maintainer API code and development files are not published here.
