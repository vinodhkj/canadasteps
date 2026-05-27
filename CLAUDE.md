# CanadaSteps — Claude Project Context

## What this project is

CanadaSteps (canadasteps.org) is a plain-language guidance website for newcomers to Canada. It explains immigration pathways, permits, and settlement steps in clear, jargon-free English aimed at people whose first language may not be English. Non-commercial, independently maintained.

## Audience

- Primary: newcomers and prospective immigrants (international students, temporary workers, PR applicants, sponsored family)
- Secondary: settlement workers looking for quick reference material

## Architecture guardrails

- **Static HTML only.** No backend, no database, no server-side code.
- **No JavaScript required** for any core content function.
- **No external dependencies** in `<head>` — no CDN scripts, no web fonts, no tracking pixels.
- **No framework** (no React, Vue, or Angular). Plain HTML + CSS.
- **No CMS** until 25+ pages with multiple contributors — evaluated explicitly, not assumed.

## Coding standards

- Semantic HTML: use `<article>`, `<section>`, `<aside>`, `<nav>`, `<main>`, `<header>`, `<footer>`.
- One `<h1>` per page, matches `<title>`.
- All external links: `target="_blank" rel="noopener"`.
- All images: meaningful `alt` attribute, never empty for informational images.
- Inline CSS is banned. All styles in `assets/style.css`.
- No inline JavaScript. No `onclick` attributes.
- Indentation: 2 spaces.

## Editorial standards (summary — full rules in docs/editorial-rulebook.md)

- One claim = one official source, logged in `docs/sources-log/<page-slug>.md`
- Never paraphrase fee amounts — quote directly and link to source
- Never state processing times as fixed numbers — link to live IRCC tool
- Inline date attribution: "as of [Month Year] per IRCC"
- Disclaimer block on every page (verbatim from rulebook Section 8)
- Grade 8 reading level or below (Flesch-Kincaid ≥ 60)
- No legal advice language ("you should", "you must" → "IRCC requires", "applicants typically")

## Testing rules

No automated test suite. The test is the editorial checklist in `docs/editorial-rulebook.md` Section 9.

Before any page ships:
1. Run the full checklist manually
2. Check all links (open every external link)
3. View on mobile viewport
4. Verify source log is complete

## Git workflow

- Commits should be meaningful: describe what changed and why, not just "update page"
- Commit after each page is completed and source-verified, not during drafting
- Main branch is the live branch — don't commit unfinished content
- Draft content in a branch or local file until it's ready

## Risk awareness

See `risks.md` for the full risk register. Critical risks:

- Content rot: IRCC changes policy without notice
- Inadvertent legal advice: phrasing that implies personalized guidance
- Scope creep: features added before confirmed reader demand

## What NOT to build yet

See `memory/rejected_approaches.md` for the complete list. Summary:

- No CMS, calculator, chatbot, newsletter, user accounts, comments, or consultant directory
- No analytics that track individual users
- No monetization features in Phase 0–1
- No static site generator until 25+ pages

## Startup priorities

1. Get one page live and source-verified
2. Get one real reader
3. Get feedback
4. Then plan Phase 1

Do not optimize for architecture or scale before having real readers.

## Operational philosophy

Boring, maintainable technology. Minimum operational surface. Zero servers to patch. Content that a second contributor could pick up from the documentation alone without asking questions. Every decision that increases complexity requires a written justification.

## Key files

| File | Purpose |
|------|---------|
| `docs/editorial-rulebook.md` | All editorial standards |
| `docs/project-status.md` | Sprint tracker |
| `docs/sources-log/` | Per-page source citations |
| `requirements.md` | What we're building and what's explicitly out of scope |
| `design.md` | Architecture decisions and rationale |
| `roadmap.md` | Phased plan with milestone gates |
| `risks.md` | Risk register |
| `implementation_plan.md` | Current execution steps |
| `memory/next_prompt.md` | Handover prompt for next session |
| `memory/rejected_approaches.md` | Settled decisions — do not relitigate |

## Shared Memory Workflow

Before starting work:
1. Read:
   - memory/current_state.md
   - memory/next_prompt.md
   - memory/risks.md
   - memory/changed_files.md
   - daily.md

After completing work:
1. Update:
   - memory/current_state.md
   - memory/next_prompt.md
   - memory/changed_files.md
2. Append one concise line to daily.md
3. Update memory/risks.md only if a new risk or ambiguity is found
4. Create one clear commit only

## Project Rules

- CanadaSteps is an operational immigrant guidance site
- Official-source-first
- No speculative legal advice
- Minimal diff only
- Prefer small commits
- Do not redesign unrelated pages
- PGWP page is frozen unless explicitly reopened
- If a source ambiguity exists, stop and log it in memory/risks.md before proceeding

## Agent Coordination

- Claude Code and Codex share the same memory files
- Never overwrite another agent's handoff notes
- Preserve append-only history in daily.md
- Record changed files in memory/changed_files.md

## When working with Claude on this project

- Before drafting content: ask "What is the official IRCC URL for this claim?"
- Before adding a feature: apply the Scope Guard check (memory/rejected_approaches.md)
- Before publishing any page: run the editorial checklist (docs/editorial-rulebook.md Section 9)
- After a session: update memory/current_state.md and memory/next_prompt.md

## Standard Update Workflow

After every change to the project, always:

1. Run git status to confirm what changed
2. Stage and commit with a clear descriptive message
3. Update memory/current_state.md to reflect latest state
4. Update docs/project-status.md if sprint status changed
5. Update daily.md with a one-line session log entry

This applies to every change — content, fixes, structure, or documentation. No exceptions.

## Token Optimization Rules

To minimize context window usage every session:

### Session Start
- Read ONLY memory/next_prompt.md first
- Do not read entire codebase on startup
- Do not read all docs unless task requires it
- Ask clarifying question if task is ambiguous before reading any files

### During Work
- Read only the specific file being edited
- Do not re-read files already in context
- Do not summarize back large blocks of content
- Confirm changes in one line not paragraphs

### File Reading Priority
- memory/next_prompt.md — always first
- memory/current_state.md — only if needed
- Specific file being changed — only that file
- docs/ — only if content decision required
- Never read all files to "get context"

### Commit and Close
- git status
- commit with clear message
- update memory/current_state.md — 5 lines max
- update memory/next_prompt.md — 3 lines max
- update daily.md — one line only

### What NOT To Do
- Do not read pgwp.html to answer a question about project status
- Do not read rulebook unless writing new content
- Do not re-read sources log unless updating it
- Do not summarize entire session back to user

Goal: Every session starts in under 30 seconds with next_prompt.md only.

## Handoff Update Standard

After every completed task, update these files before committing:

**memory/current_state.md**
- Current live pages
- Latest commit hash
- What changed
- What is frozen / should not be edited

**memory/next_prompt.md**
- Exact next task prompt
- Files allowed to read
- Files allowed to edit
- Explicit do-not-touch items

**memory/changed_files.md**
- Files changed in this task
- One-line reason per file

**memory/risks.md**
- Only update if a new risk, ambiguity, source gap, or unresolved question appears
- Do not rewrite old risks unnecessarily

**daily.md**
- Append one concise line: date | task | result | commit hash

Rule: Do not commit unless memory files reflect the repo state.

memory/next_prompt.md is the handoff source of truth between sessions.
