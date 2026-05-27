# Next Session Prompt

Paste this at the start of the next working session.

---

We are building CanadaSteps (canadasteps.org) — a plain-language guidance website for newcomers to Canada. Static HTML, no backend, editorial-first.

**Current phase:** Phase 0 — Foundation

**Session ended:** May 27, 2026

**PGWP page is complete. Do not edit further until second user feedback received.**

**sin.html v1 is built. Not yet deployed. Awaiting review before Netlify push.**

**Next task:** Navigation and homepage

Start by reading the official source:
https://www.canada.ca/en/employment-social-development/services/sin.html

**Deployment:** Netlify manual drag-and-drop of canadasteps folder
**Netlify URL:** hilarious-madeleine-0801d5.netlify.app
**Custom domain:** canadasteps.org/pgwp.html

**Key files:**
- `pgwp.html` — canonical live page (root, not pages/)
- `sin.html` — SIN guide v1, built, not yet deployed
- `index.html` — currently redirects to pgwp.html, will become homepage
- `memory/current_state.md` — current project state
- `daily.md` — C:\Projects\SG\CanadaSteps.ca\canadasteps\daily.md
- `docs/editorial-rulebook.md` — all editorial rules

**Rules to follow:**
- Read memory/next_prompt.md only at session start
- Never paraphrase fees — quote and link
- Never state processing times as a number — link to live tool
- Grade 8 reading level
- Disclaimer block on every page
- No features not in `requirements.md`

---

NEXT TASK — NAVIGATION AND HOMEPAGE

⚠️ Do not start this task with less than 50% credits.

Read only:
- pgwp.html
- sin.html
- index.html
- memory/current_state.md
- C:\Projects\SG\CanadaSteps.ca\canadasteps\daily.md

Then:

1. Add nav links to pgwp.html and sin.html
   — link between the two pages in the nav bar
   — same CSS variables, no redesign

2. Replace index.html with a simple guides homepage
   — two guide cards: PGWP and SIN, both live
   — same CSS variables, mobile-first
   — no new design patterns

Commit: "nav: add guide navigation and simple homepage"
Update memory/current_state.md and daily.md only.
