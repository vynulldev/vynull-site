# vynull-site

The showcase / landing page for [Vynull](https://github.com/vynulldev/vynull) —
a virtual Pioneer CDJ / rekordbox source for Linux. Lives at
**[vynull.dev](https://vynull.dev)**.

A single static `index.html` (no build step, no framework, no external
dependencies), served by **GitHub Pages**.

## Deploy on GitHub Pages

1. Push this repo to GitHub.
2. **Settings → Pages → Source: Deploy from a branch**, branch `main`, folder
   `/ (root)`.
3. **Custom domain** — the `CNAME` file already points at `vynull.dev`. Add the
   matching DNS at your registrar:
   - apex `vynull.dev` → GitHub Pages A records
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
     (and AAAA records for IPv6 if you want them), **or** a CNAME/ALIAS to
     `vynulldev.github.io`.
   Then tick **Enforce HTTPS** once the certificate issues.

## Before publishing

Add screenshots to `assets/` (the page shows styled placeholders until they
exist, then swaps them in automatically):

- `assets/screenshot-webui.png` — the browser library manager
- `assets/screenshot-cdj.png` — color waveforms on a real CDJ
- `assets/screenshot-tui.png` — the terminal monitor

A short **demo GIF/MP4** of waveforms rendering on a deck is the highest-impact
addition — drop it in and reference it in the "See it" section.

## License

GPLv3 — see [`LICENSE`](LICENSE), matching the Vynull project.
