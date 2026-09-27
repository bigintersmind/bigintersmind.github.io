# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Ivan's professional network: peers, colleagues, and people who met Ivan at work or at an event. They usually arrive already knowing the name and want to match it to a face and a story: who Ivan is, what he does, and whether he's worth keeping in touch with.

Hiring-side visitors (recruiters, hiring managers) are not the primary audience. The page should not be tuned as a résumé. People who find Ivan through one of his projects are welcome, but the page isn't built around them.

## Product Purpose

ivanlay.com is Ivan Lay's personal landing page. It gives someone in his network one place to understand who he is and what he's good at.

A visit succeeds when the visitor does one or both of these:

- **Connects on LinkedIn.** LinkedIn is the one way to contact Ivan from the page.
- **Tries a project**: plays DiceWars JS, uses Connections Sorter, or installs spec-to-ship.

No direct contact channel (email, form) is wanted.

## Positioning

An ops leader who builds. Ivan runs operations and also ships the automation himself as real code, tools, and plugins, not just roadmaps. Many ops leaders talk about AI and automation. Ivan can point to working software he made. The projects are the proof, and the page should let them carry that claim instead of stating it in adjectives.

## Operating Context

- A single page. Every action leaves the site: LinkedIn, or a project on its own domain.
- Projects currently linked:
  - DiceWars JS: https://ivanlay.com/dicewarsjs/ (browser game, "Play")
  - Connections Sorter: https://connections-sorter.com/ (web tool, "Open")
  - spec-to-ship: https://github.com/bigintersmind/spec-to-ship (Claude Code plugin, "GitHub")
- Open: which channels visitors arrive from (LinkedIn profile, event intros, email signatures, project pages) hasn't been confirmed.

## Capabilities and Constraints

- Plain static HTML/CSS: no framework, no build step, no JavaScript today. Hosted on GitHub Pages from `main`, with the custom domain `ivanlay.com` set in `CNAME`. (Taken from the repository; not changed during init.)
- The projects list is a **curated handful**: about 3–5 entries, swapped occasionally. It doesn't need to scale to a long archive.
- Two exits only: LinkedIn and the projects. No contact form, email, newsletter, or résumé download.

## Brand Commitments

- Name: **Ivan Lay**. Domain: **ivanlay.com**. GitHub handle: **bigintersmind**. LinkedIn: https://www.linkedin.com/in/ivanlay/
- **Voice: conversational first person.** Ivan talks to a peer in plain language ("I run ops, and I build the tools my team uses"). The current bio's résumé register is out of step with this and should move to it. The projects heading ("A few things I've built") already matches.
- Professional titles in the current copy: "Operations Manager" and "AI & Automation Leader" (Ivan moved from support operations into AI and business operations in 2026). These are existing facts, not a mandated tagline.
- None of the current visuals (LinkedIn-style blue, Inter, centered card layout) have been made binding.
- **Must not feel:** corporate (a LinkedIn profile or a consultancy's About page), like a dev portfolio (terminal prompts, hacker dark mode, code as decoration), cute (playful enough that peers doubt the ops leadership), or showy (motion or scroll effects that get between the visitor and the content).

## Evidence on Hand

- `ivans-head.png`: the current photo. 200×200px, cropped from an event photo with backdrop text partly visible. It's a stand-in: Ivan is finding a higher-quality **tight headshot** (face and shoulders) to drop in, so design for that rather than for the 200px file.
- Three live projects with one-line descriptions (see Operating Context).
- Existing claims, kept general: "12+ years" in support operations; AI and automation enablement; mentoring teams; process optimization that delivered "measurable capacity gains".
- **Must not be added or fabricated:** employer names, specific metrics or numbers, testimonials, endorsements, logos, press. Ivan chose to keep these general. Add them only if he supplies them later.

## Product Principles

1. **Show, don't claim.** The "ops leader who builds" position rests on working projects, not adjectives. When copy and proof compete for space, the proof wins.
2. **Talk like a peer.** Conversational first person throughout. The page reads like Ivan introducing himself, not like a résumé summary.
3. **Two exits, both first-class.** Connecting on LinkedIn and trying a project are equally valid outcomes. Neither should read as an afterthought.
4. **Curated over complete.** A few projects that each earn their place beat a longer list.
5. **Nothing invented.** Every claim traces to something Ivan provided or to a real, linked project.
