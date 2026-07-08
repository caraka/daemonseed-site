# daemonseed-site

Source for **daemonseed.org** — the project + download site.

Hand-rolled static HTML + CSS. No framework, no build step, no JavaScript.

## Structure

```
index.html       home / hero / what-makes-it-different
download.html    per-platform downloads + verify instructions
about.html       project, license, provenance
404.html         not-found
styles.css       the whole design system (dark-first, light fallback)
favicon.svg      mark
_headers         Cloudflare Pages security headers (strict CSP, HSTS, no-referrer)
```

## Local preview

Any static server works, e.g.:

```
python3 -m http.server 8080
# → http://localhost:8080
```

## Deploy — Cloudflare Pages

Pure static site, so there is **no build**:

1. Cloudflare → Pages → connect this repo.
2. Build command: **(none)**. Build output directory: **`/`** (repo root).
3. Add the custom domain `daemonseed.org` once DNS is on Cloudflare.

`_headers` is applied automatically by Pages.

## Status

Staged, not live. Repo is **private** until launch. Go-live is a product decision — the
downloadable client is the serverless Veilid build; the site launches when the first
public alpha is ready for testers.

Built by `caraka`. AGPL-3.0-or-later.
