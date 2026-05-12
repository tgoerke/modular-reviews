# Atmospheric Reviews

Landing page for [atmospheric.reviews](https://atmospheric.reviews/) — a modular peer-review protocol for science conducted in the AT Protocol Atmosphere.

> *Note: this repo was previously an Astro site hosting an umbrella "Atmospheric Computing" landing covering four pillars. As of 2026-05, it has been refactored to focus on atmospheric.reviews alone (atmospheric.computer moved to a separate repo).*

## Local Development

Prerequisites: Hugo extended ≥ 0.159, Node 20+, pnpm.

```bash
pnpm install
pnpm run dev      # http://localhost:1313
pnpm run build    # produces ./public
```

## Structure

```
content/_index.md            # home page sections
config/_default/             # site configuration
data/authors/                # author profiles (team)
static/                      # files served as-is (CNAME, talks/)
.github/workflows/           # build + deploy to GitHub Pages
```

## Deployment

Pushes to `main` trigger the Hugo build + GitHub Pages deploy. CNAME is set to `atmospheric.reviews`.

## Tech Stack

[Hugo](https://gohugo.io/) (extended) + [Hugo Blox](https://hugoblox.com/) dev-portfolio template, deployed to GitHub Pages.
