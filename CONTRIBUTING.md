# Contribute a translation

**[Submit a translation or correction on GitHub](https://github.com/Lani27/azur-promilia-english-patch/issues/new?template=translation.yml)**

English is the maintained base. The maintainer uploads English additions and corrections;
community translators use **Japanese → English → their language** to translate new
entries and review changed ones. Please report English errors in your submission
instead of editing the English reference yourself.

Community translation contributors (Discord): **Indonesian (rukathebest)** and **French (tonax.)**.
Brazilian Portuguese contributor: **reinhardwq**.
Additional GitHub contributors: **French [pedrokarim](https://github.com/pedrokarim)**, **Spanish [KarloZ7715](https://github.com/KarloZ7715)** and **Thai [CXZP](https://github.com/CXZP)**.

## Download an editable kit

Current kit release: **[translator-files-20261128.1](https://github.com/Lani27/azur-promilia-english-patch/releases/tag/translator-files-20261128.1)**.
English base: `camera-expanded-20261127-02`. Each file contains 72,216 entries.

| Language | ZIP with instructions | Editable JSON | Current coverage |
| --- | --- | --- | --- |
| Start a new language | [Blank kit](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.1/translator-kit.zip) | [translations.json](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.1/translations.json) | All targets blank |
| Bahasa Indonesia | [Indonesian kit](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.1/translations.id.zip) | [translations.id.json](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.1/translations.id.json) | 71,925 filled; 291 to review |
| Français | [French kit](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.1/translations.fr.zip) | [translations.fr.json](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.1/translations.fr.json) | 70,495 filled; 1,721 to translate/review |
| Español | [Spanish kit](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.1/translations.es.zip) | [translations.es.json](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.1/translations.es.json) | 71,925 filled; 291 to review |
| ไทย | [Thai kit](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.1/translations.th.zip) | [translations.th.json](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.1/translations.th.json) | 63,686 filled; 8,530 to translate/review |
| Português (Brasil) | [Brazilian Portuguese kit](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.1/translations.pt-BR.zip) | [translations.pt-BR.json](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.1/translations.pt-BR.json) | 71,445 filled; 771 to translate/review |

Choose a prefilled kit when your language already exists. These large JSON files
are hosted as release downloads. You can download them without a GitHub account;
sign in to GitHub to submit an issue. The ZIP includes the full [translator instructions](https://github.com/Lani27/azur-promilia-english-patch/releases/download/translator-files-20261128.1/TRANSLATING.md).

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
and retain previous wording for review. All five language ZIPs include `REVIEW.html`
and `review.json`. Indonesian, French, Spanish and Brazilian Portuguese each retain **291 translations
whose English references changed**. Two Indonesian dialogue-variant formatting errors have been corrected without
changing the translated wording. French has **1,430 other untranslated entries**. Thai retains **8,528
submitted translations needing formatting corrections**, plus **2 unfinished entries**.
Brazilian Portuguese retains **480 translations needing formatting corrections**. Its original wording is preserved for review.
Open `REVIEW.html` first; it shows the first 1,000 review entries, and `review.json`
contains the full list. Correct the target in the editable JSON, preserving
placeholders, numbers, tags and line breaks. Pending wording survives later kit refreshes.

Thai font support is included in patcher v0.6.6 and the hosted Thai language pack;
contributors do not need to edit fonts. Please report combining-mark or wrapping
problems with the affected text and a screenshot.

If you have already started work, submit it with its original kit version first.
Do not replace reference fields or overwrite your work with a newer kit. Only your
edits are merged; unchanged entries do not replace other contributors' newer work.
Changed references or conflicting corrections are held for review. Then continue
with the refreshed kit. Missing or outdated target text uses English fallback in
the game until an updated translation is published.
