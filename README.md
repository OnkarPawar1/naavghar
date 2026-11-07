# Naavghar · नावघर

An editorial, bilingual Marathi baby boy names explorer built as a static website for **GitHub Pages**. Inspired by the design discipline of [Nutlope/hallmark](https://github.com/Nutlope/hallmark): readable contrast, task-first navigation, visual craft, responsive layouts and reduced-motion support. The project does not copy Hallmark's assets or depend on installing Hallmark.

## All source names included

- **List A:** 711 numbered entries, including repeated names and source variations.
- **List B:** 500 numbered entries, including repeated names and source variations.
- **List C:** 630 entries, including repeated entries and English-only source names.
- **Total: 1,841 source entries, with no deduplication in the underlying data.** The optional *Hide repeated spellings* filter changes only what is displayed.

List C supplies no Marathi spellings. Where English names match A/B, the source-provided Marathi spellings are reused; otherwise a phonetic Marathi spelling is suggested and **clearly marked as approximate**. Please verify before using officially. Imported meaning text is reproduced from source listings and may include inconsistencies. The three files are represented as A/B/C in the names dataset, without republishing editorial boilerplate.

## Features

Search English, Marathi, meanings and personal notes; filter by letter, source, bookmark, shortlist, reviewed or highlight; preserve checked status; bookmark and shortlist entries; colour-code entries in six shades; edit English and Marathi spelling, meanings and notes; switch grid/list; sort; select displayed names; bulk review/shortlist/print; print filtered results or saved shortlist; download CSV; export and restore a JSON backup; six colour themes; responsive design; keyboard `/` to search. All personal settings are saved to your browser using `localStorage`.

**Important:** GitHub Pages is static. Edits and shortlists are **not synchronized between devices**. Use **Back up my changes** and **Restore a backup** for portability. Visitors can't change `names.json` on the GitHub repository through the website.

## Deploy to GitHub Pages

1. On GitHub, create a **public** repository named `naavghar` (or another name).
2. Upload `index.html`, `styles.css`, `app.js`, and `names.json` to the repository root. The included `build_data.py` is optional and is for reproducible local parsing only; it requires the original uploaded source files in its hardcoded paths.
3. In **Settings → Pages**, set **Build and deployment → Deploy from a branch**, choose `main` and `/(root)`, then save.
4. Your website address will be `https://YOUR-USERNAME.github.io/naavghar/`. It may take several minutes to become available.

To preview locally:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`. Opening `index.html` directly with a `file://` URL will normally block the JSON fetch.

## File layout

```
index.html       Page markup
styles.css      Theme, responsive design, print stylesheet
app.js          Filtering, shortlist, edits, browser storage
names.json      All 1,841 source entries
build_data.py   Optional local data reconstruction script
```

This site uses Google Fonts when online and includes system-font fallbacks.