# Height Comparison

A local, offline height-comparison chart builder for OCs and RPG characters.

**Live: https://gaelziade.github.io/height-compare/**

Load PNGs, tell it where the floor and the top of the head are, give each character a
height, and it lines them up against a mugshot-style scale. Everything runs in the
browser — your images are never uploaded anywhere.

## What it does

- **Load PNGs** — button or drag them onto the canvas. Transparent backgrounds work best.
- **Calibrate floor & head** — two draggable lines per character. Accessories that stick out
  (guitars, weapons, cat ears, hats) still get drawn, they just don't count toward the height.
  The floor/head lines are guessed automatically from the image's alpha crop.
- **Any height format** — `1.85`, `185`, `185cm`, `6'1"`, `6ft2`, `73in`.
- **Background scale** — mugshot-style lines with labels, spacing configurable in inches or cm.
- **Silhouettes** — per character or all at once, each in its own color or one color for everybody.
- **Colored outlines** — per character, with adjustable thickness, so overlapping silhouettes
  stay readable.
- **Eyedropper** — sample a color straight off the artwork (hair, armor, eyes), or use the
  dominant-color swatches. A screen-wide eyedropper is available in Chrome/Edge.
- **Layout** — reorder left to right, drag to overlap, choose who draws on top, raise characters
  off the ground (Shift+drag) for anyone flying.
- **Custom backgrounds** — image or solid color, with cover/contain/stretch/tile and opacity.
- **Export PNG** up to 4x, cropped to the characters, with a transparent background if you want one.
- **Projects** autosave in the browser, and save/load as `.json` (images included) to share or back up.

## Units

Labels can read `1.85 m (6'1")`, `1.85 m`, `185 cm`, or `6'1"`. Imperial can be shown as
`6'1"` or `6 ft 1 in`. Internally everything is centimeters, so switching units never
changes a character's actual height.

## Shortcuts

| Action | Key |
| --- | --- |
| Move a character | drag |
| Raise / lower (flying characters) | Shift + drag |
| Zoom | mouse wheel |
| Pan | middle button, or Space + drag |
| Delete selected | Del |
| Fit everything on screen | F |

## Running it locally

No build step, no dependencies, no server. Download `index.html` and open it in a browser —
it works offline and behaves exactly like the hosted version.

## License

MIT
