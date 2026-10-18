---
name: Ivan Lay
description: An engineering drawing sheet printed as a cyanotype. Prussian blue ground, every line and letter in white, Ivan's name in the title block.
colors:
  prussian-blue: "#163F96"
  line-white: "#FFFFFF"
  hairline: "rgb(255 255 255 / 0.55)"
  ink: "#F5F8FF"
  ink-soft: "#C7D5F5"
  on-white: "#163F96"
  white-hover: "#E2EAFF"
typography:
  display:
    fontFamily: "'Barlow Semi Condensed', 'Barlow', system-ui, sans-serif"
    fontSize: "clamp(2.1rem, 1.3rem + 1.9vw, 2.6rem)"
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: "-0.01em"
  headline:
    fontFamily: "'Barlow', system-ui, sans-serif"
    fontSize: "clamp(1.85rem, 1.05rem + 1.9vw, 2.5rem)"
    fontWeight: 600
    lineHeight: 1.15
    letterSpacing: "-0.015em"
  title:
    fontFamily: "'Barlow', system-ui, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 600
    lineHeight: 1.3
  body:
    fontFamily: "'Barlow', system-ui, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.55
  body-small:
    fontFamily: "'Barlow', system-ui, sans-serif"
    fontSize: "0.875rem"
    fontWeight: 400
    lineHeight: 1.4
  body-table:
    fontFamily: "'Barlow', system-ui, sans-serif"
    fontSize: "0.8125rem"
    fontWeight: 400
    lineHeight: 1.3
  button:
    fontFamily: "'Barlow', system-ui, sans-serif"
    fontSize: "0.9375rem"
    fontWeight: 600
    lineHeight: 1
  heading-rule:
    fontFamily: "'Barlow Semi Condensed', 'Barlow', system-ui, sans-serif"
    fontSize: "0.6875rem"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "0.16em"
  label:
    fontFamily: "'Barlow Semi Condensed', 'Barlow', system-ui, sans-serif"
    fontSize: "0.6875rem"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "0.14em"
  caps:
    fontFamily: "'Barlow Semi Condensed', 'Barlow', system-ui, sans-serif"
    fontSize: "0.8125rem"
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: "0.08em"
  exit:
    fontFamily: "'Barlow Semi Condensed', 'Barlow', system-ui, sans-serif"
    fontSize: "0.75rem"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "0.12em"
  balloon:
    fontFamily: "'Barlow Semi Condensed', 'Barlow', system-ui, sans-serif"
    fontSize: "0.75rem"
    fontWeight: 700
    lineHeight: 1
  numeral:
    fontFamily: "'Barlow Semi Condensed', 'Barlow', system-ui, sans-serif"
    fontSize: "1.3rem"
    fontWeight: 700
    lineHeight: 1
  numeral-note:
    fontFamily: "'Barlow Semi Condensed', 'Barlow', system-ui, sans-serif"
    fontSize: "0.95rem"
    fontWeight: 700
  zone:
    fontFamily: "'Barlow Semi Condensed', 'Barlow', system-ui, sans-serif"
    fontSize: "0.5625rem"
    fontWeight: 600
    lineHeight: 1
rounded:
  balloon: "50%"
spacing:
  margin: "clamp(10px, 1.4vw, 20px)"
  ring: "18px"
  pad: "clamp(18px, 2vw, 28px)"
  gap: "clamp(1.75rem, 4vw, 3.5rem)"
  row-gap: "clamp(1.25rem, 2.5vh, 1.75rem)"
  frame-inset: "5px"
  cell-pad: "1.35rem 0.85rem 0.6rem"
  note-gap: "0.75rem"
  caption-gap: "0.7rem"
components:
  button-primary:
    backgroundColor: "{colors.line-white}"
    textColor: "{colors.on-white}"
    typography: "{typography.button}"
    padding: "0 1rem"
    height: "2.875rem"
    width: "100%"
  button-primary-hover:
    backgroundColor: "{colors.white-hover}"
  view-frame:
    padding: "{spacing.frame-inset}"
  balloon:
    textColor: "{colors.line-white}"
    typography: "{typography.balloon}"
    rounded: "{rounded.balloon}"
    size: "1.5rem"
  balloon-inspected:
    backgroundColor: "{colors.line-white}"
    textColor: "{colors.on-white}"
  exit:
    textColor: "{colors.ink}"
    typography: "{typography.exit}"
    padding: "0.25rem 0 0"
  cell-label:
    textColor: "{colors.ink-soft}"
    typography: "{typography.label}"
  heading-rule:
    textColor: "{colors.ink}"
    typography: "{typography.heading-rule}"
    padding: "0 0 0.4rem"
  table-head:
    textColor: "{colors.ink}"
    typography: "{typography.heading-rule}"
    padding: "0.5rem 0.75rem 0.4rem"
  zone-glyph:
    textColor: "{colors.ink-soft}"
    typography: "{typography.zone}"
---

# Design System: Ivan Lay

## Overview

**Creative North Star: "The Cyanotype Sheet"**

The page is one engineering drawing sheet, printed as a cyanotype. The Prussian blue runs edge to edge; everything drawn on it (the outer and inner borders, the zone strip, the view frames, the table rules, the title-block cells, every letter) is white line work, as if the sheet had been exposed from a single negative. There is no second colour on the sheet itself. Depth is never implied; the sheet is flat paper and the only things that sit "on" it are the pieces of evidence pinned into their frames.

Two kinds of lettering divide the sheet. Anything a drafter would letter by hand (the name in the title block, cell labels, zone glyphs, balloon numbers, exit labels, the ruled section heads, the table head, the note and step numerals) is Barlow Semi Condensed in capitals. Anything read as prose (the headline, the notes, view names and their one-liners, the table body, the button) is Barlow in sentence case. The condensed caps carry the drawing-sheet idiom; the prose face keeps it readable at a peer's pace.

Evidence keeps its own colour. Screenshots sit in their white frames at full colour, the only non-blue, non-white material on the page. The portrait is the one exception: it takes the cyanotype process (greyscale, screened onto the blue cell) so the drafter's face belongs to the sheet rather than being pinned to it. Motion is a single develop on load; nothing slides, scrolls in, or fades by section. The sheet refuses the centred avatar, bio, button and project-card stack, and it refuses the previous yellow-and-black shop floor entirely.

**Key Characteristics:**
- A single Prussian blue ground with no gradient, texture, or tonal layering.
- Every structural element is a white line: 1.5px outer border, 1px everything else, 55% white for secondary rules.
- One solid white cell on the whole sheet: the Connect on LinkedIn button.
- Two faces: Barlow Semi Condensed caps for drafting lettering, Barlow for prose.
- True-colour evidence in white frames; the portrait alone takes the blue process.
- Zoned border (1 to 8 across, A to D down) and a title block flush with the inner border.
- One authored motion, the develop; one signature interaction, the inspection.

## Colors

A monochrome cyanotype: one blue, white at three strengths, and two near-white inks tinted toward the blue.

### Primary
- **Prussian Blue** (`prussian-blue`): The ground of the sheet, applied to `html` and `body` and to the portrait cell behind the screened photo. It is also the `theme-color` and the favicon tile. It is never used as an accent; it is the paper.
- **Line White** (`line-white`): Every drawn line, frame, rule, and the name in the title block. It is the fill of the one white cell and of an inspected balloon, the colour of the selection highlight and the focus ring, and the caret.

### Neutral
- **Hairline** (`hairline`): White at 55%, for secondary rules only: the dividers between table steps and the scrollbar thumb. It is never used for text.
- **Ink** (`ink`): Prose white, tinted faintly toward the blue, for the headline, notes, view names, ruled section heads, the table head, and bold terms in the table.
- **Ink Soft** (`ink-soft`): Secondary prose and lettering: cell labels, zone glyphs, the sheet number, view one-liners, and table body text. It sits at roughly 6.5:1 on the blue, so it is legible as body copy, not only as decoration.
- **On White** (`on-white`): The blue returns as lettering wherever white is the fill: the button, the inspected balloon, and selected text. It is the same value as the ground, defined as its own token so that the inversion is explicit.
- **White Hover** (`white-hover`): The one white cell shifts to this slightly blued white on hover. It is the only hover fill on the sheet.

### Named Rules
**The Blue or White Rule.** Every element the page draws is either the blue or a white. There is no accent, no second hue, no grey that is not a transparency of white. If a new surface needs emphasis, it gets more line, not more colour.

**The One White Cell Rule.** The sheet carries exactly one solid white fill at rest: the primary exit (Connect on LinkedIn). A second filled cell would make it a form, not a drawing. Balloons may fill white only while inspected.

**The Evidence Keeps Its Colour Rule.** Screenshots in view frames are shown in their own colour, untreated. The portrait alone takes the cyanotype process (greyscale, screen blend onto the blue). Never tint evidence blue and never show the portrait in colour.

## Typography

**Display Font:** Barlow Semi Condensed, weights 600 and 700 (with Barlow, system-ui, sans-serif)
**Body Font:** Barlow, weights 400 and 600 (with system-ui, sans-serif)

Both families are self-hosted as four woff2 files under `fonts/` (OFL), preloaded, and declared with `font-display: block` so nothing swaps during the develop.

**Character:** A drafter's two hands. The Semi Condensed capitals are the lettering of a title block: tight, tracked, authoritative, never used for a sentence. Barlow at 400 and 600 is the prose a peer reads at a glance: warm, plain, slightly squared. Nothing on the sheet is set in a third face, and no system display face appears.

### Hierarchy
- **Display** (Semi Condensed 700, clamp(2.1rem, 1.3rem + 1.9vw, 2.6rem), 0.95, -0.01em, uppercase): The owner's name in the DRAWN BY cell only. Drops to 1.9rem at or below 24rem.
- **Headline** (Barlow 600, clamp(1.85rem, 1.05rem + 1.9vw, 2.5rem), 1.15, -0.015em): The one-sentence pitch at the top of the brief, balanced, max 15em (17em in the single column).
- **Title** (Barlow 600, 1.0625rem, 1.3): View names in captions.
- **Body** (Barlow 400, 1rem, 1.55): The notes; max 58ch, pretty-wrapped.
- **Body Small** (Barlow 400, 0.875rem, 1.4, ink-soft): View one-liners, max 32ch.
- **Body Table** (Barlow 400, 0.8125rem, 1.3, ink-soft): Table step text; the bold term in each step is Barlow 600 at 0.9375rem in ink. 0.75rem on short desktops.
- **Button** (Barlow 600, 0.9375rem, 1): The one white cell.
- **Heading Rule** (Semi Condensed 600, 0.6875rem, 0.16em, uppercase): Section heads (NOTES, A FEW THINGS I'VE BUILT) sitting on a 1px white rule, and the table head (STANDARD WORK).
- **Label** (Semi Condensed 600, 0.6875rem, 0.14em, uppercase, ink-soft): The field label in the top-left corner of every title-block cell (DRAWN BY, CONTACT, ROLES, SHEET).
- **Caps** (Semi Condensed 600, 0.8125rem, 1.2, 0.08em, uppercase): Roles and the sheet number in the title block.
- **Exit** (Semi Condensed 700, 0.75rem, 0.12em, uppercase): The action word on each view (PLAY, OPEN, GITHUB) with the outbound arrow.
- **Balloon** (Semi Condensed 700, 0.75rem, 1): The number inside a view balloon.
- **Numeral** (Semi Condensed 700, 1.3rem, 1): Step numbers in the table (1.1rem on short desktops and stacked rows). Note numerals use the same face at 0.95rem.
- **Zone** (Semi Condensed 600, 0.5625rem, 1, ink-soft): The border glyphs 1 to 8 and A to D, aria-hidden; 0.5rem at or below 68rem.

### Named Rules
**The Lettered or Read Rule.** Ask of every string: would a drafter letter it on the sheet, or is it read as prose? Lettered is Barlow Semi Condensed, uppercase, tracked. Read is Barlow, sentence case. No Semi Condensed sentence, no Barlow label.

**The Numeral Rule.** Every number that indexes something on the sheet (notes, balloons, table steps, zone glyphs) is Semi Condensed 700 or 600. Numbers inside prose stay in Barlow.

## Layout

The page is one sheet with a 1.5px white outer border, inset from the viewport by `margin` (clamp(10px, 1.4vw, 20px); 10px on short desktops). It fills the viewport height (100svh minus twice the margin) so that at 1440x900 the whole drawing is visible and the title block sits in the bottom-right corner.

Inside the outer border runs the zone strip, `ring` wide (18px; 14px at or below 68rem and on short desktops), carrying eight numbered columns across the top and bottom and four lettered rows down the left and right, each zone separated by a 1px white tick. Inside the strip is the 1px inner border of the field, padded by `pad` (clamp(18px, 2vw, 28px); 16px on short desktops).

The field is a two-column grid, 5fr brief to 7fr views, with `gap` between (clamp(1.75rem, 4vw, 3.5rem)) and `row-gap` between the views and the title block (clamp(1.25rem, 2.5vh, 1.75rem); 1rem on short desktops). The views column is itself a grid of 1.45fr to 1fr (1.3fr on short desktops): the landscape view and the table stack on the left, the portrait view runs the full height on the right.

The title block sits at the bottom right of the field, pulled out by negative margins so its top and left rules meet the inner border exactly. It is a fixed grid of four columns (6.5rem portrait, 10.5rem, 1fr, 13.75rem contact) and two rows (6.5rem and 3.25rem), capped at 37.5rem wide; short desktops shrink the first two columns and rows (5.75rem, 9rem; 5.75rem, 3rem).

Breakpoints, in the order they take effect going down:
- **Short desktop** (min-width 68.0625rem and max-height 860px): margins, ring, pad, row gaps, caption gaps and table padding tighten so the title block stays in view at 1280x800.
- **Single column** (max-width 68rem): the field becomes one column in the order title block, brief, views. The title block moves to the top strip, stretched to the inner border, as a two-column grid (6rem portrait, 1fr) with roles and contact on their own rows beneath; the SHEET cell is dropped. Brief capped at 40rem.
- **Stacked views** (max-width 40rem): views stack in order 1, 2, 3; the portrait view frame is capped at 15rem; the table turns from five columns into five rows, each a baseline-aligned grid of numeral, term, and text, divided by hairlines.
- **Small title block** (max-width 24rem): portrait cell 5rem, name 1.9rem.

Spacing is rem-based with a few fixed pixel values where the drawing needs them: the 5px frame inset around evidence, the 1px and 1.5px line weights, and the 18px ring.

## Elevation & Depth

The sheet is flat. There are no shadows, no gradients, no glass, and no tonal layering; the ground is one blue everywhere and every container is a drawn outline on it. Hierarchy comes from line weight (1.5px outer border, 1px everything else, 55% white for the least important rules) and from fill: the single white cell and the inspected balloon are the only places where figure and ground invert. Evidence in frames reads as "on" the sheet only because it carries its own colour.

### Named Rules
**The No Shadow Rule.** Nothing on the sheet casts a shadow, at rest or in any state. Hover and focus change fill and underline, never elevation.

## Shapes

Everything is rectilinear with square corners. Frames, cells, the button, the table, and the focus ring are all sharp-cornered rectangles drawn in 1px white (1.5px for the outer border). The single curve on the sheet is the balloon: a 1.5rem circle (`rounded.balloon`, 50%) holding a view number, exactly as a drawing balloon is drawn. The favicon rounds its 32px tile by 4px for the browser chrome; that radius belongs to the icon, not the sheet.

Borders are selective within compound forms: title-block cells draw a right and bottom rule each, with the outer edges removed where the block meets the inner border, so no rule is ever doubled. Table steps divide with hairlines, not full lines, so the table reads as one object.

## Components

### Buttons
The one solid white cell: a plain rectangle of line white with the blue returning as lettering, the outbound arrow at the far right.
- **Shape:** Square corners, no border, fills its cell (100% wide, 2.875rem tall, 0 1rem padding).
- **Primary:** `button-primary`: line white fill, on-white text, Barlow 600 at 0.9375rem, text and icon spread with space-between and a 0.75rem gap. Lives in the CONTACT cell of the title block.
- **Hover / Focus:** Background shifts to white-hover over 0.2s with the ease-out curve. Focus is the shared link ring: 2px solid line white, 4px offset.
- **Secondary / Ghost:** None. There is one button on the sheet. Secondary actions are exits (below).

### View Frame
A piece of evidence pinned to the sheet: a 1px white frame with a 5px inset holding a true-colour screenshot at full width.
- **Corner Style:** Square.
- **Background:** None; the inset shows the blue.
- **Shadow Strategy:** None (see Elevation & Depth).
- **Border:** 1px line white.
- **Internal Padding:** 5px (`frame-inset`). The table variant removes the padding so its own rules meet the frame.

### View Caption and the Inspection
Each view is a single link wrapping its frame and caption. The caption is a three-column grid (1.5rem balloon, text, exit) with a 0.6rem column gap, 0.7rem below the frame. The balloon is a 1.5rem outlined circle with the view number in Semi Condensed 700; the name is Title, the one-liner is Body Small in ink-soft; the exit is Semi Condensed 700 caps with the outbound arrow and a transparent 1px underline. The portrait view moves its exit under the text (two-column caption) because its column is narrow; it returns beside the text when views stack.
- **The inspection (hover / focus-visible on the link):** the balloon fills line white with on-white text and the exit's underline turns line white, both over 0.2s with the ease-out curve. Nothing moves or scales.

### Standard-Work Table
The spec-to-ship process drawn as a table inside a view frame. A table head in Heading Rule caps (0.5rem 0.75rem 0.4rem padding) sits on a 1px line; beneath it five equal columns, each a step with a Semi Condensed 700 numeral at 1.3rem in line white, a bold Barlow term at 0.9375rem in ink, and a Body Table line in ink-soft, divided by hairlines. At 40rem and below the five columns become five hairline-divided rows with numeral, term and text on one baseline.

### Title Block
The drafter's title block, flush with the inner border at the bottom right (top strip on narrow sheets). Every cell carries a field label (Label style, ink-soft, 0.45rem from the top, 0.8rem from the left) and bottom-aligns its content under 1.35rem 0.85rem 0.6rem padding. Cells: portrait; DRAWN BY with the name at Display size; CONTACT with the button; ROLES as Caps separated by 1.5rem; SHEET with the domain and sheet count in ink-soft.
- **Portrait:** Fills its cell with the blue behind it, object-fit cover, `filter: grayscale(1) contrast(1.18) brightness(0.94)` and `mix-blend-mode: screen` so nothing prints darker than the blue and highlights stay paper white. The cell isolates its blending. A `--portrait-zoom` token (currently 1.4, origin 60% 45%) crops the stand-in photo's backdrop; it is provisional and returns to 1 when the tight headshot lands.

### Ruled Section Heading
An h2 in Heading Rule caps sitting on a 1px line-white rule with 0.4rem beneath the text, followed by its content 0.9rem to 1rem below. Used for NOTES and A FEW THINGS I'VE BUILT; the table head is the same lettering inside a frame.

### Numbered Notes
The bio as drawing notes: an ordered list with CSS counters, each note a two-column grid (1.6rem numeral gutter, text) with a 0.35rem gap and 0.75rem between notes. Numerals are Semi Condensed 700 at 0.95rem, nudged 0.12em down to sit on the Body baseline.

### Zone Strip
The border glyphs. Four absolutely positioned grids in the 18px ring: eight cells across the top and bottom, four down each side, each cell a centred Zone glyph in ink-soft, divided by 1px line-white ticks. Aria-hidden and unselectable; it is part of the sheet, not content.

### Icon
The only icon on the sheet is a 16-unit outbound arrow drawn as an inline SVG symbol (`#icon-out`: a diagonal stroke with a square-capped corner, 1.8 stroke width, currentColor), sized at 0.9em next to the button text and every exit. No other glyphs, icon tiles, or badges appear.

### Motion: the Develop
The sheet's one authored moment. On load, under `prefers-reduced-motion: no-preference`, `.sheet` animates from 40% opacity to full in 0.9s with `cubic-bezier(0.16, 1, 0.3, 1)`, as a cyanotype develops. State transitions (button fill, balloon fill, exit underline) use the same curve over 0.2s. Nothing else animates; reduced motion skips the develop and keeps the transitions.

### Focus
Every link: `outline: 2px solid` line white, `outline-offset: 4px`, square. Selection inverts to line white with on-white text.

## Do's and Don'ts

### Do:
- **Do** draw every new container as a 1px line-white outline on the blue (1.5px only for the sheet's outer border); use hairline (55% white) for rules that subdivide an object.
- **Do** decide lettered or read before setting any text: Barlow Semi Condensed uppercase and tracked if a drafter would letter it, Barlow sentence case if it is read.
- **Do** keep evidence in true colour inside a 5px-inset white frame, and give every view a balloon number, a name, one line, and an exit word with the outbound arrow.
- **Do** give every title-block cell a field label in the top-left corner, and keep the block flush with the inner border.
- **Do** keep all motion to the develop on load and 0.2s fill or underline transitions with cubic-bezier(0.16, 1, 0.3, 1).
- **Do** keep the focus ring 2px line white at 4px offset, square.

### Don't:
- **Don't** add a second colour, a gradient, glass, texture, or any grey that is not a transparency of white.
- **Don't** add a second solid white fill at rest; the Connect on LinkedIn cell is the only one.
- **Don't** cast shadows on anything, or lift, scale, or slide anything on hover.
- **Don't** round corners; the balloon circle is the only curve.
- **Don't** tint screenshots blue, or show the portrait in colour.
- **Don't** set a sentence in Barlow Semi Condensed, set a label in Barlow, or introduce a third face or a system display face.
- **Don't** fade or slide sections in on scroll, or stagger anything; the sheet develops once, whole.
- **Don't** fall back to the centred avatar, bio, button, and project-card stack.
