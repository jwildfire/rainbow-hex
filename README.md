# rainbow-hex

A small style sheet: paper and graphite, plum links, three typefaces, and a seven-hue
spectrum seen through hex outlines. It is the look of [jwildfire.github.io](https://jwildfire.github.io).

**See it: https://jwildfire.github.io/rainbow-hex/**

One file, no scripts, no build step.

## Use it

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Instrument+Sans:wght@400;500;600&family=Instrument+Serif&family=IBM+Plex+Mono:wght@400;500&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://jwildfire.github.io/rainbow-hex/rainbow-hex.css">
<body style="--dept:var(--spec-3)">
```

| You are making | Take |
|---|---|
| A new page or report | `index.html` as a template, with `rainbow-hex.css` |
| An app with its own styles | `rainbow-hex-tokens.css`: the colours and type as CSS variables, no rules |
| Charts, canvas, R | `rainbow-hex-tokens.json`: the same as data, with a chart order |
| A favicon or a logo | `hex-mark.svg` |

## The rainbow hex

The spectrum is only ever seen through hexes or as a thin edge. It never colours text
and never fills a plain area.

| Class | What it is |
|---|---|
| `hr`, `.hexline` | The strip: a divider, once or twice a page |
| `.hexband`, `.hexband.fade` | A band of honeycomb for the top of a page; one a page |
| `.hexfield` | A quiet honeycomb behind a block |
| `.hexmark` | One small rainbow hex: a logo or a bullet |
| `.hex`, `.hex.ring` | A picture or initials in a hex |
| `ul.hexlist` | Hex bullets in the page's colour |
| `.spec-edge` | The spectrum as a thin line on top of a card |

Also: `.card`, `.chip`, `.tag`, `.btn`, `.bar`, `.stats`, `details.row`, `.callout`, `.topbar`,
`.swatches`. The sample page shows each one.

## Colour

Seven hues at the same lightness, `--spec-0` to `--spec-6`. A page or section takes one as
its own (`--dept`). Light and dark follow the system; `data-theme="light"` or `"dark"` on
the `html` element overrides.

## Licence

MIT. See [LICENSE](LICENSE). The typefaces are loaded from Google Fonts under their own licences.
