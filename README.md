# CanadaSteps

Plain-language guidance for newcomers to Canada. No backend. No accounts. No fluff.

**Site:** canadasteps.org  
**Status:** Early MVP — first pages in development

---

## What this is

A static HTML website that explains Canadian immigration steps clearly, accurately, and in plain English (Grade 8 reading level). Every claim is sourced to an official government URL. No legal advice. No consultant referrals. No commercial agenda.

## What this is not

- A law firm or immigration consultant
- A replacement for Canada.ca
- A calculator, chatbot, or AI product
- A community or forum

---

## Local setup

No build step required. Open any `.html` file directly in a browser, or serve locally:

```bash
# Python (built-in, no install)
python -m http.server 8080
# then open http://localhost:8080/pages/pgwp.html
```

## Project structure

```
canadasteps/
├── README.md                  ← you are here
├── CLAUDE.md                  ← context for AI assistants
├── AGENTS.md                  ← editorial advisory roles
├── .gitignore
├── requirements.md            ← what we're building and constraints
├── design.md                  ← design decisions and rationale
├── roadmap.md                 ← phased plan
├── risks.md                   ← known risks and mitigations
├── implementation_plan.md     ← current execution plan
├── daily.md                   ← session log
├── memory/                    ← session state and handover notes
├── docs/
│   ├── editorial-rulebook.md  ← editorial standards
│   ├── project-status.md      ← sprint tracker
│   └── sources-log/           ← per-page source citations
├── pages/                     ← HTML content pages
├── assets/                    ← CSS, images, JS
└── scripts/                   ← tooling scripts (link checker, etc.)
```

## Contributing

1. Read `docs/editorial-rulebook.md` before writing anything
2. Every factual claim needs a source in `docs/sources-log/<page-slug>.md`
3. Run through the publish checklist in the rulebook before any page ships
4. Update `docs/project-status.md` when a task closes

## Content principles

- One claim = one official source
- Never paraphrase fee amounts — quote and link directly
- Processing times: always link to the live IRCC tool, never state a number
- Grade 8 reading level or below
- Disclaimer block on every page
