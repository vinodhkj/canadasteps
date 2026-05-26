# CanadaSteps — Design Decisions

## Architecture: static HTML, no framework

**Decision:** Plain HTML + CSS. No React, no Vue, no static site generator for now.

**Why:** The site is content, not an application. Five pages of HTML have zero build complexity, zero dependency rot, and open in any browser from the filesystem. The day this becomes painful to maintain is the day we evaluate Eleventy or Hugo — not before.

**Upgrade trigger:** More than 25 pages OR a second regular contributor who cannot comfortably edit raw HTML.

---

## Hosting: GitHub Pages or Netlify free tier

**Decision:** Deploy from the main branch via GitHub Pages or Netlify free tier.

**Why:** $0/month, automatic SSL, CDN-backed, survives a traffic spike from a Reddit post without intervention. No server to patch.

**What we're not doing:** VPS, Nginx, Docker, AWS. The operational overhead is not justified.

---

## No CMS

**Decision:** Content lives as HTML files in the repository.

**Why:** A CMS adds: a hosting dependency, an admin interface to secure, a database to back up, plugin update cycles, and onboarding complexity. With 5–25 pages, Git is the CMS.

**What we lose:** Non-technical editors cannot contribute without learning Git. Acceptable at this scale.

---

## No JavaScript (for core content)

**Decision:** Pages must be fully usable with JavaScript disabled.

**Why:** Our users are on a wide range of devices and network conditions. Immigration guidance is too important to gate behind a script that fails silently. JS may be added later for non-critical UI enhancements only.

---

## No analytics with personal tracking

**Decision:** No Google Analytics, no Meta Pixel, no session recording in MVP.

**Why:** Our audience includes visa applicants who have legitimate reasons to be privacy-conscious about browsing immigration sites. We will not collect data we don't need.

**What we can use:** Server-level log analysis (Netlify analytics, self-hosted Plausible) if we need aggregate page view data later. Opt-in only, aggregate only.

---

## URL structure

Pattern: `canadasteps.org/pgwp`, `canadasteps.org/express-entry`

**Why:** Short, shareable, no file extension visible. Map via Netlify redirects or GitHub Pages permalink config.

**File naming:** `pages/pgwp.html` maps to `/pgwp`.

---

## No versioning of content pages (yet)

**Decision:** Git history is the version history.

**Why:** Displaying "last updated" dates on pages is useful, but "version 1.3" of a content page is meaningless to users. We use inline date attribution ("as of May 2026 per IRCC") for time-sensitive claims. Full version history is in `git log`.

---

## Rejected design options

| Option | Rejected because |
|--------|-----------------|
| WordPress | CMS overhead, plugin updates, PHP hosting required, overkill |
| Next.js / React | Application framework for a content site; unnecessary build complexity |
| Notion-to-web export | Vendor lock-in, limited control over HTML structure and SEO |
| Ghost | Paid tiers, newsletter-first, not designed for reference content |
| Webflow | Monthly cost, vendor lock-in, export limitations |
