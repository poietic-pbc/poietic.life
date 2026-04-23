# poietic.life

Landing page for [Poietic PBC](https://poietic.life), a public benefit
corporation building open-source infrastructure for hybrid human-AI science.

This is a [GitHub Pages org site](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages#types-of-github-pages-sites),
served from this repository's `main` branch:

- Default URL: https://poietic-pbc.github.io/
- Custom domain: https://poietic.life (configured via `CNAME`)

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

At the `poietic.life` registrar, set:

- `ALIAS` or `ANAME` at the apex (`poietic.life`) pointing to
  `poietic-pbc.github.io`. If the registrar does not support ALIAS/ANAME,
  use four A records to GitHub Pages IPs:
    - 185.199.108.153
    - 185.199.109.153
    - 185.199.110.153
    - 185.199.111.153
- `CNAME` for `www.poietic.life` pointing to `poietic-pbc.github.io`.

Then, in this repository's Settings → Pages, verify the custom domain is
recognized and enable "Enforce HTTPS" once GitHub has provisioned the cert.

## Related

- [poietic-pbc/deep-research-competition](https://github.com/poietic-pbc/deep-research-competition),
  the live drug-discovery competition.
- [graphwork/workgraph](https://github.com/graphwork/workgraph), the
  WorkGraph product.
