# Grydin Mart — marketing landing page

A light-theme, static marketing landing page for Grydin Mart. It is designed to be hosted as static files; it has no server or checkout integration.

## Preview

Run `run-site.cmd` or `node server.js`, then open `http://127.0.0.1:4173/`. The local server is needed because browsers block loading the GLB from a `file://` URL. The hero displays the supplied GLB as an interactive 3D model, using the reference artwork as its loading poster.

## Project files

- `index.html` — complete page, responsive styling and interactions.
- `assets/grydin-grocery-bag.glb` — 3D grocery bag model used in the “Why Grydin” section.
- `assets/grydin-grocery-bag-hero.glb` — updated 3D bag model used in the hero.
- `assets/grydin-hero-art.png` — cropped grocery artwork used in the hero.
- `assets/grydin-app-showcase.png` — app and fresh-produce showcase visual.
- `assets/grydin-app-demo.mp4` — optional H.264 app screen recording, layered into the phone screen when present.
- `server.js` and `run-site.cmd` — dependency-free local preview server and launcher.
- `logo/grydin-mart-mark.svg` — Grydin grocery-bag-and-sprout brand mark.
- `logo/grydin-mart-logo.svg` — full vector logo lockup.

## Brand direction

- Grydin green `#2C6E2F`
- Accent yellow `#FFB81C`
- Warm paper `#f8f8f2`
- Ink `#17251e`
- Poppins headings and Roboto Mono captions

The landing page presents Grydin mart's customer app, live tracking, order verification, substitutions, alerts, local payment methods, and rider program. The app showcase image remains visible as a fallback. To show a recorded demo in the angled phone screen, add an H.264 MP4 named `grydin-app-demo.mp4` in `assets/`; playback starts muted, inline, and looping when the showcase approaches the viewport. The 3D hero uses Google's `<model-viewer>` component from its official CDN and the provided GLB asset. The CDN script and Google Fonts require an internet connection; the model file is served locally. No delivery area, prices, customer statistics, customer quotes, contact details, store hours, or ordering destinations have been invented. Connect the app-store badges and rider CTA to their real destinations when those URLs are available.
