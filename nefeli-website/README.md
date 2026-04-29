# nefeli-website

Quarto source for the personal portfolio. See the [repo root README](../README.md)
for what's on the site and overall layout.

**Live:** https://nefelizafeiri.github.io/portfolio/

## Local preview

```bash
# One-time install
# https://quarto.org/docs/get-started/

cd nefeli-website
quarto preview
```

The preview opens in the browser at `http://localhost:4040` and live-reloads
as you edit `index.qmd`, `capstone.qmd`, or `styles.css`.

## Deploying

The site auto-deploys via GitHub Actions on every push to `main` — see
[`.github/workflows/main.yml`](../.github/workflows/main.yml) (in the repo
root). No manual `quarto render` or upload step needed.

To preview the rendered output without pushing:

```bash
quarto render
open docs/index.html
```

## Project structure

```
nefeli-website/
├── _quarto.yml              # Site config (theme, title, output dir)
├── index.qmd                # Hero + Education + Experience + Projects + Activities + Skills
├── capstone.qmd             # Deloitte capstone detail page (linked from project card)
├── styles.css               # Custom SCSS — palette, hero, project cards, tabs
├── headshot.jpg             # Hero portrait
└── docs/                    # Quarto build output — committed for GitHub Pages
```

## Editing tips

- **Adding a project card** — add a `.project-card` block inside the `#projects`
  section in `index.qmd`. Cards in reverse-chronological order (newest first).
- **Featured project styling** — apply the `project-card-featured` class for the
  accent line on the left edge.
- **Tab nav** — section IDs (`education`, `experience`, `projects`, `activities`,
  `skills`) drive the sticky tab nav and IntersectionObserver-based active state
  in the script at the bottom of `index.qmd`.
- **Color palette** — defined as CSS custom properties at the top of `styles.css`
  (`--ink`, `--surface`, `--accent`, etc.).
