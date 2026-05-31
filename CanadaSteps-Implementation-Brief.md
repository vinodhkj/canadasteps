# CanadaSteps Implementation Brief

## Approved Direction

Use **Direction B — Warm Resource Directory** as the homepage base.

Use **Direction A discipline** for the PGWP guide page.

This means:

* Homepage should feel warm, polished, card-based, and like a real public guide website.
* PGWP should feel disciplined, text-first, calm, and easier to scan.
* Avoid the old narrow document/list layout.
* Avoid loud warning boxes.
* Avoid generic AI-template styling.
* Keep everything static HTML/CSS only.

## Scope

Edit only:

* `index.html`
* `pgwp.html`
* relevant memory files:

  * `memory/current_state.md`
  * `memory/next_prompt.md`
  * `memory/changed_files.md`
  * `daily.md`

Do not edit:

* other public HTML pages
* `sitemap.xml`
* `robots.txt`
* draft/internal pages
* hosting/deployment config
* all-page navigation rollout
* global CSS extraction

## Must Preserve

Preserve exactly or semantically:

* GA4 script tag in the `<head>` of both pages
* page status/source strip concept
* topbar message
* founder-note text
* official source links
* disclaimer language
* PGWP Step 5 dual route logic:

  * IMM 5710 = inside-Canada default route
  * IMM 1295 = outside-Canada alternative route
* Adobe Acrobat / form validation caution
* "What SettleWise does not determine" safety/scope content
* mobile horizontal-scroll nav concept
* scrollable fees/cost table
* no left-rail clamp system

## Homepage Design: Direction B Warm Resource Directory

Goal:
Make the homepage look like a polished public guide/resource directory, not a narrow document list.

Use:

* warm cream background
* clean top navigation
* stronger hero area
* visible search/browse module if practical
* clear guide categories
* card-based guide discovery
* muted olive/clay/slate accents
* comfortable spacing
* strong but calm typography
* mobile-friendly card rhythm

Homepage sections:

* Hero:

  * Title should feel more premium and welcoming.
  * Keep meaning: practical newcomer guides, official sources, independent/not IRCC.
* Status metrics:

  * May 2026
  * 11 guides
  * official sources
  * independent/not IRCC
* Guide categories:

  * Just Arrived
  * Work & Life
  * Graduation & Immigration
  * PR Pathways
* Guide entries:

  * Turn current flat rows into refined cards or card-like panels.
  * Keep guide names, descriptions, and links.
  * Add subtle category tags/metadata if useful.
  * Use borders and spacing, not heavy shadows.
  * Avoid too many decorative effects.

## PGWP Design: Direction A Discipline

Goal:
Make PGWP less overloaded and easier to scan.

Use:

* text-first guide structure
* lighter manual-style step numbers
* hairline dividers
* compact metadata
* disciplined section hierarchy
* fewer loud colored boxes
* calm official-source treatment
* strong scan flow

PGWP page structure should visually support:

1. Header and summary
2. Page status/source strip
3. Scope/safety module
4. Who this applies to / may not apply to
5. Before you start checklist
6. Fees/cost table
7. Application steps
8. Step 5 IMM 5710 / IMM 1295 routing
9. Adobe Acrobat validation caution
10. Commonly missed items
11. Official links
12. After you apply
13. Disclaimer/footer

## PGWP Safety/Scope Module

Restyle "What SettleWise does not determine" as a calm scope/trust module.

Do not make it a loud red warning box.

Use:

* soft background
* thin burgundy/oxblood left rule
* calm heading
* readable bullets
* less visual weight than the main page header

Do not remove the safety content.

## PGWP Step 5 Route Cards

Make the IMM route split easy to scan.

Desktop:

* side-by-side or clean two-column treatment if space allows
* inside Canada card:

  * IMM 5710
  * default route
  * navy/serious accent
* outside Canada card:

  * IMM 1295
  * alternative route
  * gray/slate accent

Mobile:

* stacked cards
* comfortable touch spacing
* no clipping

Keep the wording cautious:
Users should follow the document checklist generated in their IRCC account.

## Navigation

Improve top navigation discoverability without crowding the header.

Use grouped nav:

* All Guides → `index.html`
* First Weeks → `index.html#just-arrived`
* Work & Life → `index.html#working-daily-life`
* Graduation → `index.html#graduation-immigration`
* PR → `pr-pathways.html`

Mobile:

* single-row horizontal-scroll nav is acceptable
* tap targets must be comfortable
* avoid multi-row nav clogging the viewport

## Styling Direction

Use performance-safe fonts and CSS only.

Suggested palette:

* background: warm cream / off-white
* card surface: slightly lighter cream
* primary text: deep navy/slate
* muted text: slate gray
* accent green/olive for guide/source confidence
* clay/ochre accents for metadata
* restrained burgundy only for scope/safety boundaries

Do not rely on Georgia/basic cards if it makes the site feel like the old version. If using system fonts, create the new identity through spacing, hierarchy, card rhythm, nav treatment, and metadata styling.

## Responsive Requirements

Test at:

* desktop width
* tablet-ish width
* mobile width around 320px

Confirm:

* no horizontal page overflow
* mobile nav scrolls horizontally and does not wrap
* cost table scrolls horizontally and does not clip
* route cards stack correctly
* footer links remain usable
* page remains readable without zooming

## Before Editing

After creating this brief file:

1. Re-read:

   * `memory/current_state.md`
   * `memory/next_prompt.md`
   * `memory/changed_files.md`
   * `daily.md`
   * `settlewise-editorial-rulebook.md`
   * `CanadaSteps-Implementation-Brief.md`
2. Inspect current `index.html` and `pgwp.html`.
3. Summarize the implementation plan.
4. Flag risks before coding.

## After Editing

Show:

1. Changed files
2. Key diffs for `index.html` and `pgwp.html`
3. Confirmation that GA4 tag remains in both pages
4. Confirmation that PGWP Step 5 IMM 5710 / IMM 1295 logic remains
5. Confirmation that Adobe Acrobat validation caution remains
6. Confirmation that mobile nav and cost table still work
7. Memory file updates
8. Unresolved risks

Do not commit until I approve.
