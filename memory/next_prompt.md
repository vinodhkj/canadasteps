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

Current state:
- Top nav uses category links: All Guides, Start Here, Money & Taxes, PGWP
- Homepage has a lightweight Start Here flow before guide cards for SIN, bank account, CRA My Account, taxes, and PGWP
- Homepage groups guides by Start Here, Money & Taxes, and Study & Graduation
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
