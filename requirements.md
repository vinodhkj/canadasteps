# CanadaSteps — Requirements

## Problem statement

Newcomers to Canada cannot effectively use official IRCC documentation. The result: avoidable mistakes, expensive consultants for simple questions, and high anxiety around what should be manageable processes.

CanadaSteps provides plain-language, source-verified guidance pages that remove that friction.

## User

**Primary:** International students, temporary workers, PR applicants, sponsored family members researching their own immigration situation.

**Profile:** Non-native English speaker, moderate digital literacy, high stakes (errors have real consequences), likely on mobile.

**NOT the user:** Immigration consultants, researchers, lawyers. They have better tools.

## Core functional requirements

### Must have (MVP)

- [ ] Static HTML pages — no backend, no JavaScript required for core function
- [ ] Each page covers one permit/pathway clearly
- [ ] All claims sourced to official government URLs
- [ ] Source log maintained per page
- [ ] Disclaimer block on every page
- [ ] Works on mobile (responsive, no horizontal scroll)
- [ ] Pages load in under 2 seconds on a 4G connection
- [ ] No user data collected (no analytics that track individuals)

### Must not have (MVP — explicitly out of scope)

- User accounts or login
- Newsletter or email capture
- Comments or community features
- AI chatbot or Q&A
- Points calculator or eligibility tool
- Consultant directory or referral links
- CMS or admin panel
- Backend server
- Database

## Non-functional requirements

- **Accuracy:** No claim without an official source. Outdated content flagged visibly, not silently removed.
- **Reading level:** Grade 8 or below (Flesch-Kincaid score ≥ 60).
- **Accessibility:** WCAG 2.1 AA minimum — alt text, semantic HTML, keyboard navigable.
- **Privacy:** No cookies, no tracking pixels, no third-party scripts in MVP.
- **Hosting cost:** $0/month on free tier (GitHub Pages or Netlify).
- **Maintenance:** Any single page must be updatable by one person in under 30 minutes.

## Constraints

- Content must never constitute legal advice
- Cannot imply affiliation with the Government of Canada or IRCC
- Must not accept advertising that could create editorial conflicts
- All external links must point to official government domains or the IRCC processing times tool

## Success criteria for MVP

1. Five pages published and source-verified
2. At least one real reader (not the author) navigates a page and finds it useful
3. Pages indexed by Google
4. Zero broken links at launch
5. All five pages pass the editorial rulebook checklist
