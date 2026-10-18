---
version: 1
slug: "index-html"
primary_target: "index.html"
related_targets: []
---

# Landing page (index.html)

## Scope and mode

The whole of ivanlay.com: one page. Visitor mode: **Persuade**. A peer decides to connect with Ivan or try one of his projects.

## Audience, job, action, proof

- Audience: Ivan's professional network. They arrive knowing the name and want the face and story (PRODUCT.md).
- Action: connect on LinkedIn, or open a project. Both are first-class.
- Proof: three live projects. Real screenshots from the live sites: DiceWars JS (`img/dicewars.webp`, captured 2026-09-25) and Connections Sorter (`img/connections-sorter.webp`, retaken 2026-09-26 with two rows sorted). spec-to-ship is drawn as a table on the sheet listing its real steps from the repo README: spec → prd → issues → triage → AFK loop.
- Copy: approved by Ivan on 2026-09-25. Headline "I run operations, and I build the automation myself." (changed from "support operations" on 2026-09-26, when the title became Operations Manager) Bio as approved. Projects heading "A few things I've built". Button "Connect on LinkedIn".

## Constraints

- Plain static HTML/CSS on GitHub Pages. No build step. JS optional and never required for content.
- Must not feel corporate, dev-portfolio, cute, or showy (PRODUCT.md).
- Photo: `ivans-head.png` (200×200) is a stand-in. The slot is designed for a tight square headshot at ≥800×800, to be dropped in later.
- Brief for the 2026-10-18 redesign: "more professional and minimalist". Ivan chose the drawing sheet from the second hand and asked for it "more like a blueprint": the cyanotype is pinned.

## Direction contract

THESIS: Ivan's page is one engineering drawing sheet, printed as a cyanotype: the document builders actually work from, with Ivan's name in the title block where the drafter's goes. It refuses the centred avatar, bio, button and project-card stack, and it refuses the previous board's yellow-and-black shop floor.

OWN-WORLD: Prussian blue ground (#163F96) edge to edge; every line, rule, frame and letter is white, hairlines at 55% white. A zoned border (1–8 across, A–D down) rings the field. Views are 1px white frames holding true-colour screenshots; the spec-to-ship process is a table drawn in white rules. The portrait is a cyanotype (grayscale, screened onto the blue, so nothing prints darker than the sheet); the evidence keeps its own colour. One solid white cell on the whole sheet: the Connect on LinkedIn button. Type is Barlow, with Barlow Semi Condensed caps for drafting lettering (title, labels, exits, balloons). No gradients, no glass, no shadows, no second colour.

STORY: A peer reads the headline in one line, the bio as numbered notes, sees three working tools as numbered views, finds Ivan's face and name in the title block, and connects on LinkedIn or opens a view.

FIRST VIEWPORT: Desktop 1440×900: the whole sheet visible. Left five columns: headline at display size, then NOTES with the bio as notes 1 and 2. Right seven columns: view 1 DiceWars (3:2), view 2 Connections Sorter (portrait) beside it, view 3 the spec-to-ship table below, each captioned with a balloon number, name, one line and its exit (Play, Open, GitHub). Bottom right: the title block with the cyanotype portrait, IVAN LAY, the white Connect on LinkedIn cell, and a roles row. Mobile 390: the sheet turns portrait; the title block moves to the top strip so face and name lead, then the headline, notes and views stacked.

FORM: Engineering drawing sheet with zoned border and title block, #1 of 7 on my second-round grounded list (IMPECCABLE'S PICK), rendered as a cyanotype at Ivan's request. seed: d1eb231f3c89a910 (re-roll round 1). Signature interaction, "the inspection": hover or focus on a view fills its balloon white and underlines its exit, the inspector's mark on the drawing. Motion grammar: one authored moment, "the develop": on load the line work and lettering come up from 40% to full white in under a second, as a cyanotype develops; nothing slides, nothing scrolls in; reduced motion skips it.

FINISH: unreviewed and undocumented is unfinished; this build ends with the finish review, the verdict, DESIGN.md, and every shipping raster carrying its provenance

## Unresolved

- Final headshot (Ivan sourcing). Replace `ivans-head.png` with a square crop ≥800×800; the cyanotype treatment is CSS and carries over.
