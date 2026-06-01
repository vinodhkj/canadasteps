# Current State

_Updated: 2026-05-31 (mobile nav + hero shortcut + identity polish)_

## Phase

Phase 1 - Editorial redesign refinement

## Live pages

- `pr-pathways.html` - PR pathways navigation guide, live at canadasteps.ca/pr-pathways.html
- `index.html` - guides homepage, live at canadasteps.ca/
- `pgwp.html` - PGWP guide, live at canadasteps.ca/pgwp.html
- `spouse-work-permit.html` - spouse open work permit navigation guide, live at canadasteps.ca/spouse-work-permit.html
- `sin.html` - SIN guide, live at canadasteps.ca/sin.html
- `taxes.html` - tax filing guide, live at canadasteps.ca/taxes.html
- `cra-account.html` - CRA My Account guide, live at canadasteps.ca/cra-account.html
- `bank-account.html` - bank account and GIC basics guide, live at canadasteps.ca/bank-account.html
- `gic-unlock.html` - GIC unlock guide for international students, pending deploy at canadasteps.ca/gic-unlock.html
- `ontario-drivers-license.html` - Ontario driver's licence guide, live at canadasteps.ca/ontario-drivers-license.html
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

May 31 - Mobile nav + hero shortcut + identity polish: index.html — (1) nav reordered: All guides / SIN / PGWP / PR / Work & Life / Graduation so PR visible early on mobile; (2) fake search-mock replaced with static shortcut panel (10 buttons: SIN, PGWP, PR, Banking, Taxes, CRA, Photo Card, Driver's Licence, Phone Plan, GIC Unlock); (3) maple identity layer: --maple #b23a32 + --maple-soft #f7e7e3, logo dot teal→maple, section nums maple, card-arrow maple; (4) SVG icons on all 11 guide cards (30×30 maple-soft badge, stroke-based, no library). pgwp.html unchanged. Pending user approval — not committed.

## Backlog (do not implement now)

1. Generic newcomer wording — pages over-referencing "international students": ontario-drivers-license.html, ontario-photo-card.html, taxes.html, cra-account.html, bank-account.html, phone-plan.html. Use broader wording (newcomers, new residents, Ontario residents, etc.). Keep student-specific only where genuinely relevant.
2. "Plain-English map" overuse — replace with "guide," "checklist," "overview," "starting point" except on pathway-style pages.
3. Safety wording — review pr-pathways.html (overconfident transition wording), spouse-work-permit.html (spouse eligibility wording), cra-account.html (NOA registration warning), official-source label wording.
4. SEO + trust content review — homepage, PGWP, SIN, internal linking, title/meta, FAQ opportunities, legal-advice wording. Prioritized backlog (must fix / should improve / nice to have). Conservative — no broad rewrites.

## Previous change (committed 025136e)

May 31 - Direction B + Direction A redesign: index.html guide entries converted to card panels; hero metrics strip added; pgwp.html: Inter removed, scope-module, toned warning boxes, outlined step-nums, route-cards Step 5.

## Previous change

May 30 - Must Fix Before Deploy: PGWP form accuracy corrected (IMM 5710 default, IMM 1295 alternative); SettleWise rulebook compliance added (Page Status Bar, "What SettleWise Does Not Answer" safety block); mobile usability improved (horizontal-scroll nav, table scrolling, and expanded touch targets on nav/footer links). index.html and pgwp.html only.

## Previous change

May 30 - GA4 added: Google Analytics 4 tag (G-4M1LTVRG81) inserted immediately after <head> on all 12 public HTML pages. Draft/internal files skipped. Next: deploy to Cloudflare Pages, verify in GA4 Realtime, monitor Cloudflare Core Web Vitals for regressions. UI redesign with Claude Design is separate — do not mix with this commit.

## Previous change

May 30 - SEO setup: sitemap.xml and robots.txt created at site root. Sitemap includes homepage + 11 public guide pages (no drafts or internal files). Google Search Console domain ownership verified via DNS. Next: deploy, verify URLs live, then submit sitemap in Search Console. UI redesign work with Claude Design is separate and ongoing — do not mix with this commit.

## Previous change

May 29 - PR nav restored: PR link added back to all 12 pages as last nav item; `Working & Daily Life` shortened to `Work & Life`; `Graduation & Immigration` shortened to `Graduation` for mobile fit. PR section remains in its own homepage section (long-term planning, not day-one).

May 29 - PR nav/risk cleanup: PR nav link removed from all 12 pages (footer links and page content unaffected); pr-pathways.html intro reframed to explicit plain-English map statement with negations; spouse-work-permit.html gained standalone bridge warning note (temp status vs PR sponsorship are separate IRCC processes).

May 29 - PR/legal-risk cleanup: spouse-work-permit.html reality-check gained two explicit bullets (Spouse Open Work Permit is temporary only; visitor visas/work permits/PR sponsorship are different processes); nav label "PR Pathways" → "PR" on all 12 pages (mobile wrapping; homepage section title unchanged). No layout, color, or content structure changes.

## Previous change

May 29 - PR Pathways Guide added: pr-pathways.html created (9 sections, IRCC-only sources, strict no-eligibility-advice guardrails, higher-risk immigration topic); index.html updated with new PR Pathways section and nav; PR Pathways nav link and footer link added to all 12 pages; related-guide transitions added to pgwp.html and spouse-work-permit.html; R10 risk logged.

## Previous change

May 29 - Spouse Open Work Permit Guide added: spouse-work-permit.html created (7 sections, IRCC sources only, process-navigation framing, strict immigration-advice guardrails); index.html updated with guide entry under Graduation & Immigration; footer updated on all 11 pages.

## Previous change

May 29 - GIC Unlock Guide added: gic-unlock.html created (8 sections, IRCC sources); index.html updated with guide entry under Just Arrived; bank-account.html updated with GIC Unlock transition card; GIC Unlock added to footer on all 10 pages.

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
