# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

Landing page for **Couchday** — a gentle iOS/macOS day planner app. The site is a static HTML/CSS/JS site deployed to Cloudflare, live at [couchday.app](https://couchday.app).

## Deployment

**Pushing to `main` deploys the site.** Cloudflare's Git integration builds and
publishes automatically — no manual step, and nothing else is needed to go live.

```bash
git push origin main    # this is the deploy
```

Do **not** reach for `npx wrangler deploy`. The stored wrangler OAuth token is
long expired and won't refresh non-interactively, so it fails; its suggested
`--temporary` flag is worse, publishing to a throwaway account under a different
URL instead of updating the real site. If a direct deploy is ever genuinely
needed, re-auth first with `npx wrangler login`.

The `wrangler.jsonc` config serves the entire repo root as static assets
(`"directory": "."`). The `_headers` file controls HTTP response headers for
caching and security. URLs are served without the `.html` extension —
`/couchday-privacy.html` redirects (307) to `/couchday-privacy`.

To confirm a deploy landed, fetch the live page and check for the changed text
rather than only the absence of the old text (an error page also lacks it).

## Structure

- `index.html` — single-page marketing site (all CSS and JS inline, no build step)
- `privacy.html` / `couchday-privacy.html` — privacy policy pages
- `*.png` — app screenshots and icons referenced directly in HTML
- `_headers` — Cloudflare headers config (cache, security headers)
- `couch-habits-landing-page.md` — copy/content reference doc

## Design system

Dark theme (`#0a0a0f` background, white text). Accent color is warm orange (`#ff8b5f`). All CSS is inline in `index.html`. Scroll-triggered animations use `IntersectionObserver` with `.reveal` and `.stagger-children` classes. Parallax background uses floating gradient orbs.
