# ivanlay.com

The source for [ivanlay.com](https://ivanlay.com), Ivan Lay's personal landing page. It is one HTML page and one stylesheet, served by GitHub Pages from `main`. There is no build step and no JavaScript.

The page is designed as a lean-ops shadow board cut from two-layer tool foam: each project hangs in its own pocket, where safety yellow shows through a black top layer. There is one scheme, dark, whatever the visitor's system setting. Two documents govern changes to it. `PRODUCT.md` says who the page is for, how it should sound, and what it may and may not claim. `DESIGN.md` records the visual system: colors, type, components and motion. Read both before changing the copy or the look.

## Preview locally

```bash
python3 -m http.server
```

Then open http://localhost:8000. Opening `index.html` directly in a browser also works.

## Replace the photo

Save a square headshot of at least 800×800 over `ivans-head.png`. The slot crops to a square, so a tight face-and-shoulders crop works best. If you use a different filename or format, update the `src` of the `plate--photo` image in `index.html` and set its `width` and `height` to the file's pixel size.

## Add or swap a project

Each project is an `<li class="tool">` in the `.rack` list in `index.html`. The layout is built for three to five projects. Screenshots live in `img/` as WebP, each with a `.webp.json` sidecar recording where it came from.

The first row pairs a 3:2 screenshot with a 24:35 one. The column split on `.rack` in `style.css` (the `0.68627` factor) keeps the two images the same height, so recompute it if either aspect ratio changes. A new project also needs its own area in the rack's `grid-template-areas`.

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
