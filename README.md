# Behnke-IT — Website

Single-page static site for **Daniel Behnke / Behnke-IT**. No build step, no dependencies.

- `index.html` — the whole site (inline CSS + JS)
- `assets/` — logo mark
- `netlify.toml` — Netlify deploy config
- `robots.txt` / `sitemap.xml` — SEO basics

## Deploy to Netlify

**Option 1 — Git integration (recommended):**
1. In Netlify: *Add new site → Import from Git → GitHub → Behnke-IT/website*
2. Build command: *(leave empty)* — Publish directory: `.`
3. Deploy. The repo's `netlify.toml` already sets these.

**Option 2 — CLI:**
```bash
npm i -g netlify-cli
netlify deploy --prod --dir .
```

## Local preview

Any static server works. Easiest:
```bash
python3 -m http.server 4000
# → http://localhost:4000
```

## Editing content

Everything lives in `index.html`. The site is bilingual (EN/DE) — both copies live inline in the same document and swap via the language toggle, so edit both when you change copy.

## License

© Daniel Behnke. All rights reserved.
