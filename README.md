# Ian Bonaparte — Portfolio

Design Engineer portfolio. Single-page site, no build step.

## Structure

- `index.html` — the published site. Fully self-contained (styles, scripts and images inlined). This is what GitHub Pages serves.
- `Ian Bonaparte PS2.dc.html` — the working source file the export is generated from.
- `assets/` — original screenshots and logos used by the source file.
- `CLAUDE.md` — content library: all approved copy, case studies and asset notes.

## Publishing

`index.html` sits at the repo root, so GitHub Pages can serve it directly:

1. Settings → Pages
2. Source: **Deploy from a branch**
3. Branch: `main`, folder: `/ (root)`

The site is then live at `https://<username>.github.io/<repo>`.

## Custom domain

Add the domain under Settings → Pages → Custom domain, then create a `CNAME`
file at the repo root containing that domain on a single line. At the registrar:

- Apex domain (`example.com`) — four A records pointing to `185.199.108.153`,
  `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- Subdomain (`www.example.com`) — one CNAME record pointing to `<username>.github.io`

Leave "Enforce HTTPS" checked once the certificate is issued.

## Updating content

Edit the source file, not `index.html` — the export is regenerated from it.
