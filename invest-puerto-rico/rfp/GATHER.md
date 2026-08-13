# GATHER.md — Information-Gathering Guide for the InvestPR RFP Proposal

**Purpose:** This file is an operating guide for an agent (you) conducting a structured interview with a human to collect everything needed to complete `rfp/PROPOSAL.md`. Every gap in that file is tagged `[G-##: description]`. Your job is to resolve every tag with real, submission-quality information, then update PROPOSAL.md in place.

**Context you need first:** Read `rfp/IPR-RFP-CRM-Architecture-Systems-Integration-Ops-Support_FINAL.md` (the RFP) and `rfp/PROPOSAL.md` (the skeleton) before starting.

---

## Hard Constraints (do not let these slip)

| Constraint | Detail |
| :--- | :--- |
| **Questions deadline** | Fri, Aug 14, 2026 — if the human has clarifying questions for InvestPR, they must be emailed to talmodovar@investpr.org before this date. **Ask about this FIRST — it is the most time-sensitive item.** |
| **Submission deadline** | Fri, Aug 28, 2026, 6:00 PM AST |
| **Format** | PDF, emailed to talmodovar@investpr.org, subject: `RFP Response - CRM Architecture Systems Integration & Ops Support` |
| **Required attachments** | Resumes for EVERY assigned professional; ≥2 client references; ≥3 professional references; conflict-of-interest statement (explicit even if none) |
| **Engagement term** | Sept 14, 2026 → June 30, 2027, option to renew |

## What Wins (use this to prioritize effort)

Evaluation weights: **50%** ability/capacity to perform, **20%** cost reasonability & clarity, **20%** examples of work product, **10%** references.

Implications for how you gather:
- Spend the most interview time on **team, experience, and technical approach** (the 50%).
- **Work samples are worth as much as price.** Push hard for real, sanitized artifacts (integration maps, SOPs, training decks) — the RFP names these explicitly.
- Quantified case-study results beat adjectives. Always ask "what's the number?"
- Pricing needs to be *clear and itemized* more than merely cheap.

---

## How to Run the Session

1. Work through the sections below **in order** (they're sequenced so early answers inform later ones).
2. For each item: ask the question, capture the answer, and immediately write it into `PROPOSAL.md`, replacing the `[G-##]` token. Keep answers in the proposal's voice (confident, specific, first-person plural).
3. If the human doesn't know an answer, record it in a **"Open Items"** list at the bottom of this file with an owner and due date — don't stall the session.
4. If an answer is weak relative to the evaluation criteria (e.g., a case study with no numbers), say so and coach for a stronger version before moving on.
5. Track progress with the checklist boxes below.
6. When every token is resolved, run the **Final QA** section at the end.

---

## Session 0 — Urgent Triage (do this first)

- [x] **Q0.1:** ~~Questions to InvestPR before Aug 14?~~ **DECIDED Aug 12, 2026: No questions round.** Operator's call — no time for a back-and-forth before submission. Consequence: we self-answer the open scope variables (support volume, user count, current-state documentation, record/platform counts) by writing them as **explicit stated assumptions** in the proposal, especially in §F Budget. Every place we would have asked a question becomes a visible assumption line the evaluator can price against. Note: InvestPR shares all vendor Q&A responses on Aug 19 — check for that email and fold anything material into the draft before submitting.
- [ ] **Q0.2:** "Who is the internal owner of this proposal, and who signs it?" → feeds [G-04].
- [ ] **Q0.3:** InvestPR's stack has been inferred from public evidence (see `rfp/TECH-BRIEF.html`, "First, the headline"): **Salesforce CRM** (named in their own CRM Administrator job posting) + **HubSpot marketing** (hs-scripts on investpr.org) + Google/Meta/LinkedIn ad tags + GTM + Microsoft Clarity. Scheduling and outreach tools are unknown. Use this to pick the strongest certifications and case studies to foreground — but do NOT state platform assumptions in the proposal itself; the RFP discloses the official stack to finalists under NDA.

## Session 1 — Firm Identity (G-01, G-02, G-06 → G-09)

- [ ] **G-01:** Exact legal name of the firm.
- [ ] **G-06:** Corporate structure, jurisdiction of organization, year founded.
- [ ] **G-07:** Office location(s). *Probe: any Puerto Rico presence, PR-based staff, Spanish-language capability, or prior PR/LatAm client work? Any of these is a differentiator for a PR-based nonprofit — feature it.*
- [ ] **G-08:** Company background: founding story, headcount, growth, markets served. Ask for an existing boilerplate/capabilities deck to mine rather than making the human dictate.
- [ ] **G-09:** Core technical competencies. Cross-check against the RFP scope: data architecture, marketing automation, paid media/attribution, sales enablement tools, workflow automation, training. Flag any scope area the firm is thin on — that needs a partner/contractor story, not silence.
- [ ] **G-02:** Planned submission date (aim ≥2 business days before Aug 28).

## Session 2 — Experience & Case Studies (G-10 → G-14) — worth 20% directly, supports the 50%

- [ ] **G-10:** Experience summary: years doing CRM restructures/integrations, # of projects, platforms, industries. *Probe for nonprofit, government, or economic-development clients.*
- [x] **G-11 (partial):** Case Study 1 = Masterworks closed-loop marketing stack — drafted in PROPOSAL.md and as a full visual document, `rfp/CASE-STUDY-MASTERWORKS.html` (Aug 12). **Still open:** G-11c measurable results — the HTML doc marks every unverified figure with ◆ for Hai to confirm or replace; nothing ◆-marked may be copied into the proposal.
- [ ] **G-12 / G-13:** 1–2 more case studies. For each, insist on:
  - The client (or anonymized descriptor if under NDA),
  - The challenge in one or two sentences,
  - What the firm actually did (tools + tactics),
  - **A measurable result** — dedupe %, sync error reduction, attribution recovery, reporting time saved, lead-response time. If the human offers only qualitative outcomes, ask: "If we looked at the before/after dashboards, what number changed?"
  - Best-fit topics per the RFP: data normalization, system efficiency, campaign attribution.
- [ ] **G-14:** Work product samples for the appendix. Ask specifically for: one integration/architecture diagram, one SOP, one user manual or training deck, sanitized for confidentiality. *These are scored at 20% — treat "we don't have samples handy" as an open item with a deadline, not a no.*

## Session 3 — Technical Approach (G-15 → G-17)

- [ ] **G-15:** Review the placeholder five-phase methodology in PROPOSAL.md §C with the human. Ask: "Does this match how you'd actually run it? What would you change, rename, or re-sequence?" Capture their methodology name/branding if they have one.
- [ ] **G-16:** Tools & software actually used: data-quality/dedupe tools, iPaaS/integration platforms (e.g., middleware), documentation tools, PM stack, monitoring/alerting for sync failures.
- [ ] **G-17:** Support model: intake channel (email/ticketing/Slack), response-time SLAs by severity, who staffs it, escalation path, what the monthly support log looks like. *The RFP scores "technical support availability" — get concrete commitments.*

## Session 4 — Team (G-18 → G-25) — the core of the 50% criterion

- [ ] **G-18:** Org structure for this account (who reports to whom).
- [ ] **G-19 → G-23:** For each role (Engagement Lead, Technical/CRM Architect, Integration Specialist, Training Lead, others): name, area of responsibility, certifications (enterprise CRM platforms, martech, analytics).
- [ ] **G-24:** 100–150 word bio per person. Ask for existing bios/LinkedIn profiles to adapt.
- [ ] **G-39:** **Resumes for every named person — REQUIRED attachment.** Get the actual files or a firm commitment with a date.
- [ ] **G-25:** Capacity confirmation: "Can these exact people start Sept 14, 2026, and stay allocated through June 2027?" The RFP requires stating that qualified staff are *immediately available* — don't let this be aspirational.

## Session 5 — Timeline (G-26)

- [ ] **G-26:** Walk the placeholder schedule in PROPOSAL.md §E. Adjust phase durations to the firm's honest estimates. Confirm no holiday/staffing conflicts Sept–Dec 2026. Keep every RFP deliverable visibly mapped to a milestone date.

## Session 6 — Budget (G-27 → G-31) — worth 20%

- [ ] **G-27:** Pricing structure decision: fixed fee vs. hourly vs. retainer, and hybrid shape. *Recommend: fixed fee for implementation + flat monthly retainer for support — matches exactly what the RFP asks vendors to separate.*
- [ ] **G-28a–f:** One-time implementation pricing per line item (discovery, remediation, integrations, SOPs, training).
- [ ] **G-29a–e:** Monthly retainer amount and what it includes (hours? unlimited within scope?).
- [ ] **G-30:** Compute total: implementation + (retainer × months from start through June 30, 2027 — roughly 9.5 months). Verify the math yourself.
- [ ] **G-31:** Assumptions & exclusions: included hours, overage rates, change-order triggers, payment terms, whether travel/onsite work is included.
- [ ] Sanity check: "If InvestPR compares this line-by-line against two competitors, is anything unexplained or padded-looking?" Clarity is scored.

## Session 7 — References & Compliance (G-32 → G-38)

- [ ] **G-32 / G-33:** ≥2 client references for *similar CRM integration and data governance* work: org, contact name/title, email, phone, services provided. **Ask: "Have these contacts agreed to be listed and been warned they may be called?"**
- [ ] **G-34 / G-35 / G-36:** ≥3 professional references: name, relationship, contact info. (These are distinct from the client references.)
- [ ] **G-37:** Conflict of interest: ask explicitly about any board, staff, family, or financial ties to InvestPR or Puerto Rico government entities. If none → use the explicit "no conflicts" statement (required by the RFP even when none exist).
- [ ] **G-38:** Data-security practices statement; confirm willingness to sign an NDA (required for platform disclosure if shortlisted).
- [ ] **G-40 / G-41:** Collect appendix artifacts: work samples (from Session 2) and certification/partner credentials.

---

## Final QA (run when all tokens are resolved)

- [ ] Grep PROPOSAL.md for `[G-` — zero matches remain.
- [ ] Every RFP §5 requirement (A–G) has substantive content, not thin filler.
- [ ] Both reference minimums met: ≥2 client + ≥3 professional.
- [ ] Conflict-of-interest statement present and explicit.
- [ ] Resumes attached for every person named in §D.
- [ ] Budget separates one-time vs. monthly, states the pricing structure, and the arithmetic checks out.
- [ ] Timeline starts Sept 14, 2026 and covers through June 30, 2027.
- [ ] Case studies all contain at least one quantified result.
- [ ] Tone pass: confident, specific, no unexplained jargon, consistent "we."
- [ ] Export to PDF; confirm email recipient, subject line (`RFP Response - CRM Architecture Systems Integration & Ops Support`), and send before Fri, Aug 28, 2026, 6:00 PM AST.

## Open Items

*(Record anything the human couldn't answer during a session: item, G-## tag, owner, due date.)*

> **For Hai:** two items are assigned to you below — **G-06a** (confirm the exact registered entity name and state) and **G-11–13** (case studies with hard numbers, which are worth 20% of the score on their own and also feed the 50% criterion). The case studies are the higher-value of the two by a wide margin.

| G-## | Item | Owner | Due |
| :--- | :--- | :--- | :--- |
| G-06a | **→ HAI:** Verify exact registered entity name, LLC status, and WA formation date against the Secretary of State filing. Currently written as "Res AI, LLC, State of Washington" on Robby's recollection — needs confirmation before it goes on a signed proposal. | **Hai** | Aug 21 |
| G-11–13 | **→ HAI:** Case studies with quantified results. **Case Study 1 (Masterworks marketing stack) is now drafted** — narrative in PROPOSAL.md §B plus a full visual document at `rfp/CASE-STUDY-MASTERWORKS.html`. Hai's jobs: (a) review the draft for factual accuracy (architecture, roles, framing); (b) **confirm or replace every ◆-marked figure** — $2K/day → $1M/day capital raised, cost-per-funded-investor change, share of conversions recovered server-side (G-11c blocks on this); (c) supply 1–2 more case studies for G-12/G-13 — candidates: HubSpot lifecycle work at Masterworks, a current Res engagement (anonymized is fine). Each needs at least one hard number. | **Hai** | Aug 21 |
| G-39 | **Robby's resume — edited Aug 12 (D7, D8):** Worthy corrected to Jan 2025–Apr 2026; Res AI entry added (marked DRAFT) with start date Nov 2025 (matches Hai's LinkedIn); Carat corrected to 2004–Nov 2008; summary 15+ → 20+ years; Zocdoc refocused to growth team / marketing stack / Salesforce (corroborates §A). **Still needed:** Robby to (a) expand the Res AI bullet with current engagements, (b) confirm the Worthy (–Apr 2026) / Res AI (Nov 2025–) ~6-month overlap is the intended presentation, since both entries will be read side by side. | Robby | Aug 21 |
| G-39b | **→ HAI: Hai's resume must corroborate the Carat overlap.** §A now claims the partnership began at Carat in 2004. Hai's LinkedIn export shows "Carat Interactive, Sep 2003 – Nov 2004, San Francisco Bay Area." Confirm the dates and location are accurate as written, since Robby's corrected entry places him at Carat from 2004. If the geography differs (SF vs. NY), we should soften §A to "met through Carat" rather than implying a shared office. Both resumes are required attachments and will be read side by side. | **Hai** | Aug 21 |
| G-19b–23b | Decide on certifications. HubSpot Marketing/Sales/RevOps certs are free, ~3–4 hrs each, verifiable by URL. Directly scored in §5.D. Robby has direct Salesforce experience (Zocdoc) and both have HubSpot experience (Masterworks) — formal credentials would convert that into scoreable evidence. | Both | Aug 19 |
| ~~G-09a~~ | ~~Training/enablement evidence.~~ **RESOLVED Aug 12:** both principals have built programs from scratch and trained internal and external teams across many platforms. Written into §A. | — | Done |
| G-14/G-40 | Work product samples (20% of score): integration map, SOP, training material. Sanitize existing or author originals — decide which path. | Both | Aug 21 |
| G-32–36 | 2 client references + 3 professional references, **with permission confirmed**. | Both | Aug 24 |
| G-27–31 | Pricing: implementation fixed fee + monthly retainer through Jun 30, 2027. | Both | Aug 24 |
| — | Watch for InvestPR's Aug 19 Q&A email to all vendors; fold material answers into the draft. | Robby | Aug 19 |
| — | Rename `gather-assets/hai-li.md` → `hai-tran.md` to match the correct legal name. | Robby | Low priority |
