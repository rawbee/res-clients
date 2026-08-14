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
- [x] **Q0.2:** ~~Who signs?~~ **DRAFTED Aug 13 (D11):** Robby Abaya, Co-Founder & Principal, signs — drafted into the cover letter with rabaya@gmail.com. **Confirm signatory choice and whether to use a tryres.ai address instead; phone still needed (G-04a).**
- [ ] **Q0.3:** InvestPR's stack has been inferred from public evidence (see `rfp/TECH-BRIEF.html`, "First, the headline"): **Salesforce CRM** (named in their own CRM Administrator job posting) + **HubSpot marketing** (hs-scripts on investpr.org) + Google/Meta/LinkedIn ad tags + GTM + Microsoft Clarity. Scheduling and outreach tools are unknown. Use this to pick the strongest certifications and case studies to foreground — but do NOT state platform assumptions in the proposal itself; the RFP discloses the official stack to finalists under NDA.

## Session 1 — Firm Identity (G-01, G-02, G-06 → G-09)

- [x] **G-01 / G-06:** Written as "Res AI, LLC, State of Washington" — **G-06a verification against WA SoS still open (Hai)**.
- [x] **G-07:** New York, NY; remote-first with two San Juan trips budgeted (kickoff + training). **Drafted Aug 13 (D11)** — no PR presence or Spanish capability claimed; confirm if either exists, it would be a differentiator.
- [x] **G-08 / G-09:** §A drafted in full (Session 1 + D11).
- [x] **G-02:** Aug 26, 2026 — written into the header, token removed.

## Session 2 — Experience & Case Studies (G-10 → G-14) — worth 20% directly, supports the 50%

- [x] **G-10:** Experience narrative drafted Aug 13 (D11) from both resumes — Masterworks/Zocdoc/Pinwheel platform + industry coverage. *No nonprofit/government client claimed; if one exists, add it.*
- [x] **G-11:** Case Study 1 = Masterworks. **G-11c resolved Aug 13 (D11):** results bullet now uses only figures corroborated by `gather-assets/hai-li.md` (Hai's own LinkedIn: $2K→$1M+ daily capital raised; $4M/mo spend; 0→25+ team). The *other* ◆-marked figures in CASE-STUDY-MASTERWORKS.html (cost per funded investor, server-side recovery share, speed-to-lead) remain **excluded** pending Hai. Hai still reviews the whole case study for accuracy.
- [x] **G-12 / G-13:** Drafted Aug 13 (D11): Case 2 = Zocdoc (Robby, growth-team marketing systems, enterprise Salesforce); Case 3 = Pinwheel (Robby, SDK/API integration platform for Cash App & Discover). Both grounded in Robby's resume. **Still open: one hard number each (G-12c, G-13c) — owner Robby.** Original coaching guidance:
  - The client (or anonymized descriptor if under NDA),
  - The challenge in one or two sentences,
  - What the firm actually did (tools + tactics),
  - **A measurable result** — dedupe %, sync error reduction, attribution recovery, reporting time saved, lead-response time. If the human offers only qualitative outcomes, ask: "If we looked at the before/after dashboards, what number changed?"
  - Best-fit topics per the RFP: data normalization, system efficiency, campaign attribution.
- [x] **G-14:** **Path decided Aug 13 (D12):** Appendix B = (1) sanitized Masterworks architecture map from CASE-STUDY-MASTERWORKS.html, (2) an authored data-governance SOP excerpt, (3) an authored training-material excerpt. Written into §B. **Producing the three artifacts is still open — G-14/G-40 Open Items row.**

## Session 3 — Technical Approach (G-15 → G-17)

- [x] **G-15:** Drafted Aug 13 (D11): methodology named **Audit → Normalize → Connect → Codify → Enable**, five phases mapped to RFP deliverables. Principals: confirm or rename.
- [x] **G-16:** Drafted Aug 13 (D11): native platform tooling first + Insycle for bulk data quality; native connectors → Zapier/Make/Workato → custom serverless middleware (with runbooks); health checks + alerting; docs in client's workspace + Loom; shared PM board. Principals: strike anything you wouldn't actually use.
- [x] **G-17:** Drafted Aug 13 (D11): email+Slack intake, 4-business-hour acknowledgment, Sev1 same-day / Sev2 next-day / Sev3 within 5 days, AST-aligned hours, monthly support log with invoice, POCs Robby (technical) / Hai (engagement). **These are now commitments in the proposal — confirm you'll staff them.**

## Session 4 — Team (G-18 → G-25) — the core of the 50% criterion

- [x] **G-18:** Drafted Aug 13 (D11): two-principal core — Hai (engagement/enablement), Robby (architecture/integration/ops), specialist bench under Robby's direction.
- [x] **G-19 → G-23:** Table drafted Aug 13 (D11): four RFP roles consolidated onto the two principals (Hai = Engagement + Training lead; Robby = Architect + Integration lead). **Certifications cells assert "HubSpot Academy certifications scheduled for completion before kickoff" — this makes the cert decision (G-19b–23b) a commitment: take them, or edit the cells.**
- [x] **G-24:** Bios drafted Aug 13 (D11) from `gather-assets/` — every claim traceable to the resumes/LinkedIn export.
- [ ] **G-39:** **Resumes for every named person — REQUIRED attachment.** Robby's is edited but has DRAFT markers + overlap question; Hai's needs to be produced from the LinkedIn export. See Open Items.
- [x] **G-25:** Capacity statement drafted Aug 13 (D11): both principals immediately available Sept 14 → June 30, 2027. **This is now an explicit availability commitment in the proposal.**

## Session 5 — Timeline (G-26)

- [x] **G-26:** Schedule adopted as proposed Aug 13 (D11), with a re-baseline clause added (week-3 checkpoint if discovery breaks the stated assumptions). **Principals: confirm no holiday/staffing conflicts Sept–Dec 2026.**

## Session 6 — Budget (G-27 → G-31) — worth 20%

- [x] **G-27:** Drafted Aug 13 (D11): fixed fee for implementation + flat monthly retainer, per the recommended shape.
- [x] **G-28a–f:** Drafted Aug 13 (D11): $9,500 / $14,500 / $17,500 / $11,500 / $8,500 = **$61,500**.
- [x] **G-29a–e:** Drafted Aug 13 (D11): $2,500 + $1,500 + $1,500 + $1,000 = **$6,500/mo**, includes up to 30 hrs/mo.
- [x] **G-30:** Drafted Aug 13 (D11): **$107,000** = $61,500 + $6,500 × 7 (retainer starts Dec 1, 2026, after implementation — *not* the ~9.5-month shape this guide originally suggested; the implementation fee covers Sept–Nov). Math verified.
- [x] **G-31:** Drafted Aug 13 (D11): 7 numbered assumptions — environment size (25 users / 500K records / 10 platforms), access timing, 30 hrs/mo retainer + $200/hr pre-approved overage, change-order triggers, 2 San Juan trips included, third-party licensing passed through at cost, net-30.
- [ ] **Sanity check (STILL OPEN — principals):** all Section F numbers are agent-drafted market-rate estimates. Review as a package: is $107K the bid you want to make? Is anything unexplained or padded-looking? Clarity is scored at 20%.

## Session 7 — References & Compliance (G-32 → G-38)

- [ ] **G-32 / G-33:** ≥2 client references for *similar CRM integration and data governance* work: org, contact name/title, email, phone, services provided. **Ask: "Have these contacts agreed to be listed and been warned they may be called?"**
- [ ] **G-34 / G-35 / G-36:** ≥3 professional references: name, relationship, contact info. (These are distinct from the client references.)
- [x] **G-37:** Full no-conflicts statement drafted Aug 13 (D11), including the "no ties to PR government entities" clause. **Principals: confirm it is factually true for both of you before signing.**
- [x] **G-38:** Data-security + NDA-willingness statement drafted Aug 13 (D11): named MFA/SSO accounts, least privilege, data stays in client systems, credential return, incident notification.
- [ ] **G-40 / G-41:** Collect appendix artifacts: work samples (path decided — see G-14) and certification records (pending the cert decision).

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
| G-06a | **→ HAI: Verify exact registered entity name — new evidence suggests it is NOT "Res AI, LLC."** The tryres.ai footer (extracted Aug 13 into `brand/TRYRES-SITE-COPY.md`) reads **"© MMXXVI Resonance AI Technology, LLC."** The proposal, README, and Robby's resume all currently say "Res AI, LLC." Confirm the registered name + state against the Secretary of State filing, then correct PROPOSAL.md (header, §A, §G statements, signature block), README, both resumes, and the deck consistently. Per D6 this must be right everywhere before signing. | **Hai** | Aug 21 |
| G-11 | **→ HAI: Review Case Study 1 as now written.** The results bullet in PROPOSAL.md §B uses the figures from your own LinkedIn export ($2K→$1M+ daily capital raised; $4M/mo; 0→25+ team) — confirm the framing is accurate. The remaining ◆-marked figures in CASE-STUDY-MASTERWORKS.html (cost per funded investor, server-side recovery share, speed-to-lead) are still excluded; supply any you want added. | **Hai** | Aug 21 |
| G-12c / G-13c | **→ ROBBY: One hard number each for the Zocdoc and Pinwheel case studies** (drafted Aug 13 from your resume). Candidates: attribution coverage or acquisition-efficiency change at Zocdoc; SDK adoption, integration count, or support-load reduction at Pinwheel. Qualitative fallback weakens a 20% criterion — find a number. | **Robby** | Aug 21 |
| G-04a | **→ ROBBY:** Phone number for the signature block; confirm you're the signatory and whether to use a tryres.ai address instead of rabaya@gmail.com. | **Robby** | Aug 21 |
| §F review | **→ BOTH: Approve or adjust the drafted pricing** — $61,500 implementation + $6,500/mo × 7 = **$107,000 total**, 30 hrs/mo retainer, $200/hr overage, 2 San Juan trips included, net-30. All agent-drafted (D11); this is the single highest-stakes review item. | **Both** | Aug 21 |
| D11 review | **→ BOTH: Read PROPOSAL.md end-to-end.** Nearly every section now carries drafted commitments in your names — SLAs (Sev1 same-day), capacity through June 2027, travel, the conflict statement, methodology name. Strike anything you won't stand behind. | **Both** | Aug 21 |
| G-39 | **Robby's resume — RFP-tailored Aug 13 (D13); previously edited Aug 12 (D7, D8).** Now repositioned from an AI/solutions-architect resume to a CRM-architecture / systems-integration / martech one: new subtitle line and summary, `TECHNICAL SKILLS` replaced by an `AREAS OF EXPERTISE` block led by CRM & martech / data governance / integrations / attribution / enablement, Masterworks and Zocdoc entries expanded to corroborate §A and Case Studies 1–2, contact line now carries email + a `[G-04a]` phone token. **No dates, titles, or employers changed.** **Still needed from Robby:** (a) expand the Res AI bullet with current engagements — the `[DRAFT]` marker is still in the file; (b) confirm the Worthy (–Apr 2026) / Res AI (Nov 2025–) ~6-month overlap is the intended presentation, since both entries will be read side by side; (c) confirm the two new Masterworks bullets (HubSpot-canonical stack + Segment/Braze fan-out; in-house automation service doing SMS, ad-audience sync, and offline conversion feedback) describe **his own** contribution accurately — they come from his verbal description via D9, not from a prior written source, and they are what make §A's platform paragraph survive D6. | Robby | Aug 21 |
| G-39b | **→ HAI: Hai's resume must corroborate the Carat overlap.** §A now claims the partnership began at Carat in 2004. Hai's LinkedIn export shows "Carat Interactive, Sep 2003 – Nov 2004, San Francisco Bay Area." Confirm the dates and location are accurate as written, since Robby's corrected entry places him at Carat from 2004. If the geography differs (SF vs. NY), we should soften §A to "met through Carat" rather than implying a shared office. Both resumes are required attachments and will be read side by side. | **Hai** | Aug 21 |
| G-19b–23b | **Certifications — now a commitment, not just a decision.** The §D table (drafted Aug 13, D11) asserts "HubSpot Academy certifications scheduled for completion before kickoff." Either actually schedule/take them (free, ~3–4 hrs each, verifiable by URL) or edit the cells before submission. Per D6, an unfulfilled cert claim next to resumes with no certs is a scoring risk. | Both | Aug 19 |
| ~~G-09a~~ | ~~Training/enablement evidence.~~ **RESOLVED Aug 12:** both principals have built programs from scratch and trained internal and external teams across many platforms. Written into §A. | — | Done |
| G-14/G-40 | Work product samples (20% of score). **Path decided Aug 13 (D12):** (1) sanitize the Masterworks architecture map, (2) author a data-governance SOP excerpt, (3) author a training-material excerpt — §B now promises exactly these three in Appendix B. **Remaining work: produce the three artifacts.** Agent can draft 2 and 3; the map needs sanitization sign-off from Hai. | Both | Aug 21 |
| G-32–36 | 2 client references + 3 professional references, **with permission confirmed**. The only section still fully open — 17 of the 21 remaining tokens. Names cannot be drafted by agent. | Both | Aug 24 |
| — | Watch for InvestPR's Aug 19 Q&A email to all vendors; fold material answers into the draft. | Robby | Aug 19 |
| — | **Font licensing for `rfp/PROPOSAL-DECK.html` (see D10).** The deck embeds six commercial woff2 faces (American Grotesk, Martina Plantijn, Atlas Typewriter) pulled from tryres.ai and inlined as base64. Embedding them in our own submitted proposal is ordinary brand use; **serving them from a publicly shared artifact URL is redistribution.** Confirm the licenses cover both, or swap to fallback faces before the deck is shared outside Res. Does not block the PDF submission to InvestPR. | Robby | Aug 21 |
| — | Rename `gather-assets/hai-li.md` → `hai-tran.md` to match the correct legal name. | Robby | Low priority |
| G-39c | **Hai's resume does not exist yet — only the raw LinkedIn export (`gather-assets/hai-li.md`).** Appendix A requires a resume for *every* named team member (RFP §6), and Robby's is now RFP-tailored (D13) while Hai's is an unformatted paste. Produce a matching resume for Hai in the same tailored format — an agent can draft it from the export, but Hai must supply the CRM/martech-specific detail (HubSpot depth at Masterworks, enablement/training programs run) that the export doesn't contain. **A polished resume next to a raw export is a visible asymmetry on a 50%-weighted criterion.** | **Hai** (draft: agent) | Aug 21 |
| G-39d | **Clear the `[G-04a]` and `[G-19b]` tokens now sitting inside `Robby_Abaya_Resume.md` before PDF export.** They are deliberate visible markers (same convention as PROPOSAL.md) but the resume is a shipped attachment — a `[G-…]` string in the submitted PDF is worse than a missing phone number. Covered by the final-QA checklist. | Robby | Aug 26 |
