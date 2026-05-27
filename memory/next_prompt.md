# Next Session Prompt

Paste this at the start of the next working session.

---

We are building CanadaSteps (canadasteps.org) — a plain-language guidance website for newcomers to Canada. Static HTML, no backend, editorial-first.

**Current phase:** Phase 0 — Foundation

**Session ended:** May 27, 2026

**Latest handoff:** Shared agent memory workflow added to CLAUDE.md and AGENTS.md. No HTML or CSS changed.

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

NEXT TASK — NETLIFY DEPLOYMENT

Deploy all three pages to Netlify via manual drag-and-drop.

Steps:
1. Open Netlify dashboard: hilarious-madeleine-0801d5.netlify.app
2. Drag the entire canadasteps/ folder onto the deploy drop zone
3. Verify at canadasteps.org:
   - / loads index.html homepage (not a redirect)
   - /pgwp.html loads PGWP guide with nav links
   - /sin.html loads SIN guide with nav links
   - Nav links between pages work in both directions
4. After deploy confirmed: update memory/current_state.md — mark sin.html and index.html as live

Do not edit any HTML files during this task.
Commit: "ops: post-deploy state update" after confirming live.
