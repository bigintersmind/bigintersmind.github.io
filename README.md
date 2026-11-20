# ivanlay.com

The source for [ivanlay.com](https://ivanlay.com), Ivan Lay's personal landing page. It is one HTML page and one stylesheet, served by GitHub Pages from `main`. There is no build step and no JavaScript.

The homepage reads like a personal letter. The letterhead introduces Ivan and links to LinkedIn. Each project has a name, a short description, and a link. `PRODUCT.md` describes the audience and voice, and `DESIGN.md` records the visual system.

## Preview locally

```bash
python3 -m http.server
```

Then open http://localhost:8000. Opening `index.html` directly in a browser also works.

## Replace the photo

Save a square headshot of at least 800×800 over `ivans-head.png`. The letterhead crops the photo to a small portrait, so a tight face-and-shoulders crop works best. If you use a different filename or format, update the `src` of the `portrait` image in `index.html` and set its `width` and `height` to the file's pixel size.

## Add or swap a project

Add a list item to `.project-list` in `index.html`, following the structure of an existing project. Give its heading and action unique IDs and reference both with the link’s `aria-labelledby`.

## Deployment

GitHub Pages builds from the root of `main` and serves it at ivanlay.com, the domain set in `CNAME`. Merging to `main` publishes. `_config.yml` keeps `README.md`, `PRODUCT.md` and `DESIGN.md` off the public site.

## Files

```text
index.html       the page
style.css        all styles; color tokens at the top
favicon.svg
img/             project screenshots and their provenance sidecars
ivans-head.png   headshot (a stand-in until the new photo)
PRODUCT.md       audience, positioning, voice, and claims the page may make
DESIGN.md        the visual system
.impeccable/     design records: direction brief, design tokens, live-mode config
_config.yml      keeps the project docs out of the published site
CNAME            custom domain
```
