# CanadaSteps — Editorial Rulebook

> Authoritative guide for all content written or reviewed on canadasteps.org.  
> When in doubt, default to clarity over completeness.

---

## 1. Mission and voice

CanadaSteps explains Canadian immigration steps in plain language. The voice is:

- **Calm and factual** — not promotional, not alarmist
- **Direct** — use "you" to address the reader
- **Neutral** — no opinions on IRCC decisions or policy
- **Empathetic** — acknowledge that immigration is stressful; never condescending

Avoid: jargon, acronyms without expansion, immigration-lawyer hedging, or bureaucratic passive voice.

---

## 2. Reading level

Target Grade 8 (Flesch-Kincaid ≤ 60). Practical rules:

- Sentences: 20 words or fewer on average
- Paragraphs: 3–4 sentences max
- Prefer common words ("start" over "commence", "need" over "require")
- Define every acronym on first use: "Post-Graduation Work Permit (PGWP)"

---

## 3. Accuracy and sourcing

### 3.1 One claim, one source

Every factual claim that is not common knowledge must be traceable to one official URL. Acceptable sources:

| Source | Domain |
|--------|--------|
| IRCC program pages | ircc.canada.ca |
| Canada.ca guides | canada.ca |
| Official regulations | laws-lois.justice.gc.ca |
| IRCC processing times | ircc.canada.ca/english/information/times |

Do not cite: immigration law firm blogs, Reddit, news articles, or unofficial calculators.

### 3.2 Source log

For each page, maintain a corresponding file in `docs/sources-log/<page-slug>.md` with:

```
| Claim | Source URL | Date verified |
|-------|-----------|---------------|
| PGWP validity matches study permit length | https://... | 2026-05-01 |
```

### 3.3 Fees and processing times

- **Never paraphrase fee amounts.** Quote the official figure verbatim and link directly.
- **Processing times change frequently.** Always link to the live IRCC processing times tool rather than stating a number of weeks.
- Add the note: *Processing times change frequently. Check the [IRCC tool](https://ircc.canada.ca/english/information/times/) for the current estimate.*

### 3.4 Date handling

Do not stamp pages with a publication date. Instead, use inline attribution:

> "As of [Month Year] per IRCC, applicants must…"

When information becomes outdated, add a visible notice at the top of the affected section:

> **Notice:** This section may be outdated. IRCC updated its policy in [Month Year]. We are reviewing this page.

Never silently remove information that may still apply to in-progress applications.

---

## 4. Legal disclaimer

CanadaSteps is **not a law firm** and does not provide legal advice.

- Replace "you should" / "you must" with "applicants typically" / "IRCC requires"
- End every page with the standard disclaimer block (see Section 8)
- Never tell a reader their specific application will succeed or fail

---

## 5. Page structure

Every content page follows this structure:

```
1. Page title (H1) — plain-language name of the permit or step
2. One-sentence summary — what this page covers
3. Who this applies to — eligibility in 2–3 bullet points
4. Step-by-step section (H2 per major step)
5. Common questions (FAQ, optional)
6. Related pages (links)
7. Disclaimer block
```

### H1 / H2 / H3 rules

- H1: one per page, matches the page `<title>`
- H2: major steps or sections only
- H3: sub-steps or sub-sections within an H2
- No H4 or deeper — restructure instead

---

## 6. Links

- Always use descriptive link text: "IRCC PGWP guide" not "click here"
- External links (canada.ca, ircc.canada.ca) open in a new tab (`target="_blank" rel="noopener"`)
- Internal links use relative paths: `../pages/express-entry.html`
- Check all links before publishing; broken links erode trust

---

## 7. Images and media

- Every image needs an `alt` attribute with a meaningful description
- Do not use stock photos of people — they can misrepresent the audience
- Infographics must include a text equivalent (table or list) for accessibility
- No autoplay audio or video

---

## 8. Standard disclaimer block

Paste verbatim at the bottom of every page:

```html
<aside class="disclaimer">
  <p><strong>Not legal advice.</strong> CanadaSteps provides general information 
  about Canadian immigration programs. Every situation is different. For advice 
  about your specific case, consult a licensed immigration consultant (RCIC) or 
  immigration lawyer.</p>
</aside>
```

---

## 9. Content review checklist

Before any page is published or updated, confirm:

- [ ] All claims traced to an official source in the source log
- [ ] Fees linked directly, not paraphrased
- [ ] Processing times linked to the live IRCC tool, not stated as a fixed number
- [ ] Reading level checked (aim for Grade 8)
- [ ] No legal advice language ("you should", "you will")
- [ ] Disclaimer block present
- [ ] All external links open in a new tab
- [ ] All images have alt text
- [ ] Source log file updated for this page

---

## 10. Change log

| Date | Change | Author |
|------|--------|--------|
| 2026-05-25 | Initial rulebook created | CanadaSteps team |
