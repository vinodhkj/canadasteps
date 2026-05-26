# Next Session Prompt

Paste this at the start of the next working session.

---

We are building CanadaSteps (canadasteps.org) — a plain-language immigration guidance website for newcomers to Canada. Static HTML, no backend, editorial-first.

**Current phase:** Phase 0 — Foundation

**Where we left off:** Project scaffold complete. All documentation written. pgwp.html stub exists but content is not finished.

**Immediate goal for this session:** Complete the PGWP page.

**Next steps (in order):**

1. Open `pages/pgwp.html` and complete the content:
   - Verify eligibility rules against current IRCC PGWP page
   - Verify PGWP validity rules (8 months to 2 years / 2 years or more)
   - Add the 180-day application window with source
   - Add the application fee (link directly to IRCC fee page, do not paraphrase)
   - Add inline date attribution ("as of [Month Year] per IRCC")
   - Link processing time section to live IRCC tool

2. Create `docs/sources-log/pgwp.md` with source citations for every factual claim

3. Run the editorial rulebook checklist against pgwp.html

4. Create `assets/style.css` (minimal, mobile-first, system fonts)

5. Run `git init` and make the first commit

**Key files:**
- `docs/editorial-rulebook.md` — all editorial rules
- `docs/sources-log/` — source citations go here
- `implementation_plan.md` — full step-by-step plan
- `risks.md` — known risks and mitigations
- `memory/current_state.md` — current project state

**Rules to follow:**
- Never paraphrase fees — quote and link
- Never state processing times as a number — link to live tool
- Grade 8 reading level
- Disclaimer block on every page
- No features not in `requirements.md`
