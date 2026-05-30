# Changed Files

---
## 2026-05-30 - Must Fix Before Deploy: UI, Accessibility & Form Accuracy

**Modified:**
- `index.html` — added Page Status Bar; increased navigation and footer tap targets; implemented responsive horizontally-scrollable navigation bar for mobile viewports to prevent screen clogging.
- `pgwp.html` — corrected PGWP form guidance to IMM 5710 (in-Canada) as the primary default and IMM 1295 (outside-Canada) as the alternative; added mandatory "What SettleWise Does Not Answer" safety block; added Page Status Bar; hyperlinked processing times in meta row to official IRCC source; fixed horizontal scrolling for the cost table; brought horizontal-scroll nav bar and padding improvements to match index.html.

**Also modified:**
- `memory/current_state.md`, `memory/next_prompt.md`, `memory/changed_files.md`, `daily.md`

---
## 2026-05-30 - GA4 analytics added

**Modified (all 12 public pages):**
- `index.html`, `sin.html`, `bank-account.html`, `cra-account.html`, `gic-unlock.html`, `ontario-drivers-license.html`, `ontario-photo-card.html`, `pgwp.html`, `phone-plan.html`, `pr-pathways.html`, `spouse-work-permit.html`, `taxes.html` — GA4 tag (G-4M1LTVRG81) inserted immediately after `<head>`; no other changes

**Skipped:** `Pages/pgwp-v01.html`, all `.md`, memory, docs

**Also modified:**
- `memory/current_state.md`, `memory/next_prompt.md`, `memory/changed_files.md`, `daily.md`

---
## 2026-05-30 - SEO setup: sitemap and robots

**Created:**
- `sitemap.xml` — homepage + 11 public guide pages; excludes Pages/pgwp-v01.html (draft) and all internal/memory files; lastmod 2026-05-29
- `robots.txt` — allows all crawlers; references https://canadasteps.ca/sitemap.xml

**Note:** Google Search Console domain ownership verified via DNS prior to this commit.

**Modified:**
- `memory/current_state.md` — SEO setup recorded
- `memory/next_prompt.md` — post-deploy verification steps added
- `memory/changed_files.md` — this entry
- `daily.md` — appended session log line

---
## 2026-05-29 - PR/legal-risk cleanup (post-Gemini validation)

**Modified:**
- `spouse-work-permit.html` — reality-check: added two explicit bullets clarifying (1) Spouse Open Work Permit is temporary work authorization only, not PR; (2) visitor visas/work permits/PR sponsorship are separate IRCC processes
- `pr-pathways.html` — nav label: "PR Pathways" → "PR" (mobile; section title and track-tag unchanged)
- `index.html` — nav label: same
- `pgwp.html` — nav label: same
- `sin.html` — nav label: same
- `taxes.html` — nav label: same
- `cra-account.html` — nav label: same
- `bank-account.html` — nav label: same
- `gic-unlock.html` — nav label: same
- `ontario-drivers-license.html` — nav label: same
- `phone-plan.html` — nav label: same
- `ontario-photo-card.html` — nav label: same
- `memory/current_state.md` — recorded this change
- `memory/changed_files.md` — this entry
- `memory/risks.md` — no new risks; existing R10/R9 still active
- `daily.md` — appended session log line

---
## 2026-05-29 - PR Pathways Guide added

**Created:**
- `pr-pathways.html` — new PR pathways navigation guide; 9 sections; IRCC-only sources; strict process-navigation framing with no eligibility claims, no CRS commentary, no draw predictions; higher-risk immigration topic guardrails applied throughout

**Modified:**
- `index.html` — added PR Pathways nav link; added CSS accent rules for #pr-pathways section; added new #pr-pathways section with guide entry; added PR Pathways to footer
- `pgwp.html` — added PR Pathways nav link; added PR Pathways related-guide transition card; added Phone Plan, Photo Card, PR Pathways to footer (footer was incomplete)
- `spouse-work-permit.html` — added PR Pathways nav link; added PR Pathways related-guide transition in next-guides section; added PR Pathways to footer
- `sin.html` — added PR Pathways nav link; added PR Pathways to footer
- `taxes.html` — added PR Pathways nav link; added PR Pathways to footer
- `cra-account.html` — added PR Pathways nav link; added PR Pathways to footer
- `bank-account.html` — added PR Pathways nav link; added PR Pathways to footer
- `gic-unlock.html` — added PR Pathways nav link; added PR Pathways to footer
- `ontario-drivers-license.html` — added PR Pathways nav link; added PR Pathways to footer
- `phone-plan.html` — added PR Pathways nav link; added PR Pathways to footer
- `ontario-photo-card.html` — added PR Pathways nav link; added PR Pathways to footer
- `memory/current_state.md` — recorded this change; added pr-pathways.html to live pages
- `memory/next_prompt.md` — added pr-pathways.html to current pages list
- `memory/changed_files.md` — this entry
- `memory/risks.md` — added R10 for PR pathways content-rot and immigration-advice risk
- `daily.md` — appended session log line



_Tracks files created or modified each session._

---
## 2026-05-29 - Spouse Open Work Permit Guide added

**Created:**
- `spouse-work-permit.html` — new spouse/family work permit navigation guide; 7 sections; IRCC-only sources; strict process-navigation framing with no eligibility claims; higher-risk immigration topic guardrails applied

**Modified:**
- `index.html` — added Spouse Work Permit Guide entry under Graduation & Immigration; added link to footer
- `pgwp.html` — added Spouse Work Permit link to footer
- `sin.html` — added Spouse Work Permit link to footer
- `taxes.html` — added Spouse Work Permit link to footer
- `cra-account.html` — added Spouse Work Permit link to footer
- `bank-account.html` — added Spouse Work Permit link to footer
- `gic-unlock.html` — added Spouse Work Permit link to footer
- `phone-plan.html` — added Spouse Work Permit link to footer
- `ontario-drivers-license.html` — added Spouse Work Permit link to footer
- `ontario-photo-card.html` — added Spouse Work Permit link to footer
- `memory/current_state.md` — recorded this change; added spouse-work-permit.html to live pages
- `memory/next_prompt.md` — added spouse-work-permit.html to current pages list
- `memory/changed_files.md` — this entry
- `memory/risks.md` — added R9 for spouse/family permit content-rot risk
- `daily.md` — appended session log line

---
## 2026-05-29 - GIC Unlock Guide added

**Created:**
- `gic-unlock.html` — new GIC activation guide for international students; 8 sections; IRCC sources; includes question cards, checklist, steps, miss-items

**Modified:**
- `index.html` — added GIC Unlock Guide entry under Just Arrived (between Bank Account and Phone Plan); added GIC Unlock to footer
- `bank-account.html` — added GIC Unlock transition card in What Comes Next section; added GIC Unlock to footer
- `sin.html` — added GIC Unlock to footer
- `taxes.html` — added GIC Unlock to footer
- `cra-account.html` — added GIC Unlock to footer
- `pgwp.html` — added GIC Unlock to footer
- `phone-plan.html` — added GIC Unlock to footer
- `ontario-drivers-license.html` — added GIC Unlock to footer
- `ontario-photo-card.html` — added GIC Unlock to footer
- `memory/current_state.md` — recorded this change
- `memory/next_prompt.md` — added gic-unlock.html to current pages list
- `memory/changed_files.md` — this entry
- `daily.md` — appended session log line

---
## 2026-05-29 - Mobile readability pass

**Modified (all 9 pages):**
- `index.html` — mobile breakpoint: nav wrapping, topbar/nav padding reduced
- `pgwp.html` — same
- `sin.html` — same; added .founder-note CSS; converted inline founder-note div to class
- `bank-account.html` — same as sin.html
- `taxes.html` — same as sin.html
- `cra-account.html` — same as sin.html
- `ontario-drivers-license.html` — same as sin.html
- `ontario-photo-card.html` — same as sin.html
- `phone-plan.html` — same as sin.html
- `memory/current_state.md` — recorded this change
- `memory/changed_files.md` — this entry
- `daily.md` — appended session log line

---
## 2026-05-29 - Trust clarity: topbar cleanup + CRA sequencing

**Modified:**
- `index.html` — topbar: replaced "Canada Immigration Guides — Educational Resource Only | Official IRCC ↗" with "Independent guide. Official sources linked on each page."
- `pgwp.html` — topbar: same
- `sin.html` — topbar: same
- `taxes.html` — topbar: same; NOA step updated to note CRA My Account requires assessed return; step-link → "Official CRA My Account"
- `cra-account.html` — topbar: same; reality-check box: sequencing bullet strengthened to clarify not a first-arrival task
- `bank-account.html` — topbar: same
- `phone-plan.html` — topbar: same
- `ontario-drivers-license.html` — topbar: same
- `ontario-photo-card.html` — topbar: same
- `memory/current_state.md` — recorded this change
- `memory/changed_files.md` — this entry
- `daily.md` — appended session log line

---
## 2026-05-29 - Guide nav anchor fix

**Modified:**
- `sin.html` — nav anchors and link text updated (#first-weeks→#just-arrived, #money-taxes→#working-daily-life, #study-immigration→#graduation-immigration)
- `bank-account.html` — same
- `phone-plan.html` — same
- `taxes.html` — same
- `cra-account.html` — same
- `ontario-drivers-license.html` — same
- `ontario-photo-card.html` — same
- `pgwp.html` — same
- `memory/current_state.md` — recorded this change
- `memory/changed_files.md` — this entry
- `memory/next_prompt.md` — removed stale risk note
- `daily.md` — appended session log line

---

## 2026-05-29 - Newcomer journey sequencing

**Modified:**
- `index.html` — sections renamed (Just Arrived / Working & Daily Life / Graduation & Immigration); IDs, CSS selectors, nav links, section-cat labels, h2 text, and orientation descriptions updated; Just Arrived entry order updated (Phone Plan before Photo Card, Driver's License last); removed duplicate orientation paragraph above sections
- `memory/current_state.md` — recorded this change
- `memory/changed_files.md` — this entry
- `memory/next_prompt.md` — noted anchor ID change risk for guide page nav links
- `daily.md` — appended session log line

---

## 2026-05-29 - Reference audit: footer nav, nav crumbs, track-tags, link text

**Modified:**
- `sin.html` — nav crumb "Settlement Track" → "First Weeks"; related guide link text standardized (Tax Filing Guide, Bank Account Guide); footer: added Phone Plan, Photo Card links
- `bank-account.html` — nav crumb "Money & Taxes" → "First Weeks"; track-tag "Money & Taxes" → "First Weeks" (class and text); footer: added Phone Plan, Photo Card links
- `taxes.html` — related guide link text standardized (CRA My Account Guide, Bank Account Guide, SIN Guide, PGWP Guide); footer: added Phone Plan, Photo Card links
- `cra-account.html` — footer: added Phone Plan, Photo Card links
- `ontario-drivers-license.html` — nav crumb "Daily Life" → "First Weeks"; track-tag "Daily Life" → "First Weeks"; footer: added Phone Plan, Photo Card links
- `ontario-photo-card.html` — nav crumb "Daily Life" → "First Weeks"; track-tag "Daily Life" → "First Weeks"
- `phone-plan.html` — footer: added Photo Card link
- `memory/current_state.md` — recorded this change
- `memory/changed_files.md` — this entry
- `daily.md` — appended session log line

---

## 2026-05-29 - Trust/QA pass: broken link fix + rel=noopener audit

**Modified:**
- `taxes.html` - fixed broken CRA URL slug: you-have-to-file-return.html → you-have-file-a-return.html (line 549). Correct URL confirmed via CRA site search.
- `pgwp.html` - added rel="noopener" to all 28 target="_blank" links that were missing it. No content changes.
- `memory/current_state.md` - recorded this change
- `memory/changed_files.md` - this entry
- `daily.md` - appended session log line

**Audited (no changes needed):**
- `sin.html` - all 21 external links have rel="noopener" ✓
- `cra-account.html` - all 8 external links have rel="noopener" ✓
- CRA login, register, My Account URLs confirmed valid via search ✓

---
## 2026-05-29 - Layout rebalance: remove asymmetric rail, restore centered frame

**Modified:**
- `index.html` - .page-banner-inner + .page-wrap: clamp rail removed, margin: 0 auto restored, max-width 980px → 1100px; mobile margin-left: 0 overrides removed
- `sin.html` - .page-wrap: clamp rail removed, margin: 0 auto, max-width 920px → 1000px; mobile margin-left: 0 removed
- `pgwp.html` - same (was 980px → 1000px)
- `taxes.html` - same (920px → 1000px)
- `cra-account.html` - same
- `bank-account.html` - same
- `ontario-drivers-license.html` - same
- `phone-plan.html` - same
- `ontario-photo-card.html` - same
- `memory/current_state.md` - recorded layout system decision and rationale
- `memory/changed_files.md` - this entry
- `memory/next_prompt.md` - updated layout state
- `daily.md` - appended session log line

---
## 2026-05-29 - Editorial rail documentation pass

**Modified:**
- `memory/current_state.md` - documented rail strategy, before/after, affected containers
- `memory/changed_files.md` - this entry
- `memory/next_prompt.md` - refreshed to reflect unified rail and current layout state
- `daily.md` - appended session log line

---
## 2026-05-29 - Unified editorial rail layout

**Modified:**
- `index.html` - homepage left margin reduced to clamp(1.5rem, 5vw, 6rem) on .page-banner-inner and .page-wrap
- `sin.html` - .page-wrap margin: 0 auto → clamp(1.5rem, 4vw, 5rem) left rail; mobile reset added
- `pgwp.html` - same
- `taxes.html` - same
- `cra-account.html` - same
- `bank-account.html` - same
- `ontario-drivers-license.html` - same
- `phone-plan.html` - same
- `ontario-photo-card.html` - same
- `memory/current_state.md` - recorded this change
- `memory/changed_files.md` - this entry
- `daily.md` - appended session log line

---
## 2026-05-29 - Left-anchor homepage editorial column

**Modified:**
- `index.html` - .page-banner-inner and .page-wrap margin changed from 0 auto to clamp left-anchor; mobile breakpoint resets added
- `memory/current_state.md` - recorded this change
- `memory/changed_files.md` - this entry
- `daily.md` - appended session log line

---
## 2026-05-29 - Phase 1 editorial authenticity pass

**Modified:**
- `index.html` - removed Inter from font stack, removed hover slide transform, removed disclaimer border-radius, promoted "Last reviewed" date, added newcomer orientation line
- `memory/current_state.md` - recorded this change
- `memory/changed_files.md` - this entry
- `daily.md` - appended session log line

---
## 2026-05-28 - Phase 1 editorial refinement polish

**Modified:**
- `index.html` - widened editorial layout, added scroll-margin breathing for homepage anchors, refined trust strip copy, strengthened guide-entry hover/title hierarchy, and added small entry metadata
- `pgwp.html` - aligned visual language with homepage by widening layout, replacing inline trust strip with reusable class, softening repeated boxed surfaces, increasing section rhythm, and converting the next-step block to reusable CSS
- `memory/current_state.md` - recorded Phase 1 refinement polish and corrected current file-structure note
- `memory/changed_files.md` - this entry
- `memory/next_prompt.md` - refreshed stale homepage guide list and next-priority handoff
- `daily.md` - appended concise session log line

---
## 2026-05-28 - Phase 1 homepage editorial redesign

**Modified:**
- `index.html` - page-banner zone, editorial list entries (guide-entries/guide-entry), larger h1, removed guide-card grid and Live badges, increased section spacing
- `.gitignore` - added .claude/ exclusion

---
## 2026-05-28 - Visual identity refresh (commit 5f307ca)

**Modified:**
- `index.html` - section accent CSS (teal/amber/navy borders), section-cat labels, founder-note class
- `bank-account.html` - track-tag amber variant CSS + HTML class
- `cra-account.html` - track-tag amber variant CSS + HTML class
- `taxes.html` - track-tag amber variant CSS + HTML class
- `ontario-drivers-license.html` - track-tag daily/navy variant CSS + HTML class
- `ontario-photo-card.html` - track-tag daily/navy variant CSS + HTML class

---
## 2026-05-28 - Ontario Photo Card Guide added

**Created:**
- `ontario-photo-card.html` - new Ontario Photo Card guide for international students and newcomers; 7 sections; ServiceOntario and Ontario.ca official links

**Modified:**
- `index.html` - added Ontario Photo Card Guide card to First Weeks section; added ontario-photo-card.html to footer links
- `memory/current_state.md` - recorded new ontario-photo-card.html page
- `memory/changed_files.md` - this entry
- `daily.md` - appended session log line

---
## 2026-05-28 - Phone Plan Guide added

**Created:**
- `phone-plan.html` - new phone plan guide for newcomers and international students; 7 sections; CRTC and CCTS official links

**Modified:**
- `index.html` - added Phone Plan Guide card to First Weeks section; added phone-plan.html to footer links
- `sin.html` - added phone plan related guide transition card before "coming soon" block
- `bank-account.html` - added phone plan related guide transition card in What Comes Next section; fixed CRA card arrow encoding
- `memory/current_state.md` - recorded new phone-plan.html page
- `memory/changed_files.md` - this entry
- `daily.md` - appended session log line

---
## 2026-05-28 - Trust and operational clarity pass

**Modified:**
- `index.html` - footer grounded: clearer institutional position, expanded guide links
- `pgwp.html` - footer grounded, topbar link softened (#f0c76a → rgba)
- `sin.html` - footer grounded, topbar link softened, "Settlement Track" → "First Weeks"
- `taxes.html` - footer grounded, topbar link softened
- `bank-account.html` - footer grounded, topbar softened, encoding fixed (→, ↗, —)
- `cra-account.html` - footer grounded, topbar softened, encoding fixed (→, ↗, —)
- `ontario-drivers-license.html` - footer grounded, topbar softened, all `->` fixed to `↗`/`→`, G1 caution note added, 2 new miss-items (experience letters, insurance/licence), "identity workflows" wording fixed
- `memory/current_state.md` - updated last change
- `memory/changed_files.md` - this entry
- `daily.md` - appended session log line

---
## 2026-05-28 - Homepage IA refactor: newcomer journey structure

**Modified:**
- `index.html` - restructured into 3 sections (First Weeks / Money & Taxes / Study & Immigration), updated nav, simplified top copy, softened IRCC topbar link, removed start-flow and guide-group CSS
- `sin.html` - nav updated: Start Here → First Weeks, PGWP → Study & Immigration
- `bank-account.html` - nav updated: Start Here → First Weeks, PGWP → Study & Immigration
- `taxes.html` - nav updated: Start Here → First Weeks, PGWP → Study & Immigration
- `cra-account.html` - nav updated: Start Here → First Weeks, PGWP → Study & Immigration
- `pgwp.html` - nav updated: Start Here → First Weeks, PGWP (current) → Study & Immigration (current)
- `ontario-drivers-license.html` - nav updated: current moved from All Guides to First Weeks; PGWP → Study & Immigration
- `memory/current_state.md` - recorded homepage IA refactor
- `memory/next_prompt.md` - updated nav and section structure
- `memory/changed_files.md` - recorded files changed in this task
- `daily.md` - appended concise session log line

---
## 2026-05-28 - Ontario Driver's License Guide added

**Created:**
- `ontario-drivers-license.html` - new Ontario driver's licence guide for international students and newcomers using existing guide layout and official DriveTest/Ontario links

**Modified:**
- `index.html` - added Daily Life guide card for Ontario Driver's License Guide
- `memory/current_state.md` - recorded new Ontario Driver's License Guide
- `memory/next_prompt.md` - refreshed current pages and homepage state
- `memory/changed_files.md` - recorded files changed in this task
- `daily.md` - appended concise session log line

---
## 2026-05-28 - Homepage Start Here flow

**Modified:**
- `index.html` - added lightweight Start Here flow before guide cards and moved the `#start-here` anchor to the new section
- `memory/current_state.md` - recorded homepage Start Here flow
- `memory/next_prompt.md` - refreshed current homepage state
- `memory/changed_files.md` - recorded files changed in this task
- `daily.md` - appended concise session log line

---
## 2026-05-28 - Visual comfort polish

**Modified:**
- `index.html` - warmed base palette, softened cards, and added subtle category label accents
- `pgwp.html` - warmed base palette and softened repeated guide surfaces
- `sin.html` - warmed base palette and softened repeated guide surfaces
- `taxes.html` - warmed base palette and softened repeated guide surfaces
- `cra-account.html` - warmed base palette and softened repeated guide surfaces
- `bank-account.html` - warmed base palette and softened repeated guide surfaces
- `memory/current_state.md` - recorded visual comfort polish
- `memory/next_prompt.md` - refreshed stale Cloudflare/current-pages handoff
- `memory/changed_files.md` - recorded files changed in this task
- `daily.md` - appended concise session log line

---

## 2026-05-28 - Navigation category cleanup

**Modified:**
- `index.html` - replaced stale guide-by-guide nav with category nav, added homepage anchors, and grouped Bank Account under Start Here
- `pgwp.html` - updated top nav to shared category nav
- `sin.html` - updated top nav to shared category nav with Start Here active
- `taxes.html` - updated top nav to shared category nav with Money & Taxes active
- `cra-account.html` - updated top nav to shared category nav with Money & Taxes active
- `bank-account.html` - updated top nav to shared category nav with Start Here active
- `memory/current_state.md` - recorded nav cleanup
- `memory/changed_files.md` - recorded files changed in this task
- `daily.md` - appended concise session log line

---

## 2026-05-28 - Bank Account Guide added

**Created:**
- `bank-account.html` - new bank account and GIC basics guide for international students using existing guide layout and official FCAC/CDIC links

**Modified:**
- `index.html` - added Bank Account Guide card under Money & Taxes
- `sin.html` - added related bank account guide transition card before disclaimer
- `taxes.html` - added related bank account/direct deposit guide transition card before disclaimer
- `cra-account.html` - added related bank account guide transition card where direct deposit setup is relevant
- `memory/current_state.md` - recorded new Bank Account Guide
- `memory/changed_files.md` - recorded files changed in this task
- `daily.md` - appended concise session log line

---

## 2026-05-28 - CRA My Account guide added

**Created:**
- `cra-account.html` - new CRA My Account guide for international students using existing guide layout and official Canada.ca/CRA links

**Modified:**
- `index.html` - added CRA My Account Guide card under Money & Taxes
- `taxes.html` - added related CRA My Account guide transition card before disclaimer
- `memory/current_state.md` - recorded new CRA My Account page and Cloudflare Pages workflow status
- `memory/changed_files.md` - recorded files changed in this task
- `daily.md` - appended concise session log line

---

## 2026-05-28 - Deployment workflow update

**Modified:**
- `memory/current_state.md` - documented Cloudflare Pages deployment workflow and removed Netlify from active workflow
- `memory/changed_files.md` - recorded Cloudflare Pages deployment workflow update
- `daily.md` - appended concise Cloudflare Pages auto-deploy note

---

## 2026-05-28 - CRA certified software link correction

**Modified:**
- `taxes.html` - corrected CRA certified software URL
- `memory/current_state.md` - noted CRA certified software link corrected
- `memory/changed_files.md` - recorded files changed in this task
- `daily.md` - appended concise session log line with commit hash

---

## 2026-05-28 - Tax filing guide added

**Created:**
- `taxes.html` - new tax filing guide, Money & Taxes track, 7 sections, CRA sources only

**Modified:**
- `index.html` - added "Money & Taxes" guide card + Tax Guide nav link + footer link
- `pgwp.html` - added Tax Guide nav link + footer link (structural only, content frozen)
- `sin.html` - added Tax Guide nav link + footer link + taxes transition card before disclaimer
- `memory/current_state.md` - updated to reflect taxes.html added, not yet deployed
- `memory/next_prompt.md` - updated handoff to deploy next
- `memory/changed_files.md` - this file
- `daily.md` - appended session log line

---

## 2026-05-28 - Final proportional polish

**Modified:**
- `index.html` - widened desktop content, slightly increased desktop text/nav sizing, and strengthened footer grounding
- `pgwp.html` - widened desktop content, slightly increased desktop text/nav sizing, and strengthened footer grounding
- `sin.html` - widened desktop content, slightly increased desktop text/nav sizing, and strengthened footer grounding
- `memory/current_state.md` - recorded latest proportional polish pass
- `memory/next_prompt.md` - updated next-session handoff
- `memory/changed_files.md` - recorded files changed in this task
- `daily.md` - appended concise session log line

---

## 2026-05-28 - Site legitimacy pass

**Modified:**
- `index.html` - added simple site footer and homepage last-reviewed line
- `pgwp.html` - added simple site footer
- `sin.html` - added simple site footer
- `memory/current_state.md` - recorded latest legitimacy pass
- `memory/next_prompt.md` - updated next-session handoff
- `memory/changed_files.md` - recorded files changed in this task
- `daily.md` - appended concise session log line

---

## 2026-05-28 - Layout-density polish

**Modified:**
- `index.html` - widened desktop content container and tightened homepage header rhythm
- `pgwp.html` - widened desktop content container and tightened major section/callout spacing
- `sin.html` - widened desktop content container and tightened major section/callout spacing
- `memory/current_state.md` - recorded live domain and latest density pass
- `memory/next_prompt.md` - updated next-session handoff
- `memory/changed_files.md` - recorded files changed in this task
- `daily.md` - appended concise session log line

---

## 2026-05-27 � Trust polish

**Modified:**
- `index.html` � removed Google Fonts link, switched to local/system font stack, muted teal values
- `pgwp.html` � removed Google Fonts link, switched to local/system font stack, muted teal values
- `sin.html` � removed Google Fonts link, switched to local/system font stack, muted teal values
- `memory/current_state.md` � recorded trust-polish pass
- `memory/next_prompt.md` � added latest handoff note
- `memory/changed_files.md` � recorded files changed in this task
- `daily.md` � appended concise session log line

---


## 2026-05-27 — Founder note fix (090af0e)

**Modified:**
- `sin.html` — founder note updated to match pgwp.html and index.html (was missed in earlier pass)

---

## 2026-05-27 — Guide workflow connections (f373ebb)

**Modified:**
- `pgwp.html` — added "Next step" transition card linking to /sin.html before disclaimer
- `sin.html` — added "More guides coming" card before disclaimer
- `index.html` — added category labels (Study & Graduation / Working in Canada) above guide cards

---

## 2026-05-27 — Shared agent workflow

**Modified:**
- `canadasteps/CLAUDE.md`
- `canadasteps/AGENTS.md`
- `canadasteps/memory/current_state.md`
- `canadasteps/memory/next_prompt.md`
- `canadasteps/memory/changed_files.md`
- `canadasteps/daily.md`

---

## 2026-05-25 — Initial scaffold

**Created:**
- `canadasteps/CLAUDE.md`
- `canadasteps/README.md`
- `canadasteps/AGENTS.md`
- `canadasteps/.gitignore`
- `canadasteps/requirements.md`
- `canadasteps/design.md`
- `canadasteps/roadmap.md`
- `canadasteps/risks.md`
- `canadasteps/implementation_plan.md`
- `canadasteps/daily.md`
- `canadasteps/docs/editorial-rulebook.md`
- `canadasteps/docs/project-status.md`
- `canadasteps/docs/sources-log/` (empty directory)
- `canadasteps/pages/pgwp.html`
- `canadasteps/assets/` (empty directory)
- `canadasteps/scripts/` (empty directory)
- `canadasteps/memory/current_state.md`
- `canadasteps/memory/next_prompt.md`
- `canadasteps/memory/changed_files.md`
- `canadasteps/memory/risks.md`
- `canadasteps/memory/known_failures.md`
- `canadasteps/memory/rejected_approaches.md`

**Modified:** None (first session)
