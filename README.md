# Grydin Mart — marketing landing page

A light-theme, static marketing landing page for Grydin Mart. It is designed to be hosted as static files; it has no server or checkout integration.

## Preview

Run `run-site.cmd` or `node server.js`, then open `http://127.0.0.1:4173/`. The local server is needed because browsers block loading the GLB from a `file://` URL. The hero and “Why Grydin” section display the supplied GLB as an interactive 3D model; the hero uses the reference artwork as its loading poster.

## Project files

- `index.html` — complete page, responsive styling and interactions.
- `assets/grydin-grocery-bag.glb` — provided 3D grocery bag model.
- `assets/grydin-hero-art.png` — cropped grocery artwork used in the hero.
- `server.js` and `run-site.cmd` — dependency-free local preview server and launcher.
- `logo/grydin-mart-mark.svg` — Grydin grocery-bag-and-sprout brand mark.
- `logo/grydin-mart-logo.svg` — full vector logo lockup.

## Brand direction

- Evergreen `#194d35` / `#246044`
- Warm paper `#f8f8f2`
- Fresh lime `#d5ed83`
- Citrus coral `#e76c42`
- Ink `#17251e`

The landing page uses brand-led, general marketing copy and an illustrative app preview. The 3D hero uses Google's `<model-viewer>` component from its official CDN and the provided 22.4 MB GLB asset. The CDN script requires an internet connection; the model file is served locally. No delivery area, prices, customer statistics, customer quotes, contact details, store hours, or ordering destinations have been invented. The current primary actions navigate within the page; connect them to the actual store/app destination when it is available.
