# overberg.co

Personal landing page for **Adam Overberg** — civic tools and web apps built
around Chicago and open government data.

Live at **[overberg.co](https://overberg.co/)**.

## What's here

A single, dependency-free static page (`index.html`) — inline CSS and an inline
SVG mark (the Chicago flag star), no build step and no framework, the same
philosophy as the projects it links to. Served via GitHub Pages (`CNAME` →
`overberg.co`, `.nojekyll`). It's a hub for what I'm currently building:

- **[Chicago District Explorer](https://chidistricts.com/)** — click any point
  in Chicago (or search an address) and see every civic district that contains
  it — ward, police district, community area, congressional and state
  legislative districts, elected school board, CPS zones, and more — plus who
  represents you there. Embedded live on the page.
- **[District Explorer: New York City](https://nyc.chidistricts.com/)** — the
  same lookup, ported to NYC.
- **[District Explorer: San Francisco](https://sf.chidistricts.com/)** — ported
  to SF.

## Develop

No build step. Open `index.html` directly, or serve the folder:

```bash
python3 -m http.server 8000   # then open http://localhost:8000/
```

## Deploy

Pushing to `main` publishes to [overberg.co](https://overberg.co/) via GitHub
Pages.
