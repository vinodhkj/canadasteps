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

Current state:
- Top nav uses: All Guides, First Weeks, Money & Taxes, Study & Immigration (anchors to homepage sections)
- Homepage structured into 3 sections: First Weeks in Canada / Money & Taxes / Study & Immigration
- First Weeks: SIN, Bank Account, Ontario Driver's License
- Money & Taxes: Tax Filing, CRA My Account
- Study & Immigration: PGWP
- Ontario Driver's License is in First Weeks section (not Daily Life)
- Subtle maple-leaf SVG is part of the CanadaSteps logo
- Visual comfort pass uses warmer neutrals, softer cards, and subtle category accents

Do not touch unless explicitly requested:
- CSP, HSTS, DMARC, DKIM, DNSSEC, security.txt
- analytics, forms, backend setup
- PGWP guide content
- agent workflow/memory format

Next priority:
- Push local commits to GitHub and verify Cloudflare Pages deployment.
- Then continue content expansion only from user-validated priorities.
---
