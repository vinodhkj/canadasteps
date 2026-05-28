# Current State

_Updated: 2026-05-28_

## Phase

Phase 0 - Foundation

## Live pages

- `index.html` - guides homepage, live at canadasteps.ca/
- `pgwp.html` - PGWP guide, live at canadasteps.ca/pgwp.html
- `sin.html` - SIN guide, live at canadasteps.ca/sin.html
- `taxes.html` - tax filing guide, live at canadasteps.ca/taxes.html
- `cra-account.html` - CRA My Account guide, live at canadasteps.ca/cra-account.html
- `bank-account.html` - bank account and GIC basics guide, live at canadasteps.ca/bank-account.html

## What works

- Site is LIVE at canadasteps.ca
- Production deployment pipeline is Local -> GitHub -> Cloudflare Pages -> canadasteps.ca
- Cloudflare Pages auto-deploys on git push to main
- Netlify removed from active deployment workflow; no more manual drag/drop deployments
- DNS connected and verified May 26, 2026
- SSL certificate active

## Last change

May 28 - Homepage Start Here flow added before guide cards; Start Here nav now anchors to the practical step-by-step flow.

## Previous change

May 27 - Editorial trust pass: nav anchored with 2px navy border, logo enlarged, nav-links moved to sans-serif, topbar emoji removed, founder note bar removed (now transparent attribution line), h2 enlarged, gov-icon boxes muted. All 3 pages.

## Frozen files

- pgwp.html content is frozen - no edits until second user feedback received
  (nav and transition card additions are exempt as structural, not content)

## What is incomplete

- assets/style.css does not exist - all pages use inline styles
- docs/sources-log/sin.md not yet created
- No automated link-checking

## Immediate next action

Push main to GitHub; Cloudflare Pages should auto-deploy the homepage Start Here flow and recent visual/navigation polish to canadasteps.ca.

## File structure note

- Canonical pgwp.html is in the PROJECT ROOT
- pages/pgwp.html has been removed (was a duplicate)
- Do not recreate pages/pgwp.html

---

## SIN guide - verified source facts

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

- PROCESSING TIMES: Online - about 5 business days. By mail - about 20 business days.
  Do not state as fixed - link to official source.

- NO FEE (verbatim): "There is no fee to apply for a SIN." Safe to state.

- REQUIRED DOCUMENT - temporary resident: Primary document is work permit issued by IRCC.
  Study permit must state "may accept employment" or "may work" in Canada.
