# Emira 2026 — Ditëlindja

A one-page birthday microsite for Emirë, tuned for iPhone 16 Pro / 17 Pro.

## Run locally

Any static server works. Easiest:

```bash
python3 -m http.server 8765
# then open http://127.0.0.1:8765
```

## Deploy to Vercel

1. Push this folder to a GitHub repo.
2. Import the repo in Vercel — no build step, no framework preset needed.
3. Deploy.

The included `vercel.json` sets long cache headers on `/assets/*`.

## Structure

```
index.html      one page, semantic markup
styles.css      mobile-first, fluid scale from viewport up to 500px cap
assets/         photos, icon, decorative SVGs
```

All positioning is done in a single logical-pixel unit (`--u`) that scales
with the viewport, so it looks the same at iPhone 16 Pro (393pt) and
17 Pro (402pt), and centered on desktop.
