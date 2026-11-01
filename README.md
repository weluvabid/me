# me

A small home for my personal identity assets.

## Structure

```text
.
├── brand/
│   ├── mark.svg
│   └── mark-dark.svg
├── favicon/
│   ├── favicon.svg
│   └── favicon.ico
└── exports/
    ├── brand/       # PNG raster exports of the mark
    └── favicon/     # PNG favicon exports
```

## Using the mark

- `brand/mark.svg` — white mark for dark surfaces.
- `brand/mark-dark.svg` — dark mark for light surfaces.
- `favicon/favicon.svg` — white mark on a rounded dark tile.
- `favicon/favicon.ico` — multi-resolution browser icon.
- `exports/` — pre-rendered PNG sizes for contexts that need raster assets.

Prefer the SVG files whenever the consuming platform supports them.

## Favicon

For a website, copy the favicon assets into its public/static directory and reference the SVG with an ICO fallback:

```html
<link rel="icon" href="/favicon.svg" type="image/svg+xml" />
<link rel="alternate icon" href="/favicon.ico" />
```

Adjust the paths to match the consuming project's base path and asset conventions.
