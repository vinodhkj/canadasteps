# Current State

_Updated: 2026-05-28_

## Phase

Phase 1 - Editorial redesign refinement

## Live pages

- `index.html` - guides homepage, live at canadasteps.ca/
- `pgwp.html` - PGWP guide, live at canadasteps.ca/pgwp.html
- `sin.html` - SIN guide, live at canadasteps.ca/sin.html
- `taxes.html` - tax filing guide, live at canadasteps.ca/taxes.html
- `cra-account.html` - CRA My Account guide, live at canadasteps.ca/cra-account.html
- `bank-account.html` - bank account and GIC basics guide, live at canadasteps.ca/bank-account.html
- `ontario-drivers-license.html` - Ontario driver's licence guide, pending deploy at canadasteps.ca/ontario-drivers-license.html
- `phone-plan.html` - phone plan guide for newcomers, live at canadasteps.ca/phone-plan.html
- `ontario-photo-card.html` - Ontario Photo Card guide, live at canadasteps.ca/ontario-photo-card.html

## What works

- Site is LIVE at canadasteps.ca
- Production deployment pipeline is Local -> GitHub -> Cloudflare Pages -> canadasteps.ca
- Cloudflare Pages auto-deploys on git push to main
- Netlify removed from active deployment workflow; no more manual drag/drop deployments
- DNS connected and verified May 26, 2026
- SSL certificate active

## Last change

May 29 - Newcomer journey sequencing: homepage sections renamed (First Weeks→Just Arrived, Money & Taxes→Working & Daily Life, Study & Immigration→Graduation & Immigration); entry order in Just Arrived updated (Phone Plan before Photo Card, Driver's License last); orientation descriptions updated for each stage. index.html only.

## Layout system — settled (May 29)

Approach: centered outer frame, left-aligned content inside. This matches Apple Support / GOV.UK / modern public-reference sites.
- Homepage .page-banner-inner + .page-wrap: max-width 1100px, margin: 0 auto
- Guide pages .page-wrap: max-width 1000px, margin: 0 auto
- Mobile (≤600px): full-width via padding, no margin overrides needed
- .site-footer-inner: margin: 0 auto on all pages (unchanged)
- All content inside containers remains left-aligned — text, headings, rows

Why the left-rail was reverted:
- clamp(1.5rem, 5vw/4vw, 6rem/5rem) created visible dead space on right at 1200–1600px
- Document/PDF feel replaced balanced website feel
- Inconsistency between homepage and guide pages read as a layout error
- Centered frame with wider max-width achieves the same editorial weight without the imbalance

## Previous change (implementation)

May 29 - Unified editorial rail across all 9 pages:
  - Homepage (.page-banner-inner + .page-wrap): margin-left: clamp(1.5rem, 5vw, 6rem); margin-right: auto
  - Guide pages (.page-wrap, all 8 files): margin-left: clamp(1.5rem, 4vw, 5rem); margin-right: auto
  - Mobile breakpoints on all guide pages: margin-left: 0 explicitly added
  - .site-footer-inner remains margin: 0 auto on all pages (footer stays centered)
  Layout only — no content, color, or typography changes.

## Previous change

May 29 - Phase 1 editorial authenticity pass: removed Inter from font stack (system fonts only), removed hover slide transform from guide entries, removed border-radius from disclaimer, promoted "Last reviewed" date visibility, added newcomer orientation line before first section. index.html only.

## Previous change

May 28 - Phase 1 refinement polish: homepage editorial guide entries gained subtle metadata, hover hierarchy, wider editorial measure, improved anchor scroll breathing, and calmer institutional trust-strip copy. PGWP visual language was softened through reusable CSS to reduce stacked-box repetition without rewriting content.

## Previous change

May 28 - Phase 1 homepage editorial redesign: page-banner zone (full-width bg-soft header), guide cards replaced with editorial list entries (rule-separated title + desc), h1 enlarged, "Live" badges removed, section spacing increased. index.html only.

## Previous change

May 28 - Phone Plan Guide added: phone-plan.html created (7 sections, CRTC/CCTS sources), homepage First Weeks card added, footer updated, transition cards added to sin.html and bank-account.html.

## Previous change

May 28 - Ontario Driver's License Guide added as a Daily Life page; homepage now includes a live guide card for it.

## Frozen files

- pgwp.html content is frozen - no edits until second user feedback received
  (nav and transition card additions are exempt as structural, not content)

## What is incomplete

- assets/style.css does not exist - all pages use inline styles
- docs/sources-log/sin.md not yet created
- No automated link-checking

## Immediate next action

Review the Phase 1 polish in browser after deployment, especially homepage anchor landing, mobile guide-entry rhythm, and PGWP section density.

## File structure note

- Canonical site files are in `canadasteps/`
- `pages/pgwp.html` has been removed (was a duplicate)
- Do not recreate `pages/pgwp.html`

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
