# BB — Bento Box Generator

A browser-based photo layout tool for building bento-style grids. No install, no build step — single HTML file.

## What it does

- Drag photos from your library onto any cell in the grid
- Pan and zoom photos inside each cell
- Resize cells by dragging the corner handle or using the +/− controls
- Pick cell shapes: rounded, square, circle, squircle, diamond, hex
- Choose from preset layouts or build a custom grid
- Export as PNG, JPEG, or WebP at any resolution with preset canvas sizes (1:1, 4:5, 9:16, 16:9) or custom pixel dimensions
- Work saves automatically in your browser — refreshing restores your last session

## Keyboard shortcuts

| Key | Action |
|-----|--------|
| `Cmd/Ctrl + Z` | Undo |
| `Cmd/Ctrl + Shift + Z` | Redo |
| `Delete` / `Backspace` | Remove selected cell |

## How to run locally

No build step needed — just open the file:

```bash
open index.html
# or
python3 -m http.server 8080
```

## How to contribute

1. Fork the repo
2. Create a feature branch (`git checkout -b feature/my-thing`)
3. Make changes and open a PR against `main`

Accepts JPEG, PNG, WebP, GIF, and HEIC/HEIF photos.

## Stack

- Vanilla HTML/CSS/JS (no framework, no bundler)
- [heic2any](https://github.com/alexcorvi/heic2any) for HEIC conversion
- Native Canvas 2D for image export
