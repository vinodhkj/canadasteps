# Current State

_Updated: 2026-05-27_

## Phase

Phase 0 — Foundation

## Live pages

- `pgwp.html` — PGWP guide, live at canadasteps.org/pgwp.html
- `sin.html` — SIN guide, built but NOT YET DEPLOYED
- `index.html` — guides homepage, built but NOT YET DEPLOYED

## What works

- Site is LIVE at canadasteps.org/pgwp.html
- Deployed via Netlify manual drag-and-drop
- DNS connected and verified May 26, 2026
- SSL certificate active

## Last change

May 27 — Editorial trust pass: nav anchored with 2px navy border, logo enlarged, nav-links moved to sans-serif, topbar emoji removed, founder note bar removed (now transparent attribution line), h2 enlarged, gov-icon boxes muted. All 3 pages.

## Previous change (pre-trust-pass)

May 27 � Trust-polish pass: local/system font stacks, Google Fonts removed, teal slightly muted.

## Previous change

May 27 — f373ebb — Guides connected as workflow system:
- pgwp.html: "Next step" card added before disclaimer → links to /sin.html
- sin.html: "More guides coming" card added before disclaimer
- index.html: category labels added above each guide card (Study & Graduation / Working in Canada)

## Frozen files

- pgwp.html content is frozen — no edits until second user feedback received
  (nav and transition card additions in this session are exempt as structural, not content)

## What is incomplete

- assets/style.css does not exist — all pages use inline styles
- sin.html not yet deployed
- index.html not yet deployed
- docs/sources-log/sin.md not yet created
- No automated link-checking

## Immediate next action

Deploy to Netlify: drag canadasteps folder. Deploys pgwp.html, sin.html, index.html, and nav in one push.

## File structure note

- Canonical pgwp.html is in the PROJECT ROOT
- pages/pgwp.html has been removed (was a duplicate)
- Do not recreate pages/pgwp.html

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
