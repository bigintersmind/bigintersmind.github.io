# ivanlay.com

The source for [ivanlay.com](https://ivanlay.com), Ivan Lay's personal landing page. It is one HTML page and one stylesheet, served by GitHub Pages from `main`. There is no build step and no JavaScript.

The page is designed as one engineering drawing sheet printed as a cyanotype: a Prussian blue ground with every line, frame, rule and letter in white. A zoned border rings the sheet, the headline and bio sit top left as the drawing's notes, the three projects are numbered views on the right, and Ivan's photo, name and the LinkedIn button live in the title block at the bottom right, where the drafter's name goes. There is one scheme, whatever the visitor's system setting. Two documents govern changes to it. `PRODUCT.md` says who the page is for, how it should sound, and what it may and may not claim. `DESIGN.md` records the visual system: colors, type, components and motion. Read both before changing the copy or the look.

## Preview locally

```bash
python3 -m http.server
```

Then open http://localhost:8000. Opening `index.html` directly in a browser also works.

## Replace the photo

Save a square headshot of at least 800×800 over `ivans-head.png`. The title block crops it to a square, so a tight face-and-shoulders crop works best. The blue cyanotype tint is applied in CSS (`.portrait` in `style.css`), so any photo takes it. If you use a different filename or format, update the `src` of the `portrait` image in `index.html` and set its `width` and `height` to the file's pixel size.

## Add or swap a project

Each project is an `<li class="view">` in the `.view-grid` list in `index.html`: a framed screenshot (or, for a process rather than a screen, a table drawn in white rules) with a balloon number, name, one line and an exit. The layout is built for three to five projects. Screenshots live in `img/` as WebP, each with a `.webp.json` sidecar recording where it came from.

The desktop grid places the views by name in `grid-template-areas` on `.view-grid` in `style.css` (a landscape view and a portrait view share the first row; a wide view spans below). A new project needs its own area there and its own `view--name` class, and the balloon numbers continue the sequence. Keep the whole sheet within a 1440×900 viewport: the title block must stay in view.

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
.impeccable/     design records: direction brief, design tokens, review captures, decision sketches
_config.yml      keeps the project docs out of the published site
CNAME            custom domain
```
