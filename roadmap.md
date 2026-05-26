# CanadaSteps — Roadmap

Phases are milestone-gated, not time-gated. Do not move to the next phase until the current one's goal is confirmed.

---

## Phase 0 — Foundation (current)

**Goal:** Infrastructure ready. One page live. Editorial process proven.

**Gate:** pgwp.html published, source-verified, passes full editorial checklist, accessible via real URL.

### Tasks

- [x] Project folder structure created
- [x] CLAUDE.md written
- [x] Editorial rulebook written
- [x] README, AGENTS.md, design.md, risks.md, roadmap.md created
- [ ] Git repository initialized and first commit made
- [ ] Hosting configured (GitHub Pages or Netlify)
- [ ] Domain connected (canadasteps.org)
- [ ] pgwp.html content completed and source-verified
- [ ] sources-log/pgwp.md created
- [ ] Base CSS stylesheet (assets/style.css)
- [ ] pgwp.html passes full editorial checklist

---

## Phase 1 — Core pages (5 pages)

**Goal:** Cover the five highest-search-volume topics for newcomers. Get indexed. Get a real reader.

**Gate:** 5 pages live, all source-verified, at least one reader found organically or via sharing.

### Topics (priority order)

1. PGWP (Post-Graduation Work Permit)
2. Express Entry overview
3. PR card — first-time application
4. Study permit — how to apply
5. Spousal sponsorship overview

### Tasks

- [ ] Content drafted for all five pages
- [ ] All five pages pass editorial checklist
- [ ] Source logs complete for all five pages
- [ ] All internal links working
- [ ] Google Search Console verified
- [ ] Pages indexed

---

## Phase 2 — Depth and discovery

**Goal:** Add depth pages, improve navigation, gather first real feedback.

**Gate:** At least 100 unique monthly readers. At least 3 pieces of direct user feedback received.

### Possible additions (validate demand first)

- PR card renewal
- Work permit extensions (LMIA, ICT, etc.)
- Permanent Residency pathways comparison
- IRCC account setup guide
- Settlement resources by province
- Common application mistakes (listicle format)

### Infrastructure (only if needed)

- Sitemap.xml
- robots.txt
- Basic navigation component
- Search (browser find-in-page is fine; on-site search is a Phase 3 discussion)

---

## Phase 3 — Sustainability (do not plan yet)

**Prerequisite:** Real evidence of reader demand and content maintenance working at scale.

**Possible directions (choose one, not all):**

- Static site generator (Eleventy) if HTML editing is the bottleneck
- Plausible Analytics for aggregate page view data
- Donation model (Open Collective or Ko-fi)
- Grant funding from settlement organizations
- Lightweight RCIC referral program (only if fully transparent and editorially separated)

**Things that require a separate decision with full analysis:**

- Newsletter / email list (CASL, PIPEDA compliance)
- User accounts
- Interactive tools (calculators, eligibility checkers)
- Community features

---

## What is permanently out of scope

- AI chatbot on immigration topics
- Legal advice or case review
- Consultant marketplace
- Immigration news / reactive content chasing
- Anything that requires a backend server in Phase 0–1
