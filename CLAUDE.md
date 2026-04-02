# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

Landing page for **Couchday** — a gentle iOS/macOS day planner app. The site is a static HTML/CSS/JS site deployed to Cloudflare via Wrangler.

## Deployment

```bash
npx wrangler deploy    # deploy to Cloudflare Workers (static assets)
```

The `wrangler.jsonc` config serves the entire repo root as static assets (`"directory": "."`). The `_headers` file controls HTTP response headers for caching and security.

## Structure

- `index.html` — single-page marketing site (all CSS and JS inline, no build step)
- `privacy.html` / `couchday-privacy.html` — privacy policy pages
- `*.png` — app screenshots and icons referenced directly in HTML
- `_headers` — Cloudflare headers config (cache, security headers)
- `couch-habits-landing-page.md` — copy/content reference doc

## Design system

Dark theme (`#0a0a0f` background, white text). Accent color is warm orange (`#ff8b5f`). All CSS is inline in `index.html`. Scroll-triggered animations use `IntersectionObserver` with `.reveal` and `.stagger-children` classes. Parallax background uses floating gradient orbs.

## Notes

- The App Store link in `index.html` still uses the placeholder `YOUR_APP_ID` — update when the app is live.
- Images referenced in HTML (e.g. `Couchday-timeline.png`, `Couchday-widgets.png`, `Couchday-activities.png`, `Couchday-widget-preview.png`) may not all exist in the repo yet.
