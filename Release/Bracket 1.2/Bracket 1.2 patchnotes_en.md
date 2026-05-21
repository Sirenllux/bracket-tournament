# Bracket 1.2 — Patch Notes

---

## Image Display

- Both images in a match are now displayed with **matched heights** side by side
- Images are **never cropped** — `object-fit: contain` is applied throughout
- Padding around images reduced for a better overall fit
- **WebP badge** added alongside the existing GIF badge
- GIF·WebP badge position **unified to top-left** across all previews (upload grid, folder thumbnails, entry list)

---

## Tournament Flow

### Mode Overhaul
- The old round-size selector has been replaced with **two distinct modes**
  - **Auto mode** (default): round size is calculated automatically from your upload count. Uneven numbers are handled with prelim matches and byes so everyone participates
  - **Random pick mode**: choose a round size (4·8·16·32·64…) and that many entries are drawn at random

### Preliminary Match Display
- A **prelim badge** is shown at the top during preliminary matches (`Prelim 2/6 · winner enters round-64`)
- Badge disappears automatically when the main bracket begins

### Match Screen
- **Source folder path** is now shown above each entry name
- Keyboard shortcuts remain: `←` / `1` = left, `→` / `2` = right

---

## Winner Screen

- **Win-ranking statistics panel** added after the tournament ends
  - 🥇🥈🥉 medal display, thumbnail, name, and win count
  - Relative bar chart showing each entry's performance
  - Entries with 0 wins are also listed
- Statistics panel **re-translates instantly** when the language is changed
- **Fixed a layout-breaking bug** on desktop when the statistics panel was too tall

---

## Themes

### 4 Dark Palettes
| | Palette | Vibe |
|---|---|---|
| 🟣 | **Purple** | Deep violet · lavender |
| 🔵 | **Ocean** | Dark teal · blue |
| 🩷 | **Rose** | Burgundy · pink |
| 💙 | **Slate** | Cool grey-blue |

### 4 Light Palettes
| | Palette | Vibe |
|---|---|---|
| 🟤 | **Paper** | Vintage cream (original) |
| 🟢 | **Mint** | Crisp white + teal accent |
| 🔴 | **Rose** | Warm pink tones |
| 🔘 | **Stone** | Cool neutral grey |

- Desktop: color dots shown in the header right, switching with the current theme
- Mobile: palette selector row shown above the help box in the Home tab
- Selected palette is saved to localStorage and persists across sessions

---

## Upload & File Management

- **Upload section moved above the mode selector** (upload → mode → start)
- **150 MB warning** added on mobile when uploading large batches (mobile-only)
- **X button on upload previews is always visible** on touch devices
- Clicking X now shows a **delete confirmation modal** (previously deleted immediately)
- **Folder delete** added: X button on folder card → confirmation modal → deletes all files inside
- **Individual file delete inside folders** added: delete button in entry list → confirmation modal
- **Name sort button removed** from the entry list toolbar

---

## UI / Tab Naming

- Tab names updated
  - `Setup` → **Home**
  - `Entries` → **Uploads**
- Page header and breadcrumb inside the Uploads tab updated to match

---

## Localization (KO · EN · JA)

- **Stop button** translation was missing — now fixed (KO: 중단 / EN: stop / JA: 中断)
- **Winner screen statistics panel** now re-translates correctly on language change
- Help text **fully rewritten in all three languages** to reflect current features
  - Auto / random mode explanations added
  - Prelim badge, GIF·WebP badge, folder path display, and win-ranking stats documented
  - Usage steps reordered (upload first, then select mode)
