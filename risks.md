# CanadaSteps — Risk Register

Format: **Risk** → Likelihood · Impact → Mitigation

---

## Editorial / Content risks

### R1 — Content rot
**Risk:** A page goes stale after an IRCC policy change. A reader acts on outdated information.  
**Likelihood:** High (IRCC publishes policy changes 10–20x/year)  
**Impact:** Critical — harms user, damages site credibility  
**Mitigation:**  
- Source log dates enable systematic review
- Subscribe to IRCC RSS feed and immigration news alerts
- Visible "Notice" banner for any page known to be under review
- Never silently remove outdated content — flag it first

### R2 — Fee amount inaccuracy
**Risk:** A quoted fee amount changes; user prepares wrong payment.  
**Likelihood:** Medium (fees update annually, sometimes mid-year)  
**Impact:** High  
**Mitigation:** Never paraphrase fees — always quote and link directly to the source page. Link displays are evergreen even when amounts change.

### R3 — Inadvertent legal advice
**Risk:** Phrasing crosses from guidance into advice ("you should apply before X date").  
**Likelihood:** Medium  
**Impact:** High — legal exposure, reader misplaced reliance  
**Mitigation:** Editorial rulebook language rules. Reviewer agent checklist. Standard disclaimer on every page.

---

## Operational risks

### R4 — Single maintainer bottleneck
**Risk:** One person maintains all content. Illness, unavailability = site rots.  
**Likelihood:** Medium  
**Impact:** Medium  
**Mitigation:** All content is in Git, structure is documented. A second contributor could onboard from the rulebook. No proprietary CMS lock-in.

### R5 — Hosting failure / domain expiry
**Risk:** GitHub Pages goes down or domain lapses.  
**Likelihood:** Low  
**Impact:** High (full site offline)  
**Mitigation:** Use a reliable free host (Netlify/GitHub Pages have 99.9%+ uptime). Set domain renewal reminders 60 days in advance. No server to manage = no server to fail.

### R6 — Link rot in source log
**Risk:** Official canada.ca URLs change, breaking our source citations.  
**Likelihood:** Medium (government URLs do move)  
**Impact:** Medium — we lose evidence trail, may be linking to wrong page  
**Mitigation:** Periodic link audit via script. Web Archive fallback for defunct URLs.

---

## Strategic risks

### R7 — SEO invisibility at launch
**Risk:** New domain ranks nowhere for any meaningful query for 6–12 months.  
**Likelihood:** High  
**Impact:** Medium — no organic traffic, no feedback loop  
**Mitigation:** Don't rely on SEO for initial distribution. Use direct sharing (Reddit comments, settlement org partnerships, newcomer communities). SEO is a Phase 2 benefit, not Phase 0 strategy.

### R8 — Scope creep disguised as user need
**Risk:** Features are added before a real need is confirmed (calculator, chatbot, newsletter).  
**Likelihood:** High  
**Impact:** Medium — wasted effort, complexity, maintenance burden  
**Mitigation:** Scope Guard agent review for any new feature. Default answer is "not yet." See `memory/rejected_approaches.md`.

### R9 — Monetization pressure compromises editorial integrity
**Risk:** Pressure to generate revenue leads to consultant referral links or sponsored content that conflicts with accuracy/neutrality.  
**Likelihood:** Low (near-term)  
**Impact:** Critical — site loses its only differentiator (trust)  
**Mitigation:** No monetization in Phase 0–1. Any monetization in Phase 3+ must be structurally separated from editorial decisions and disclosed explicitly.

### R10 — IRCC improves its own UX
**Risk:** Canada.ca becomes genuinely usable, removing CanadaSteps's value proposition.  
**Likelihood:** Low  
**Impact:** High  
**Mitigation:** This is fine. The mission is served if IRCC gets better. In the meantime, the site helps real people.

---

## Risk summary table

| ID | Risk | Likelihood | Impact | Status |
|----|------|-----------|--------|--------|
| R1 | Content rot | High | Critical | Mitigated (process) |
| R2 | Fee inaccuracy | Medium | High | Mitigated (rulebook) |
| R3 | Inadvertent legal advice | Medium | High | Mitigated (rulebook) |
| R4 | Single maintainer | Medium | Medium | Accepted |
| R5 | Hosting / domain failure | Low | High | Mitigated (free tier) |
| R6 | Link rot | Medium | Medium | Partially mitigated |
| R7 | SEO invisibility | High | Medium | Accepted (distribution plan needed) |
| R8 | Scope creep | High | Medium | Mitigated (process) |
| R9 | Monetization pressure | Low | Critical | Deferred |
| R10 | IRCC self-improves | Low | High | Accepted |
