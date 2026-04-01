# Deep Learning Book (Quarto)

A Quarto-based online textbook project that mirrors the VisionBook delivery style: chapter-based navigation, searchable HTML pages, and static deployment.

## Requirements

- Quarto CLI
- GitHub repository (for Pages deployment)

## Local development

```bash
quarto check
quarto preview
```

## Build static HTML

```bash
quarto render
```

Output is generated in `_site/`.

## Authoring patterns (VisionBook-like)

- Footnote:
  `Deep learning needs strong optimization intuition.[^opt]`
  `[^opt]: This is a footnote body.`
- Figure with cross-reference hover preview:
  `As shown in @fig-training-surface, ...`
  `![Caption](../figures/training-surface.svg){#fig-training-surface}`
- Image click-to-zoom:
  Enabled by `format.html.lightbox: true` in `_quarto.yml`.

## Deploy

Push to `main`. GitHub Actions renders and deploys to GitHub Pages.
