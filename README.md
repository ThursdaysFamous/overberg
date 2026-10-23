# overberg.co

Personal landing page for **Adam Overberg** — civic tools and web apps built
on open government data, starting in Chicago.

Live at **[overberg.co](https://overberg.co/)**.

## What's here

Dependency-free static pages — a shared `style.css` (Modernist: Archivo, zero
radius, 2px rules, one red), an inline SVG mark (the Chicago flag star), no build
step and no framework, the same philosophy as the projects it links to. Served via
GitHub Pages (`CNAME` → `overberg.co`, `.nojekyll`).

- `index.html` — the landing page, a hub for what I'm currently building.
- `why/index.html` → **[overberg.co/why](https://overberg.co/why/)** — why
  districtry exists: the formats Illinois counties hand their boundary data
  over in, what the county-clerk correspondence returned, the same gap in
  other states, and the case for publishing the file you already have.

What it links out to:

- **[districtry](https://districtry.com/)** (formerly the Chicago District
  Explorer) — click any point (or search an address or ZIP code) and see every
  civic district that contains it, plus who represents you there. It started
  in Chicago and now answers in a growing list of states; its front page lists
  every live place, so this site links there rather than keeping its own list.
  The Illinois map is embedded live on the page.

The numbers on both pages (places live, Illinois layers, Illinois counties
served, recorded gaps) are read from
[districtry.com/stats.json](https://districtry.com/stats.json) when the page
loads; the values written in the HTML are only what a reader sees without
JavaScript, so update them when you touch the page.

## Develop

No build step. Open `index.html` directly, or serve the folder:

```bash
python3 -m http.server 8000   # then open http://localhost:8000/
```

## Deploy

Pushing to `main` publishes to [overberg.co](https://overberg.co/) via GitHub
Pages.
