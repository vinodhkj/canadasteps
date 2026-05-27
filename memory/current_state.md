# Current State

_Updated: 2026-05-27_

## Phase

Phase 0 — Foundation

## What exists

- pgwp.html — canonical file at project root (this is the live file)
- index.html — root redirect to /pgwp.html
- docs/sources-log/pgwp.md — complete source log, last verified May 26, 2026
- docs/editorial-rulebook.md — complete
- user-feedback/pgwp-feedback-round1.md — Round 1 feedback logged
- Git: initialized, multiple commits from May 26, 2026 session

## What works

- Site is LIVE at canadasteps.org/pgwp.html
- Deployed via Netlify manual drag-and-drop
- DNS connected and verified May 26, 2026
- SSL certificate active
- index.html redirects to /pgwp.html

## Last change
May 27 — Shared agent memory workflow added to CLAUDE.md and AGENTS.md.

## What was shipped (May 26 session)

- Reality check box (180-day window, work authorization warning)
- One-PGWP lifetime warning box
- PGWP timeline at a glance
- Cost table (fees and processing time)
- Step 05 portal navigation note for language test upload
- Step 10 work authorization language clarified
- Maintained status URL corrected to verified IRCC page

## File structure note

- Canonical pgwp.html is in the PROJECT ROOT
- pages/pgwp.html has been removed (was a duplicate)
- Do not recreate pages/pgwp.html

## What is incomplete

- assets/style.css does not exist — both pages use inline styles
- sin.html not yet deployed — draft only, awaiting review
- No automated link-checking

## Immediate next action

Deploy to Netlify (drag canadasteps folder). Both guides live, homepage live, nav complete.

---

## SIN guide — verified source facts

Source: canada.ca/en/employment-social-development/services/sin/update.html
Verified: May 26, 2026

- UPDATE METHOD: Online, by mail, and in-person are all available for temporary residents
  updating their SIN record. Not in-person only. (Resolves architecture ambiguity.)

- MAINTAINED STATUS (verbatim): "If your SIN is expired, you may continue to work while
  waiting for your new immigration document if you maintain your status during the processing."
  Safe to quote directly.

- POST-APPROVAL OBLIGATION (verbatim): "Once IRCC authorizes you to continue working in
  Canada, you must apply to Service Canada with your new immigration document to update the
  expiry date on your SIN record." Safe to quote directly.

- EXPIRY DATE MATCHING (verbatim): "The expiry date on both your SIN record and your
  immigration document must match." Safe to include.

- PROCESSING TIMES: Online — about 5 business days. By mail — about 20 business days.
  Do not state as fixed — link to official source.

- NO FEE (verbatim): "There is no fee to apply for a SIN." Safe to state.

- REQUIRED DOCUMENT — temporary resident: Primary document is work permit issued by IRCC.
  Study permit must state "may accept employment" or "may work" in Canada.
