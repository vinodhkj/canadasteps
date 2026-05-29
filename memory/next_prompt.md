---
CanadaSteps session handoff

Current workflow:
- Local -> GitHub -> Cloudflare Pages -> canadasteps.ca
- Cloudflare Pages auto-deploys after git push to main
- Netlify is not part of the active workflow

Current pages:
- index.html
- pgwp.html
- sin.html
- taxes.html
- cra-account.html
- bank-account.html
- ontario-drivers-license.html
- phone-plan.html
- ontario-photo-card.html

Current layout state (as of May 29):
- All pages use centered outer frame (margin: 0 auto) with left-aligned content inside
- Homepage (.page-banner-inner + .page-wrap): max-width 1100px, margin: 0 auto
- Guide pages (.page-wrap): max-width 1000px, margin: 0 auto
- Mobile (≤600px): full-width naturally; padding handles edge spacing; no margin overrides needed
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

Next priority:
- User to review rail on live site after push
- Remaining consistency concern: guide pages do not have a .page-banner-inner equivalent (their page header lives inside .page-wrap). This is consistent enough — no action needed unless user raises it.
- Content expansion only from user-validated priorities.
---
