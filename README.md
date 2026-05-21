# 🏆 Bracket — Image Tournament

> Pick your favorite. One match at a time.

A single-file, zero-dependency browser app for running image-based tournaments. Upload photos of your favorite characters, foods, movies, or anything — then click your way to a champion.

---

## Features

**Tournament modes**
- **Auto mode** — round size is calculated automatically from your upload count. Odd numbers are handled gracefully with prelim matches and byes so everyone participates.
- **Random pick mode** — choose a round size (4 / 8 / 16 / 32 / 64…) and that many entries are drawn at random.

**Match screen**
- Side-by-side image comparison with equalized heights
- Source folder shown above each entry name
- Preliminary match badge with live progress (`Prelim 2/6 · winner enters round-64`)
- Keyboard shortcuts: `←` / `1` for left, `→` / `2` for right

**Winner screen**
- Champion display with full win-ranking statistics
- Medal rankings 🥇🥈🥉, win count, and relative bar chart for all participants

**File management**
- Upload individual images, a folder (preserving folder structure), or a ZIP file
- Supported formats: PNG · JPG · GIF · WebP · ZIP
- GIF and WebP files are marked with badges
- Delete individual entries or entire folders — both with confirmation modals
- All data persisted via IndexedDB (localStorage fallback)

**Theming**
- 4 light palettes: Paper · Mint · Rose · Stone
- 4 dark palettes: Purple · Ocean · Rose · Slate
- Palette preference saved across sessions

**Localization**
- Full UI in Korean · English · Japanese
- Language preference saved across sessions

---

## Usage

No build step. No dependencies. Just open `index.html` in a browser.

```
git clone https://github.com/your-username/bracket.git
cd bracket
open index.html
```

Or drop `index.html` anywhere and open it directly — it works fully offline after the first load (fonts and JSZip are loaded from CDN on first visit).

---

## Mobile

- ZIP upload is recommended on mobile instead of folder selection (folder picker is unavailable on iOS Safari)
- Uploading more than ~150 MB at once may cause the browser to crash on low-memory devices — split large batches into smaller uploads
- All interactions are touch-optimized; delete buttons are always visible on touch devices

---

## Tech

| | |
|---|---|
| Language | Vanilla HTML / CSS / JavaScript |
| Storage | IndexedDB (localStorage fallback) |
| ZIP parsing | [JSZip](https://stuk.github.io/jszip/) via CDN |
| Font | [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) via Google Fonts |
| Dependencies | None (runtime) |

---

## License

MIT
