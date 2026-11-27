# Contribute a translation

**[Submit a translation or correction on GitHub](https://github.com/Lani27/azur-promilia-english-patch/issues/new?template=translation.yml)**

English is the maintained base. The maintainer uploads English additions and corrections;
community translators use **Japanese → English → their language** to translate new
entries and review changed ones. Please report English errors in your submission
instead of editing the English reference yourself.

Indonesian contributor: **rukathebest (Discord)**.
French contributors: **tonax. (Discord) / [TonySanchezD](https://github.com/TonySanchezD) (GitHub)** and **[pedrokarim](https://github.com/pedrokarim) (GitHub)**.
Brazilian Portuguese contributor: **reinhardwq**.
Spanish contributor: **[KarloZ7715](https://github.com/KarloZ7715) (GitHub)**.

## Download an editable kit

Current kit release: **[translator-files-20261128.6](https://github.com/Lani27/azur-promilia-english-patch/releases/tag/translator-files-20261128.6)**.
English base: `content-3273853-20261128`. Each file contains 72,190 entries.
Coverage below describes this kit version; hosted language packs may contain newer corrections.

| Language | ZIP with instructions | Editable JSON | Kit coverage |
| --- | --- | --- | --- |
| Start a new language | [Blank kit](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.6/translator-kit.zip) | [translations.json](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.6/translations.json) | All targets blank |
| Bahasa Indonesia | [Indonesian kit](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.6/translations.id.zip) | [translations.id.json](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.6/translations.id.json) | 69,512 filled; 2,678 to translate/review |
| Français | [French kit](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.6/translations.fr.zip) | [translations.fr.json](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.6/translations.fr.json) | 69,802 filled; 2,388 to translate/review |
| Español | [Spanish kit](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.6/translations.es.zip) | [translations.es.json](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.6/translations.es.json) | 69,512 filled; 2,678 to translate/review |
| Português (Brasil) | [Brazilian Portuguese kit](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.6/translations.pt-BR.zip) | [translations.pt-BR.json](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.6/translations.pt-BR.json) | 69,072 filled; 3,118 to translate/review |

Choose a prefilled kit when your language already exists. These large JSON files
are hosted as release downloads. You can download them without a GitHub account;
sign in to GitHub to submit an issue. The ZIP includes the full [translator instructions](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.6/TRANSLATING.md).

## Translate or correct text

1. Unzip the kit and open its JSON in a UTF-8 text editor.
2. For a new language, fill in `target_locale` and `target_name`. Keep an existing language's code and name.
3. Read `source` (Japanese), `english` (maintained reference) and `context`. Edit `target`; use `notes` for questions or explanations.
4. Keep every entry, ID, hash, Japanese/English reference and context unchanged. Preserve placeholders, numbers, tags and line breaks. Leave unfinished targets empty.
5. Save the whole JSON and ZIP it. Partial contributions and corrections to existing targets are welcome.

## Submit through GitHub

Open **[Translation submission](https://github.com/Lani27/azur-promilia-english-patch/issues/new?template=translation.yml)**.
Enter your language and the kit release version, then drag your ZIP into the
**Translation file or correction details** box and submit the issue. A fork or
pull request is not required. GitHub allows ZIP attachments up to 25 MB; if your
file exceeds that, share a download link in the same box. See [GitHub's attachment instructions](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/attaching-files).

For a small correction, a file is optional: include the entry ID, current wording,
suggested replacement and enough context to explain it. If you cannot find the ID,
include the exact text and where it appears in the game. A screenshot can help.

Submissions and attachments are public. Include only translation material and
relevant notes. The maintainer reviews and validates each contribution, merges it
against the exact kit version you used, and resolves conflicting edits before
publishing a language update. Submitting an issue does not automatically update
the patcher. Approved updates reach players through the patcher's normal language
downloads and update checks.

## When English changes

The maintainer refreshes kits against the latest maintained English and publishes
a new version here. Existing translations carry over when their references still
match. Refresh review reports identify new, changed, missing or invalid entries
and retain previous wording for review. All four language ZIPs include `REVIEW.html`
and `review.json`.

This refresh identifies **2,305 new entries** in each language. Indonesian, Spanish
and Brazilian Portuguese each have **373 entries with changed references**;
French has **83**. Brazilian Portuguese also retains **440
translations needing formatting corrections**, with the original wording preserved
for review. Each review report preserves **2,331 removed entries** separately from
the editable current catalog.

Open `REVIEW.html` first; it shows the first 1,000 review entries, and `review.json`
contains the full list. Correct the target in the editable JSON, preserving
placeholders, numbers, tags and line breaks. Pending wording survives later kit refreshes.

**Thai translation withdrawn:** The previous Thai contribution and its hosted packs
and kits have been removed; see [issue #8](https://github.com/Lani27/azur-promilia-english-patch/issues/8#issuecomment-7229327535).
Only submit translations you created or have permission to share. Any new Thai
contribution must start from the blank kit.

If you have already started work, submit it with its original kit version first.
Do not replace reference fields or overwrite your work with a newer kit. Only your
edits are merged; unchanged entries do not replace other contributors' newer work.
Changed references or conflicting corrections are held for review. Then continue
with the refreshed kit. Missing or outdated target text uses English fallback in
the game until an updated translation is published.
