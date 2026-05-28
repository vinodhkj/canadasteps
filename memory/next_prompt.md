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

Current state:
- Top nav uses: All Guides, First Weeks, Money & Taxes, Study & Immigration (anchors to homepage sections)
- Homepage structured into 3 sections: First Weeks in Canada / Money & Taxes / Study & Immigration
- First Weeks: SIN, Bank Account, Ontario Driver's License, Phone Plan, Ontario Photo Card
- Money & Taxes: Tax Filing, CRA My Account
- Study & Immigration: PGWP
- Ontario Driver's License is in First Weeks section (not Daily Life)
- Subtle maple-leaf SVG is part of the CanadaSteps logo
- Visual comfort pass uses warmer neutrals, softer cards, and subtle category accents
- Phase 1 refinement polish is in place: homepage editorial entries have metadata and subtle hover hierarchy; homepage anchors use scroll-margin-top; homepage and PGWP desktop measure is slightly wider; PGWP visual surfaces are softened through reusable CSS without content rewrites.

Do not touch unless explicitly requested:
- CSP, HSTS, DMARC, DKIM, DNSSEC, security.txt
- analytics, forms, backend setup
- PGWP guide content
- agent workflow/memory format

Next priority:
- Review the Phase 1 polish after deployment, especially homepage anchor landing, mobile guide-entry rhythm, and PGWP section density.
- Continue content expansion only from user-validated priorities.
---
