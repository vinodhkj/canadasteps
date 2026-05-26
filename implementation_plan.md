# CanadaSteps — Implementation Plan

Current phase: **Phase 0 — Foundation**

---

## Immediate next steps (ordered)

### Step 1 — Complete pgwp.html content

The PGWP page stub exists. It needs:

- [ ] Eligibility section completed with current DLI requirement source
- [ ] PGWP validity rules verified against current IRCC policy
- [ ] 180-day application window confirmed and sourced
- [ ] Fee amount (if applicable) quoted and linked
- [ ] Processing time section links to live IRCC tool
- [ ] All H2/H3 structure follows rulebook

**Acceptance:** Page passes the full editorial checklist in `docs/editorial-rulebook.md`.

---

### Step 2 — Create sources-log/pgwp.md

For each factual claim on pgwp.html, record:

```markdown
| Claim | Source URL | Date verified |
|-------|-----------|---------------|
| ... | https://... | 2026-05-25 |
```

---

### Step 3 — Create assets/style.css

Minimal stylesheet. Goals:
- Readable on mobile (max-width ~680px, comfortable line length)
- Clean typography (system font stack — no web font download)
- Visible disclaimer block styling
- No external CSS dependencies

No design framework. No utility classes. Just enough CSS to make text readable.

---

### Step 4 — Git init and first commit

```bash
cd canadasteps
git init
git add .
git commit -m "Initial scaffold: project structure, PGWP page, editorial rulebook, docs"
```

---

### Step 5 — Hosting setup

1. Create a GitHub repository (canadasteps-ca or canadasteps-org)
2. Push to main
3. Enable GitHub Pages from main branch
4. Configure custom domain (canadasteps.org) in GitHub Pages settings
5. Verify SSL is active

**Alternative:** Netlify drop — drag the folder to app.netlify.com for instant deploy without CLI setup.

---

### Step 6 — Verify launch checklist

- [ ] pgwp.html live at canadasteps.org/pgwp (or /pgwp.html until redirects configured)
- [ ] No broken links
- [ ] Disclaimer block visible
- [ ] Mobile layout acceptable
- [ ] Source log complete
- [ ] Google Search Console site verified

---

## What comes after Phase 0

See `roadmap.md`. Do not plan Phase 1 work until Step 6 above is complete.

---

## Technical decisions deferred

- Static site generator (evaluate at 25+ pages)
- Sitemap.xml and robots.txt (add in Phase 1 before submitting to Search Console)
- Navigation component (needed once there are 3+ pages)
- On-site search (Phase 3 at earliest)
