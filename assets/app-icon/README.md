# ZAC app icon

A bold "Z" with an amber gradient (`#ffd24a` → `#ff7a1a`) between light-blue code brackets
(`#7fb4ff`), on a rounded navy tile (`#14306a` → `#081530`). Shapes only, no text or fonts, so
the app can draw the SVG itself at any size. It is not open source: see `LICENSE.txt`.

## Geometry

A 512-unit tile with 110-unit corners. The macOS icons pad the tile onto Apple's 824/1024 icon
grid; every other render uses the full tile.

## Files

- `craft-anything.svg`: the master SVG (also the hicolor scalable icon).
- `craft-anything-1024.png`: 1024 px render of the tile.
- `craft-anything.icns`: macOS bundle icon.
- `craft-anything.ico`: Windows icon (16, 20, 24, 32, 40, 48, 64, 128, 256).
- `hicolor/<size>/apps/ai.storyteller.craft-anything.png` (16–512) and
  `hicolor/scalable/apps/ai.storyteller.craft-anything.svg`: Linux icon theme.
- `trace.py`: upstream tool that traces raster artwork into an SVG (not used by the ZAC icon).

The file names are kept from upstream so build scripts and packaging need no change. The app draws
the SVG itself at the exact pixel size (title bar, welcome screen); the window icon is the 256 px PNG.

## Regenerate

```sh
packaging/icons.sh   # needs resvg on PATH; the .icns needs macOS's iconutil
```

On Windows without resvg, the current files were rendered with Inkscape, and the `.ico` and `.icns`
were packed with Pillow.
