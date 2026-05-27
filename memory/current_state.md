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
May 27 — Post-PGWP next steps block added between Step 11 and section 04 (SIN update, health coverage, document safety, work authorization proof). Service Canada SIN link included.

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

- assets/style.css does not exist — pgwp.html uses inline styles
- No second page published yet
- No automated link-checking

## Immediate next action

SIN guide architecture in progress. Full structure, source map, and ambiguity flags produced. Next step: verify 7 sourcing gaps directly on canada.ca sub-pages before writing any HTML.
