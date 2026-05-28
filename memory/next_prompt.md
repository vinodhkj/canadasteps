# Next Session Prompt

Paste this at the start of the next working session.

---

We are building CanadaSteps, primary domain canadasteps.ca, with canadasteps.org as alias.

Static HTML site. No backend. Editorial-first newcomer guidance.

Current state:
- Homepage exists at index.html.
- PGWP guide exists at pgwp.html.
- SIN guide exists at sin.html.
- Navigation/homepage workflow structure is complete.
- Shared Claude/Codex agent memory workflow exists.
- Latest local work: final proportional polish across index.html, pgwp.html, and sin.html.
- Changes may be uncommitted or not yet deployed, so verify git status first.

Start by running:
git status
git log --oneline -5

Then verify whether the latest final proportional polish commit exists.

If changes are uncommitted:
1. Review diff.
2. Update memory files if needed:
   - memory/current_state.md
   - memory/next_prompt.md
   - memory/changed_files.md
   - daily.md
3. Commit:
   style: improve readability and site grounding

Then deploy manually:
- Drag C:\Projects\SG\CanadaSteps.ca\canadasteps into Netlify deploy drop zone.

After deploy, verify:
- https://canadasteps.ca/
- https://canadasteps.ca/pgwp.html
- https://canadasteps.ca/sin.html
- navigation links work
- founder note exists on all pages
- mobile view looks clean

Do not edit content, architecture, navigation, agent workflow, or memory format.

If deploy is clean:
- update memory/current_state.md
- update daily.md
- commit:
  ops: post-deploy state update

Then stop building.