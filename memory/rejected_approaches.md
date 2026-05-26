# Rejected Approaches

_Features and approaches explicitly decided against, with rationale. Prevents relitigating settled decisions._

---

## Architecture

| Rejected | Why | When reconsidered |
|----------|-----|------------------|
| WordPress / any CMS | Operational overhead not justified at <25 pages | At 25+ pages with 2+ contributors |
| React / Vue / Next.js | Application framework for a content site; no justified complexity | Never for content-only pages |
| Static site generator (Hugo, Eleventy) | Premature at <25 pages | At 25+ pages when HTML editing is the bottleneck |
| Backend server / database | Zero functional need for a content site | Only if user accounts become justified |
| Docker / Kubernetes | Complete overkill | Never for this project |
| Redis / message queues | Not applicable | Never |

## Features

| Rejected | Why | When reconsidered |
|----------|-----|------------------|
| AI chatbot / Q&A | Hallucination risk on immigration law is actively harmful | Never without expert human review loop |
| Points calculator / eligibility tool | IRCC formula changes; we'd maintain a wrong tool | Phase 3, only if IRCC API exists |
| Newsletter / email capture | CASL + PIPEDA compliance overhead before we have readers | Phase 3, only with confirmed demand |
| User accounts / login | Zero functional need | Only if personalization becomes justified |
| Comments / community features | Moderation burden, misinformation risk | Phase 3+ with explicit moderation plan |
| Consultant directory | Vetting burden, complaint exposure | Never without dedicated editorial process |
| Google Analytics | Privacy concern for immigration audience | Use Plausible (aggregate, no cookies) if needed |
| Social share buttons | Third-party tracking scripts; users can share a URL | Never |
| Advertising | Editorial conflict risk | Never unless structurally separated and minimal |
