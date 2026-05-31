---
CanadaSteps session handoff — updated 2026-05-31 (corrective homepage pass)

PENDING USER APPROVAL: Corrective homepage redesign implemented but NOT committed.

Files changed since last commit (025136e):
- canadasteps/index.html — full structural rewrite to match Claude Design Direction B (slim topbar, single-row nav, two-column hero, 4-col metrics strip, 3-col card grid, dark navy footer)

Committed (025136e — do not re-do):
- pgwp.html — Inter removed, scope-module, toned boxes, outlined step-nums, route-cards
- CanadaSteps-Implementation-Brief.md — at repo root
- memory files

---
CanadaSteps session handoff

Current workflow:
- Local -> GitHub -> Cloudflare Pages -> canadasteps.ca
- Cloudflare Pages auto-deploys after git push to main
- Netlify is not part of the active workflow

Current pages:
- pr-pathways.html
- index.html
- pgwp.html
- spouse-work-permit.html
- sin.html
- taxes.html
- cra-account.html
- bank-account.html
- gic-unlock.html
- ontario-drivers-license.html
- phone-plan.html
- ontario-photo-card.html

Current layout state (as of May 30):
- All pages use centered outer frame (margin: 0 auto) with left-aligned content inside
- Homepage (.page-banner-inner + .page-wrap): max-width 1100px, margin: 0 auto
- Guide pages (.page-wrap): max-width 1000px, margin: 0 auto
- Mobile (≤600px): full-width naturally; padding handles edge spacing. Sticky nav bar utilizes horizontal scrolling badges (`overflow-x: auto`) for compact, single-row height, preventing vertical layout clogging.
- Tables (like the cost table in pgwp.html) support horizontal scrolling (`overflow-x: auto`) on narrow viewports instead of clipping.
- .site-footer-inner: margin: 0 auto on all pages (unchanged)
- Nav and topbar remain full-width on all pages
- Left-rail clamp system was tried and reverted — do not reintroduce without explicit request

Current editorial system:
- Design philosophy: "GOV.UK, not Stripe" — quiet public-reference handbook
- Font stack: system fonts only (no Inter, no web fonts)
- Hover on guide entries: background + border shift only, no slide transform
- Disclaimer block: no border-radius (flush editorial notice)
- "Last reviewed" date: body color, no monospace, month/year only
- Newcomer orientation line above first section on homepage
- Section accent borders: teal (First Weeks), amber (Money & Taxes), navy (Study & Immigration)

Do not touch unless explicitly requested:
- CSP, HSTS, DMARC, DKIM, DNSSEC, security.txt
- analytics, forms, backend setup
- PGWP guide content (frozen)
- agent workflow/memory format
- .site-footer-inner margin (stays centered)

Analytics next steps (after deploy):
- Open GA4 → Reports → Realtime — confirm hits are coming in
- Check Cloudflare Web Analytics / Core Web Vitals — confirm performance remains green
- Measurement ID: G-4M1LTVRG81

SEO next steps (after deploy):
- Verify https://canadasteps.ca/sitemap.xml shows XML in browser
- Verify https://canadasteps.ca/robots.txt loads correctly
- Submit sitemap.xml in Google Search Console

UI redesign work with Claude Design is ongoing — keep separate from SEO commit.

Content expansion only from user-validated priorities.
---
