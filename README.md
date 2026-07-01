# vynull-site

The showcase / landing page for [Vynull](https://github.com/OWNER/vynull) — a
virtual Pioneer CDJ / rekordbox source for Linux.

It's a single static `index.html` (no build step, no framework, no external
dependencies) designed for **GitHub Pages**.

## Deploy on GitHub Pages

1. Push this repo to GitHub.
2. **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   branch `main`, folder `/ (root)`.
3. Your site goes live at `https://OWNER.github.io/vynull-site/` (or a custom
   domain — add a `CNAME` file with the domain and configure DNS).

## Before publishing

- **Replace every `OWNER`** placeholder in `index.html` with your GitHub
  username/org (the Source / Download / Releases links). Search for `OWNER`.
- **Add screenshots** to `assets/` (the page shows styled placeholders until
  they exist, then swaps them in automatically):
  - `assets/screenshot-webui.png` — the browser library manager
  - `assets/screenshot-cdj.png` — color waveforms on a real CDJ
  - `assets/screenshot-tui.png` — the terminal monitor

  A short **demo GIF/MP4** (waveforms rendering on a deck) is the highest-impact
  addition — drop it in and reference it in the "See it" section.

## License

GPLv3 — see [`LICENSE`](LICENSE), matching the Vynull project.
