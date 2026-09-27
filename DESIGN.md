---
name: Ivan Lay
description: A lean-ops shadow board cut as two-layer tool foam. Every tool Ivan built hangs in its own cut pocket.
colors:
  safety-yellow: "#F2C230"
  paint-black: "#1C1C1A"
  laminate-white: "#FBFAF6"
  live-red: "#D23D31"
  live-ink: "#FFFFFF"
  foam-black: "#1B1C1A"
  foam-ink: "#ECE8DC"
  foam-ink-soft: "#C2BBA7"
typography:
  display:
    fontFamily: "'Big Shoulders Stencil', 'Arial Narrow', sans-serif"
    fontSize: "clamp(3.5rem, 1.6rem + 4.6vw, 6rem)"
    fontWeight: 800
    lineHeight: 0.86
    letterSpacing: "0.01em"
  headline:
    fontFamily: "'Archivo', system-ui, sans-serif"
    fontSize: "clamp(1.8rem, 1.05rem + 2vw, 2.75rem)"
    fontWeight: 800
    lineHeight: 1.04
    letterSpacing: "-0.012em"
    fontVariation: "'wdth' 87.5"
  title:
    fontFamily: "'Big Shoulders Stencil', 'Arial Narrow', sans-serif"
    fontSize: "clamp(1.5rem, 1.1rem + 1vw, 2rem)"
    fontWeight: 800
    lineHeight: 1
    letterSpacing: "0.02em"
  pocket-label:
    fontFamily: "'Big Shoulders Stencil', 'Arial Narrow', sans-serif"
    fontSize: "1.3rem"
    fontWeight: 800
    lineHeight: 1
    letterSpacing: "0.02em"
  location-code:
    fontFamily: "'Big Shoulders Stencil', 'Arial Narrow', sans-serif"
    fontSize: "1rem"
    fontWeight: 800
    lineHeight: 1
    letterSpacing: "0.08em"
  body:
    fontFamily: "'Archivo', system-ui, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.55
  body-small:
    fontFamily: "'Archivo', system-ui, sans-serif"
    fontSize: "0.9375rem"
    fontWeight: 400
    lineHeight: 1.45
  label:
    fontFamily: "'Archivo', system-ui, sans-serif"
    fontSize: "0.78rem"
    fontWeight: 650
    lineHeight: 1.2
    letterSpacing: "0.08em"
    fontVariation: "'wdth' 75"
  button:
    fontFamily: "'Archivo', system-ui, sans-serif"
    fontSize: "1.05rem"
    fontWeight: 750
    lineHeight: 1
    letterSpacing: "0.07em"
    fontVariation: "'wdth' 75"
rounded:
  tape: "1px"
  image: "2px"
  plate-sm: "4px"
  plate: "5px"
  pocket-sm: "11px"
  pocket: "16px"
spacing:
  plate-border: "6px"
  pocket-pad-sm: "16px"
  pocket-pad-md: "20px"
  pocket-pad: "24px"
  gutter: "clamp(1.25rem, 4vw, 3.5rem)"
  rack-gap: "clamp(1.25rem, 2.2vw, 2rem)"
components:
  pocket:
    backgroundColor: "{colors.safety-yellow}"
    textColor: "{colors.foam-black}"
    rounded: "{rounded.pocket}"
    padding: "24px 24px 12px"
  plate:
    backgroundColor: "{colors.laminate-white}"
    rounded: "{rounded.plate}"
    padding: "6px"
  tape:
    backgroundColor: "{colors.laminate-white}"
    textColor: "{colors.paint-black}"
    typography: "{typography.label}"
    rounded: "{rounded.tape}"
    padding: "0.34em 0.7em 0.3em"
  tape-action-hover:
    backgroundColor: "{colors.laminate-white}"
    textColor: "{colors.live-red}"
  pocket-cta:
    backgroundColor: "{colors.safety-yellow}"
    rounded: "{rounded.pocket-sm}"
    padding: "9px"
  plate-live:
    backgroundColor: "{colors.live-red}"
    textColor: "{colors.live-ink}"
    typography: "{typography.button}"
    rounded: "{rounded.plate-sm}"
    padding: "1rem 1.4rem 0.95rem"
  plate-card:
    backgroundColor: "{colors.laminate-white}"
    textColor: "{colors.paint-black}"
    rounded: "{rounded.plate}"
    padding: "0"
---

# Design System: Ivan Lay

## Overview

**Creative North Star: "The Shadow Board"**

The page is a lean-manufacturing 5S shadow board cut as two-layer tool foam: a black top layer where every object hangs from its own peg inside a pocket cut a hand's width larger than the object, with safety yellow showing through every cut. Nothing floats in space; everything has a cut home, and the home is visible the moment the object leaves it. The board says "this person keeps a tidy shop and makes real tools" without a single adjective.

Two material registers divide every surface. Anything **painted on the board** (the name, section headings, pocket labels, location codes, step numerals) is stencil lettering. Anything **printed and mounted** (headline, bio, label-maker tape, laminated plates, cards) is Archivo. The silhouettes are cut-outs, not painted outlines: the yellow under-layer is the pocket, and anything painted inside it is the black of the foam.

Motion obeys gravity only. Objects settle onto their hooks once on load, lift off with a small swing when hovered or focused, and fall back. Nothing slides, fades, or scrolls into view. The board rejects gradients, glass, icon tiles, and the centered avatar-bio-button-card stack.

**Key Characteristics:**
- A flat foam-black field with no gradient or texture.
- Safety-yellow cut pockets with generous 16px corners hold every object.
- Two type registers: stencil for paint, Archivo for print, never mixed within one object.
- White laminate and label tape are the only light surfaces on the board.
- One red, reserved for the live element and live states.
- Gravity-only motion: hang, settle, lift.

## Colors

The board is foam black. Safety yellow is the accent that marks every pocket and the lettering painted on the board, with white for anything printed and one reserved red.

### Primary
- **Safety Yellow** (`safety-yellow`): The pocket color, the yellow under-layer of the foam showing through every cut. Also the lettering painted on the board (the name and section headings). 10.2:1 against foam black.

### Secondary
- **Live Red** (`live-red`): The only red. Fills the LinkedIn plate, turns action tapes red on hover, draws the 3px focus ring, and fills a pocket under reduced motion. White on it is 4.7:1, and it holds 3.6:1 as a ring against the black foam.
- **Live Ink** (`live-ink`): White lettering on the red plate only.

### Neutral
- **Paint Black** (`paint-black`): Ink on laminated plates, the standard-work card, and label-maker tape only (16.3:1 on laminate white).
- **Laminate White** (`laminate-white`): Laminated plates, the standard-work card, and label-maker tape. It stays white on the black board; it is a printed object, not a surface that inverts.
- **Foam Black** (`foam-black`): The board, the top foam layer. Also the lettering inside yellow pockets (10.2:1 on the yellow).
- **Foam Ink** / **Foam Ink Soft** (`foam-ink`, `foam-ink-soft`): Body copy and secondary copy (tool descriptions) printed on the foam (14.0:1 and 8.9:1).

### Named Rules
**The One Red Rule.** Red marks the live element and live states only: the primary exit, hover on an action, focus. Never decoration, never a second accent, never a heading.

**The Paint-Through Rule.** Lettering inside a pocket is always the board color (`--on-pocket`): foam black on the yellow, never white or grey.

**The Laminate Never Inverts Rule.** Printed objects (plates, tape, cards) keep white stock and black ink, even on the black board. They never take the board's colors.

## Typography

**Display Font:** Big Shoulders Stencil 800 (with Arial Narrow, sans-serif)
**Body Font:** Archivo, variable width 75–100 and weight 400–800 (with system-ui, sans-serif)

**Character:** A condensed industrial stencil is the paint on the board. Archivo, squeezed with `font-stretch`, is the printing on labels and laminated sheets. The pairing reads as a shop floor, not a portfolio.

### Hierarchy
- **Display** (Stencil 800, `clamp(3.5rem, 1.6rem + 4.6vw, 6rem)`, 0.86, uppercase): The owner's name only, stacked one word per line.
- **Headline** (Archivo 800 at 87.5% width, `clamp(1.8rem, 1.05rem + 2vw, 2.75rem)`, 1.04, -0.012em, balanced): The single-sentence pitch. Max 15em (17em in single column).
- **Title** (Stencil 800, `clamp(1.5rem, 1.1rem + 1vw, 2rem)`, 1, uppercase): Section headings painted on the board.
- **Pocket Label** (Stencil 800, 1.3rem, uppercase): Tool names painted inside the silhouette below the plate, in a fixed 2rem strip so neighbouring pockets end on one line. Drops to 1.05rem in narrow pockets.
- **Location Code** (Stencil 800, 1rem, 0.08em): A1, A2, A3, painted on the pocket floor and breaking the slot outline.
- **Body** (Archivo 400, 1.0625rem / 1rem under 40rem, 1.55): Bio. Max 34em.
- **Body Small** (Archivo 400, 0.9375rem, 1.45): Tool descriptions. Max 34ch.
- **Label** (Archivo 650 at 75% width, 0.78rem, 0.08em, uppercase): Label-maker tape (titles, actions at 0.8rem).
- **Button** (Archivo 750 at 75% width, 1.05rem, 0.07em, uppercase): The live plate.

Step numerals on the standard-work card use Stencil 800 at 1.45rem: numbers painted onto the card.

### Named Rules
**The Paint or Print Rule.** Ask of every piece of text: is it painted on the board or printed and mounted? Painted is Big Shoulders Stencil 800, uppercase. Printed is Archivo. There is no third face and no stencil body copy.

**The Squeeze, Don't Swap Rule.** Condensed Archivo comes from `font-stretch` (75% for tape and plates, 87.5% for the headline), not from a separate condensed family.

## Layout

The board is a two-zone grid: owner and pitch on the left, the tool field on the right, split `5fr / 7fr` with a `clamp(2.5rem, 5.5vw, 6rem)` column gap. The board is capped at 90rem, uses a `clamp(1.25rem, 4vw, 3.5rem)` gutter, and is vertically centered in a full-viewport minimum height, so on a 1440×900 desktop the whole board is visible at once.

Under 68rem the board becomes a single 46rem column (pocket padding 20px). Under 40rem the rack becomes one tool per row, the standard-work card's steps stack as rows (numeral / verb / note), and pocket padding drops to 16px. Under 22rem the photo stacks above the name.

The rack is a grid of pockets. When two screenshots of different aspect ratios share a row, the column widths are calculated from the ratios (plus the fixed pocket and plate padding) so the images share one height and the pockets end on one line; a full-width card spans the row below. This calculation is specific to the current pair of screenshots and must be recomputed when a tool is swapped.

Spacing is fluid rather than stepped: vertical gaps are `clamp()` values tied to viewport height (for example `clamp(2rem, 5.5vh, 3.25rem)` above the headline), while object-level spacing is fixed in px (pocket padding, 6px plate border, 3px slot inset).

### Named Rules
**The Hand's Width Rule.** Every silhouette is the object plus a fixed painted margin (`pocket-pad`: 24px, 20px at ≤68rem, 16px at ≤40rem) on top and sides, with the label strip below. The margin also sizes the hook, which spans exactly from the pocket's top edge to the plate.

## Elevation & Depth

The board is flat paint. Depth exists only where a physical object hangs on it: laminated plates carry a hairline contact shadow at rest and a longer drop shadow only while lifted. Silhouettes, the board, and text never cast shadows. Label tape has a 1px contact shadow as a stuck-down sticker.

### Shadow Vocabulary
- **Rest** (`box-shadow: 0 1px 2px rgb(0 0 0 / 0.4)`): A plate hanging flush on its hook.
- **Lift** (`box-shadow: 0 12px 16px -12px rgb(0 0 0 / 0.7), 0 2px 4px rgb(0 0 0 / 0.3)`): A plate lifted 24px off its hook on hover or focus.
- **Tape** (`box-shadow: 0 1px 1px rgb(28 28 26 / 0.22)`): Label-maker tape stuck to the board.

### Named Rules
**The Gravity Rule.** Shadows answer to gravity: they appear only under a hung or stuck object and lengthen only when that object is lifted. No ambient glows, no floating cards at rest, no hard offset shadows.

## Shapes

Silhouettes are generously rounded (16px; 11px on the compact CTA pocket), like a routed foam cut or a painted outline around a tool. The objects inside are near-square: plates at 5px (4px for the photo and live plate), screenshots at 2px inside the plate, tape at 1px. The slot outline is a 2px painted stroke at 5px radius, inset 3px, matching the plate it holds. The hook is a 10px round peg head on a 3px stem. The focus ring follows the pocket's 16px curve.

**The Soft Cut, Hard Object Rule.** The cut or painted home is round; the object in it is almost square. Never round a plate to match its pocket.

## Components

### Pocket (signature)
The cut pocket that holds every object on the board.
- **Shape:** 16px radius, `pocket-pad` on top and sides, 12px under the label strip.
- **Color:** Safety yellow cut into the foam-black board, lettering in the board color (foam black).
- **Contents:** a slot, a plate, and a stenciled pocket label.
- **Reduced motion:** the pocket turns live red on hover or focus instead of the plate lifting.

### Slot, Hook, and Location Code
The plate's painted home. A 2px outline in the board color, inset 3px, with a stenciled location code (A1, A2, …) centered on its bottom edge, the outline breaking around it. The plate covers it at rest; it shows only when the plate lifts. The hook (peg head and stem) sits above the plate's top center, and the plate swings from `transform-origin: 50% 0`.

### Plate
A laminated print hanging in a slot.
- **Shape:** 5px radius, 6px white border around a 2px-radius image (the photo plate: 5px border, 4px radius, square crop).
- **Background:** Laminate white.
- **Shadow:** Rest at rest, Lift while lifted.
- **Hover / Focus:** `translateY(-24px)` plus a per-object swing (roughly ±0.7° to ±1.6°, alternating direction across neighbours), 0.5s `cubic-bezier(0.16, 1, 0.3, 1)`.
- **Load:** settles once from -16px with its swing, 0.75s, staggered 80ms per object after 150ms.

### Label-Maker Tape
White tape with black condensed caps (Label style), 1px radius, tape contact shadow, never wraps. Used for the owner's titles and for tool actions. Action tapes carry a 0.95em outbound-arrow SVG and turn their text live red on hover.

### Live Plate (primary action)
The only red object: a live-red plate with white Button text and an outbound arrow, hung in a compact yellow pocket (9px padding, 11px radius). It lifts and swings like any plate. One per board.

### Standard-Work Card
A laminated work-instruction sheet used for a tool that is a process rather than a screen. White stock, no padding, clipped. A condensed 0.75rem caps header ruled off by a 2px paint-black line, then numbered steps in equal columns separated by 1px warm-grey rules, each with a stencil numeral, a bold 87.5%-width verb, and a short note. Under 40rem the steps stack as rows.

## Do's and Don'ts

### Do:
- **Do** give every new object its own pocket, slot, hook, and location code, continuing the sequence (A4, A5…).
- **Do** decide paint or print before setting any text: Big Shoulders Stencil 800 uppercase if painted on the board, Archivo if printed.
- **Do** keep red to the one live plate, hover on actions, and the 3px focus ring (6px offset).
- **Do** keep laminated plates and tape white with black ink on the black board.
- **Do** keep all motion as gravity: settle, lift (-24px with swing), fall back; swap it for a red pocket under reduced motion.
- **Do** recompute the rack column split whenever a screenshot's aspect ratio changes, so paired plates share one height.

### Don't:
- **Don't** use gradients, glass, or textures on the board, or add any accent beyond the yellow and the one red.
- **Don't** put icons in tiles or badges. The only icon is a small inline outbound arrow on tape and the live plate.
- **Don't** float cards or add shadows to silhouettes, text, or the board. Only hung plates and stuck tape cast shadows.
- **Don't** slide, fade, or scroll-animate anything in.
- **Don't** set body copy, descriptions, or buttons in the stencil face, or set painted names and headings in Archivo.
- **Don't** fall back to the centered avatar, bio, button, and project-card stack.
