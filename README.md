# vynull-site

The showcase / landing page for [Vynull](https://github.com/vynulldev/vynull) —
a virtual CDJ / rekordbox source for Linux. Lives at
**[vynull.dev](https://vynull.dev)**.

A single static `index.html` (no build step, no framework, no external
dependencies), served by **GitHub Pages**.

## Deploy

Publishing is automated by
[`.github/workflows/pages.yml`](.github/workflows/pages.yml): every push to
`main` uploads the repo root and deploys it to GitHub Pages.

One-time setup in the repo:

1. **Settings → Pages → Build and deployment → Source: GitHub Actions.**
2. **Settings → Pages → Custom domain: `vynull.dev`**, then add the matching
   DNS at your registrar:
   - apex `vynull.dev` → GitHub Pages A records
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
     (plus AAAA records for IPv6 if you want them), **or** a CNAME/ALIAS record
     pointing at `vynulldev.github.io`.
3. Tick **Enforce HTTPS** once the certificate issues.

## Assets

The screenshots in `assets/` are generated reproducibly — no personal library
and no hardware required — by the screenshot pipeline in the companion
`vynull-tools` repo (`screenshots/`). `index.html` falls back to a styled
placeholder for any asset that's missing.

A short **demo GIF/MP4** of waveforms rendering on a deck is the
highest-impact addition still open — drop it in `assets/` and reference it in
the "See it" section.

## License

GPLv3 — see [`LICENSE`](LICENSE), matching the Vynull project.
