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
- Proof: three live projects. Real screenshots of DiceWars JS (`img/dicewars.webp`) and Connections Sorter (`img/connections-sorter.webp`), captured 2026-09-25 from the live sites. spec-to-ship is shown as a typeset work-instruction card listing its real steps from the repo README: spec → prd → issues → triage → AFK loop.
- Copy: approved by Ivan on 2026-09-25. Headline "I run support operations, and I build the automation myself." Bio as approved. Projects heading "A few things I've built". Button "Connect on LinkedIn".

## Constraints

- Plain static HTML/CSS on GitHub Pages. No build step. JS optional and never required for content.
- Must not feel corporate, dev-portfolio, cute, or showy (PRODUCT.md).
- Photo: `ivans-head.png` (200×200) is a stand-in. The slot is designed for a tight square headshot at ≥800×800, to be dropped in later.

## Direction contract

THESIS: Ivan's page is a lean-ops shadow board. Every project he built hangs in its own painted outline, so a peer sees at a glance what he makes. It refuses the centered avatar, bio, button and project-card stack the category always ships, and which the old page was.

OWN-WORLD: Drenched safety-yellow painted board (#F2C230). Paint-black silhouettes (#1C1C1A) sit a hand's width larger than each object. White label-maker tape carries black condensed caps. Anything painted on the board is stencil lettering (Big Shoulders Stencil); anything printed and mounted is Archivo. One red (#C8372D) marks the live element only. The dark scheme becomes two-layer tool foam: a black top layer with yellow showing through every pocket. No gradients, glass, icon tiles or floating shadowed cards.

STORY: A peer confirms the face and the name, reads in one line that Ivan runs support ops and builds the automation himself, and sees three working tools as the proof. Then they connect on LinkedIn or take a tool off the board.

FIRST VIEWPORT: Desktop 1440×900: "IVAN LAY" stenciled across the top left at display scale, with the owner photo hung in its own silhouette beside it and the two titles on label tape. Lower left: headline, bio, and the red LinkedIn plate. The right seven columns are the tool field: DiceWars (landscape), Connections Sorter (portrait) and the spec-to-ship card, each in its painted outline with a location tag (A1–A3) and action, all visible without scrolling. Mobile 390: name, photo, headline and the red plate in the first screen, with the tools hung one per row after.

FORM: 5S shadow board / two-layer tool foam, #1 of 7 on my grounded list (IMPECCABLE'S PICK). Seed key cc6eb0e4. Signature interaction, "the lift": hover or focus lifts a tool off its hook with a small swing, revealing its painted outline and the location code stenciled inside it. On load, tools settle into their outlines once. Reduced motion swaps both for a color change. Motion grammar: gravity only (hang, lift, settle), never slide or fade.

FINISH: unreviewed and undocumented is unfinished; this build ends with the finish review, the verdict, DESIGN.md, and every shipping raster carrying its provenance

## Unresolved

- Final headshot (Ivan sourcing). Replace `ivans-head.png` with a square crop ≥800×800.
