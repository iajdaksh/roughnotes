# 🗒️ Rough Notes

A browser-based floating notepad — minimal, keyboard-friendly, and built to stay out of your way. No accounts, no servers, no installs. Just open the HTML file and start writing.

---

## ✨ Features

### 📝 Floating Note Windows
- Open as many notes as you need — each one is a draggable, resizable window on a free canvas
- Drag notes anywhere, resize from the corner, and stack or spread them however you like
- Each note has an editable title so you can name and find things fast

### 💾 Persistent Storage
- Everything auto-saves to `localStorage` every 2 seconds
- Notes survive page refresh, browser close, and reopening — no manual saving needed
- Positions, sizes, content, font settings — all restored exactly as you left them
- Data stays until you clear browser history/site data

### 🗂️ Tabs Panel
- Side panel lists all open notes for quick access
- Search box to filter notes by name or content
- Navigate between notes with **↑ ↓ arrow keys** (when search is focused or nothing else is)
- Click any tab to bring that note to the front
- Minimize a note to a bubble, restore it from the tabs panel

### ⌨️ Keyboard Navigation
| Key | Action |
|-----|--------|
| `↑` / `↓` | Switch between open notes (tabs panel) |
| `←` / `→` | Move selection in Bin |
| `Enter` | Restore selected Bin item |

### 🗑️ Bin (Accidental Close Protection)
- Closing a note moves it to the **Bin** — not permanently deleted
- Bin shows a preview of each closed note
- Navigate bin cards with **← →** keyboard keys or the arrow buttons
- Press **Enter** or click to restore a note back to the canvas
- Bin holds the last **30** closed notes
- **Clear Bin** option with confirmation before permanent deletion
- Note numbering only resets when both open notes **and** bin are empty — no ID conflicts on restore

### ✕ Close All
- One-click button to close all open notes at once
- Always asks for confirmation first — all notes go to Bin, nothing is lost

### 🫧 Minimize to Bubble
- Minimize any note to a small floating bubble on the canvas
- Drag bubbles around freely
- Click a bubble or use the tabs panel to restore

### 🔤 Font & Size Controls
- 9 font choices: Caveat, Special Elite, Courier Prime, Merriweather, Space Mono, Inconsolata, Lora, Kalam, Satisfy
- Font size adjustable from 10px to 32px with + / − buttons
- Font settings apply across all notes and persist across sessions

### 📥 Import & Export
- **Upload** `.txt` files directly as notes (supports multiple files at once)
- **Download** any individual note as a `.txt` file
- **Save All** downloads all open notes at once

---

## 🚀 Getting Started

No build step, no dependencies, no server required.

```bash
# Clone the repo
git clone https://github.com/yourusername/rough-notes.git

# Open in browser
open rough-notes.html
```

Or just download `rough-notes.html` and open it in any modern browser.

---

## 🖥️ Browser Support

Works in all modern browsers that support `localStorage` and CSS custom properties:

- Chrome / Edge (recommended)
- Firefox
- Safari
- Mobile browsers (touch-friendly drag, resize, and bubble system)

---

## 📁 Project Structure

```
rough-notes/
└── rough-notes.html    # Single self-contained file — everything in one place
```

No frameworks, no build tools, no external dependencies (except Google Fonts loaded via CDN).

---

## 🎨 Design

- Dark-first aesthetic with a warm paper-ink feel
- Typography: [Cormorant Garamond](https://fonts.google.com/specimen/Cormorant+Garamond) for UI, multiple writing fonts for note content
- CSS custom properties throughout for easy theming
- Subtle animations on note open, bubble spawn, and panel transitions

---

## 🔒 Privacy

All data stays **100% local** in your browser's `localStorage`. Nothing is sent to any server. There are no analytics, no tracking, no network requests (except loading Google Fonts).

---

## 🛣️ Possible Future Ideas

- [ ] Light / dark theme toggle
- [ ] Per-note color coding
- [ ] Export all notes as a single `.zip`
- [ ] Markdown preview mode
- [ ] Note pinning / locking
- [ ] Drag notes between browser tabs (via BroadcastChannel)

---

## 📄 License

MIT — free to use, modify, and distribute.

---

*Built as a single HTML file. No frameworks. No fuss.*
