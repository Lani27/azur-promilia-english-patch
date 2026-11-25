# Azur Promilia English patcher

Community English patcher for the Japanese Azur Promilia client.

**Development preview:** the desktop updater and local patching/recovery tools are available. Full English translation is still being generated. In-game loading and layout have not yet been verified. The preview will download English data when a validated release is published; it will not apply an incomplete catalog.

## Download

Download `AzurPromiliaEnglish.exe` from the [patcher preview release](https://github.com/Lani27/azur-promilia-english-patch/releases/tag/patcher-v0.1.0). Discord can link directly to this release.

1. Open the patcher and select the folder containing `AzurPromiliaJP.exe`.
2. Let it check for the latest English data.
3. Close the game and finish any launcher update before choosing **Apply English**.
4. Use **Restore Japanese** to restore the exact locally backed-up files. Use **Recover interrupted patch** if an operation was interrupted.

The preview currently displays **English translation is in progress** until the complete catalog is available.

## Updates

English translations, glossary corrections and supported mapping changes are published as separate data packages. Existing users receive those through the patcher without another executable download.

An executable-update notice appears only when a data release requires a newer engine capability or a necessary patcher fix. A merely newer executable does not cause a notice.

Every build discovers the installed Japanese tables and row IDs again. English must match the exact current Japanese text and logical context. Changed or unknown strings stay Japanese until maintainers translate the new source. No old translation is selected by ID alone.

Players rebuild game files locally. Releases contain the patcher and English/mapping data, never complete game archives. Local originals and recovery records remain on the player's computer under `%LOCALAPPDATA%\AzurPromiliaEnglish`.

The updater uses this repository's HTTPS channel and release assets, verifies SHA-256 and file sizes, and retains compatible cached data for offline use. Packages cannot install scripts or executables. The current channel is not separately signed; the publishing GitHub account is the update trust boundary.

This is the distribution repository. Its Git tree contains only this README and the small update pointer. The executable and English data are GitHub Release downloads. Local extraction data, translation memory, credentials, maintainer API code and development files are not published here.
