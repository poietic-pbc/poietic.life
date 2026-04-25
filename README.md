# poietic.life

Landing page for [Poietic PBC](https://poietic.life), a public benefit
corporation building open-source infrastructure for hybrid human-AI science.

Served from this repository's `main` branch via
[GitHub Pages](https://docs.github.com/en/pages), reachable at
https://poietic.life (custom domain configured via `CNAME`).

## Files

- `index.html` — single-file landing page. JetBrains Mono + Instrument Serif
  from Google Fonts, inline SVG logo and favicon, no build step, no JS
  dependencies beyond a small inline script for the hero graph ticker.
- `CNAME` — tells GitHub Pages to serve from `poietic.life`.
- `LICENSE` — MIT.

## Editing

Edit `index.html` directly and push. GitHub Pages rebuilds within ~1 minute.
There is no build pipeline and there should not be one for this page. If the
page grows beyond a single file, first ask whether the complexity is worth
losing the zero-build property.

## DNS for the custom domain

At the `poietic.life` registrar, set four A records at the apex
(`poietic.life`) pointing to GitHub Pages:

- 185.199.108.153
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

For `www.poietic.life`, add a `CNAME` record pointing to `poietic.life`.

Then, in this repository's Settings → Pages, verify the custom domain is
recognized and enable "Enforce HTTPS" once GitHub has provisioned the cert.

## Related

- [poietic-pbc/deep-research-competition](https://github.com/poietic-pbc/deep-research-competition),
  the live drug-discovery competition.
- [graphwork/workgraph](https://github.com/graphwork/workgraph), the
  WorkGraph product.
