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
_headers         security headers (strict CSP, HSTS, no-referrer)
```

## Local preview

Any static server works, e.g.:

```
python3 -m http.server 8080
# → http://localhost:8080
```

## Status

Live at <https://daemonseed.org>. The downloadable client is the serverless Veilid
build — first signed alpha binaries land shortly on the
[daemonseed-releases](https://github.com/caraka/daemonseed-releases) page, at which
point the Download buttons switch from "Builds coming soon" to the live release.

Built by `caraka`. AGPL-3.0-or-later.
