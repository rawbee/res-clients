# InvestPR RFP Response

**Goal: win the Invest Puerto Rico contract** for CRM architecture optimization, systems integration, and technical operations support. This repo holds the RFP, our proposal-in-progress, and the supporting research.

## Who "we" are

**Res AI, LLC** — a Washington LLC trading as **Res** (brand: <https://tryres.ai>). Two principals, contractors engaged by specialty as needed:

| | |
| :--- | :--- |
| **Robby Abaya** | Engineering. 20+ yrs. Co-founder/CTO Worthy (2025–Apr 2026); Principal SWE Masterworks; Pinwheel (payroll APIs → Cash App, Discover); **Zocdoc — principal engineer, growth team, marketing stack, direct Salesforce experience**; Zynga; Carat. |
| **Hai Tran** | Marketing/product. 25 yrs. Co-founder + CMO then CPO, Masterworks (marketing org 0→25 people, up to **$4M/mo** paid media, **HubSpot** extensively); Zynga art/creative director; Mind Pirate (acq. HP); R/GA; Digitas; Carat. |

They have worked together across **four companies since 2004**: Carat → Zynga → Masterworks → Res.

## Deadlines (hard)

| Date | What |
| :--- | :--- |
| ~~Fri, Aug 14, 2026~~ | ~~Last day to email questions to InvestPR~~ — **declined, see Decision D1** |
| **Wed, Aug 26, 2026** | **Our internal submission target** (2 business days of buffer) |
| Wed, Aug 19, 2026 | InvestPR emails Q&A responses to *all* vendors — **watch for it**, other firms asked questions we didn't |
| **Fri, Aug 28, 2026, 6:00 PM AST** | Proposal due — PDF, emailed, subject: `RFP Response - CRM Architecture Systems Integration & Ops Support` |
| Tue, Sept 8, 2026 | Award notification |
| Mon, Sept 14, 2026 | Project start (engagement runs through June 30, 2027, renewable) |

## File map

| File | What it is | How to use it |
| :--- | :--- | :--- |
| `raw/…FINAL.pdf` | Original RFP as received | Reference only; don't edit |
| `rfp/IPR-RFP-…FINAL.md` | The RFP, converted to markdown | **Source of truth for requirements.** Read this first |
| `rfp/PROPOSAL.md` | The deliverable. Mirrors RFP §5 sections A–G | Every gap is a tagged placeholder like `[G-11c: …]`. Replace tags with real content; `grep '\[G-' rfp/PROPOSAL.md` shows what's left |
| `rfp/GATHER.md` | Interview playbook keyed to the same G-## tags | **The live tracker.** Its *Open Items* table at the bottom is the current frontier — owners and due dates included |
| `rfp/gather-assets/` | Source material from the principals | `Robby_Abaya_Resume.md` (edited Aug 12 — see D7), `hai-li.md` (Hai Tran's LinkedIn export; filename is stale, person is **Hai Tran**) |
| `rfp/TECH-BRIEF.html` | Interactive technical briefing: their ecosystem, seven problems, tool landscape, glossary | `open rfp/TECH-BRIEF.html`. Also at <https://claude.ai/code/artifact/38ca41fe-861c-4832-945c-307fa34e9173> |
| `rfp/CASE-STUDY-MASTERWORKS.html` | Interactive visual case study of the principals' Masterworks marketing stack (Case Study 1 / feeds G-11, candidate G-14 work sample) | `open rfp/CASE-STUDY-MASTERWORKS.html`. Also at <https://claude.ai/code/artifact/e27363ed-2363-4967-820f-8763bf179ee8>. **◆-marked figures are unverified drafts** — see D9 |
| `brand/TRYRES-SITE-COPY.md` | **Editable master of the tryres.ai homepage copy** (extracted Aug 13, 2026) — full narrative, epigraphs, stats + sources, FAQ, footer. A Res-brand asset stored here for convenience, not RFP material | Edit this file first; treat the live site as downstream. **Note: its footer revealed the legal entity as "Resonance AI Technology, LLC" — see the G-06a Open Items row** |
| `rfp/PROPOSAL-DECK.html` | **32-slide 16:9 presentation deck** rendering PROPOSAL.md in the tryres.ai brand language (see D10). Prints to widescreen PDF via ⌘P. Open `[G-##]` items render as blue markup; internal notes + draft bar are screen-only | `open rfp/PROPOSAL-DECK.html`. Also at <https://claude.ai/code/artifact/23ee5054-eb07-4943-833f-0c7b8bc10142>. **A rendering, not a source** — PROPOSAL.md stays the single home for proposal content; re-sync the deck manually after editing PROPOSAL.md (it does not auto-update) |

## Decisions already made — do not silently reverse these

**D1 — No questions round to InvestPR.** (Aug 12, operator's call: no time for a back-and-forth.) *Consequence:* every scope variable we'd have asked about — support volume, user count, record counts, existing documentation — becomes an **explicit stated assumption** in the proposal, especially §F Budget. That converts a gap into evidence of cost clarity, which is 20% of the score.

**D2 — Positioning is the twenty-year partnership, not the new firm.** Res AI is ~9 months old; never foreground that defensively. Lead with Hai + Robby across four companies since 2004. The capacity argument against a two-person firm is answered by continuity: no ramp-up, no internal handoff, no staffing-substitution clause, and the principals who sell the work do the work.

**D3 — Platform neutrality is about *their* stack, not *ours*.** Never assert or imply what InvestPR runs — that intel is inferred (see TECH-BRIEF) and the RFP discloses the real stack only to finalists under NDA. **But do state our own platform history plainly**: Salesforce at Zocdoc, HubSpot at Masterworks, plus Google/Meta/LinkedIn ads, GA, GTM. That paragraph in §A is our strongest fit signal — *do not delete it as an accidental platform-neutrality violation.* The committee connects the dots; we stay clean.

**D4 — The client logos are the principals' career work, not Res engagements.** Nike, Adidas, Activision, EA, HP, Intel, Jeep, NBC, Nokia, Sony, Visa, Vodafone came via R/GA, Carat, Digitas, and Zynga. Always attributed as "programs our principals have led." A 501(c)(3) committee that catches an overstatement kills the bid.

**D5 — Counter-position against their internal hire.** InvestPR is concurrently hiring a CRM Administrator. We are the senior architecture and attribution layer *above* that role, not another pair of hands competing with it. Capability transfer, not dependency.

**D6 — Everything must survive the attachments being read side by side.** Both resumes are required attachments. Any claim in the proposal that the resumes contradict is worse than no claim at all.

**D7 — Robby's resume was edited Aug 12** to reflect facts he supplied: Carat corrected to 2004–Nov 2008 (contract 2004–2006, full-time from Oct 2006 — this is what substantiates the 2004 partnership claim); Worthy corrected to Jan 2025–Apr 2026; Res AI entry added and **still marked `[DRAFT]`**; summary 15+ → 20+ years.

**D8 — Robby's resume, second edit Aug 12** (Robby's direct instruction): (1) Zocdoc entry refocused from mobile-team tech lead to **principal engineer on the growth team working on the marketing stack**, with the Salesforce experience now stated in the entry itself — this closes the D6 gap where §A's "Salesforce at Zocdoc" claim had no corroboration in the required attachment. (2) Res AI start date changed **Apr 2026 → Nov 2025** to match Hai's LinkedIn. *Consequence:* the resume now shows Worthy (Jan 2025–Apr 2026) and Res AI (Nov 2025–present) overlapping by ~6 months — Robby to confirm the concurrent-roles presentation is intended, or adjust one entry. Tracked in the G-39 Open Items row.

**D9 — Case Study 1 is the Masterworks marketing stack, drafted with explicitly-marked placeholder numbers.** (Aug 12, Robby's direction: "take liberty to fill in the gaps … and I'll adjust.") `rfp/CASE-STUDY-MASTERWORKS.html` presents the stack Robby described (HubSpot hub; website → Segment → Braze/Meta/GA fan-out; Braze automations plus a custom server service for SMS and ad retargeting) upgraded to its idealized form, and maps it node-by-node onto the TECH-BRIEF concerns. *Convention:* every figure not backed by `gather-assets/` carries a visible **◆ marker** (also flagged in the doc's draft banner and footer) — per D6, no ◆-marked number may be copied into PROPOSAL.md or shipped externally until Hai confirms it. The doc states plainly it was the principals' work at Masterworks, not a Res engagement (D4). *Amended Aug 13 (during D11):* the $2K→$1M daily-capital figure turned out to be **corroborated by Hai's own LinkedIn export** (`gather-assets/hai-li.md`, Head of Design entry), as are $4M/mo and 0→25 team — so those three moved into PROPOSAL.md §B un-marked. The other ◆ figures (cost per funded investor, server-side recovery share, speed-to-lead) remain excluded pending Hai.

**D10 — The submitted document is a 16:9 slide deck in the tryres.ai brand language.** (Aug 13, Robby's direction: "use the design language from our website … more like presentation slides instead of printed pages.") This *reverses* the Aug 13 first pass, which mirrored InvestPR's own RFP letterhead (Times serif, letter-size pages). The deck now uses the site's system, sampled directly from tryres.ai: paper `#F2F1EC`, ink `#151512`, accent `#FF4E00`, brand blue `#1355D8`; American Grotesk (display), Martina Plantijn (serif body), Atlas Typewriter (mono) — all six faces **inlined as base64** so the file is self-contained. Structure borrows the site's Roman-numeral + Latin-label motif: RFP sections A–G become I–VII (QVI SVMVS, PROBATIO, METHODVS, MANVS, TEMPVS, PRETIVM, TESTIMONIA), each opened by a dark divider slide. *Two guardrails:* (1) **the design changed, the copy did not** — PROPOSAL.md's cooler, concrete register is preserved verbatim per the voice note below; the Latin is a visual motif in eyebrows and footers, never in the proposal's own prose. (2) Orange is reserved strictly for numerals and Latin labels (as on the site); **open items are marked in brand blue**, so "unresolved" can never be confused with "accent."

**D11 — Aggressive fill pass (Aug 13, Robby's direction: "Fill in as much as you can using the info you have. Be aggressive. If things are wrong, we'll make adjustments.").** Agent drafted nearly every remaining section of PROPOSAL.md: cover letter and signature block (Robby as signatory), executive summary with pricing, G-07a travel terms, G-10 experience narrative, Case Studies 2 (Zocdoc) and 3 (Pinwheel) from Robby's resume, methodology name (**Audit → Normalize → Connect → Codify → Enable**), tools list, SLA commitments (Sev1 same-day / Sev2 next-day / Sev3 5-day, AST hours), org structure and role table (four RFP roles consolidated onto the two principals), bios from `gather-assets/`, capacity statement, timeline adoption + re-baseline clause, **full pricing ($61,500 implementation + $6,500/mo × 7 = $107,000)** with 7 stated assumptions, conflict statement, and data-security statement. *Ground rules held:* every quantified claim traces to `gather-assets/`; unverifiable numbers stayed out (G-12c/G-13c are open tokens, not invented figures); references (G-32–36) were left empty because names can't be drafted. *Consequence:* the proposal now contains drafted **commitments** (SLAs, availability, certs-before-kickoff, travel, prices) that the principals must ratify or strike — tracked as the "D11 review" and "§F review" Open Items rows, due Aug 21. Token count: 74 → 21.

**D12 — Work-samples path (Aug 13, closing the question asked repeatedly since kickoff).** Appendix B = sanitize the existing Masterworks architecture map + author two original excerpts (a data-governance SOP and a training quick-reference) in the format we'd deliver to InvestPR. Rationale: the map already exists and is our strongest artifact (D9); authoring the two excerpts is cheaper and safer than sanitizing client documents we may not have rights to, and "the format we deliver" framing keeps them honest. §B now promises exactly these three; producing them is the remaining work (G-14/G-40 row).

**Open question from D10 — font licensing.** The six embedded woff2 faces are commercial (American Grotesk, Martina Plantijn, Atlas Typewriter), pulled from tryres.ai. Embedding them in our own proposal is ordinary brand use, but a *published* artifact serves them to viewers. Robby to confirm the licenses permit this, or swap to fallbacks before anything goes public. Tracked in GATHER.md Open Items.

## Key intelligence

- **Evaluation weights:** 50% ability/capacity · 20% cost clarity/reasonability · 20% examples of work product (integration maps, SOPs, training materials) · 10% references. Spend effort accordingly.
- **Their stack is inferred, not confirmed:** Salesforce (their own CRM Administrator job posting), HubSpot (hs-scripts on investpr.org), Google/Meta/LinkedIn tags, GTM, Microsoft Clarity. Sources in TECH-BRIEF.html, "First, the headline." See D3 for how to use this.
- **Hard requirements easy to miss:** resumes for every named team member; ≥2 client references + ≥3 professional references; explicit conflict-of-interest statement even if none.

## Where things stand (as of Aug 13, 2026)

- [x] RFP parsed; proposal skeleton, gathering guide, technical brief written
- [x] Session 0 triage — questions round declined (D1)
- [x] Robby's resume corrected (D7, D8); Case Study 1 drafted with visual doc (D9)
- [x] **Aggressive fill pass complete (Aug 13, D11): PROPOSAL.md is now a full draft end-to-end** — cover letter, exec summary, §A–§F all written, **pricing drafted at $107,000 total**, work-samples path decided (D12). **21 `[G-` tokens remain** (17 are the reference tables; plus G-04a phone, G-06a entity verify, G-12c/G-13c case-study metrics)
- [x] **Proposal deck (`rfp/PROPOSAL-DECK.html`, D10):** 32 slides, 16:9, tryres.ai brand language; re-synced to the filled draft Aug 13. Font licensing still open before public sharing
- [ ] **THE SINGLE MOST IMPORTANT NEXT ACTION: principals read PROPOSAL.md end-to-end and ratify or strike the drafted commitments (D11 review + §F pricing review rows, due Aug 21).** Everything in it is now real enough to be dangerous if wrong: SLAs, availability, certs-before-kickoff, travel, $107K
- [ ] References with permission (G-32–36) — the only fully-open section; names can't be drafted. Due Aug 24
- [ ] Produce the three Appendix B artifacts (G-14/G-40, path decided in D12) + finalize both resumes (G-39/G-39b) + take-or-strike the HubSpot certs (G-19b–23b)
- [ ] Watch for InvestPR's Aug 19 Q&A email; fold material answers in
- [ ] Final QA (checklist at bottom of GATHER.md) → export PDF → email before Aug 28, 6 PM AST

## For a fresh agent

1. Read the **Decisions** section above first — it encodes calls that are expensive to re-litigate and easy to accidentally reverse.
2. Read `rfp/IPR-RFP-…FINAL.md` (requirements), then `rfp/PROPOSAL.md` to see filled vs. `[G-##]`.
3. **`rfp/GATHER.md`'s Open Items table is the live frontier** — owners, due dates, and what's assigned to Hai vs. Robby.
4. Keep the G-## tag system intact: PROPOSAL.md gaps and GATHER.md questions reference each other by these IDs.
5. Voice: declarative and specific, first-person plural. The tryres.ai brand voice is literary and dramatic; §A deliberately runs cooler than the website because a nonprofit committee scoring on a rubric rewards concreteness. Don't over-correct in either direction.
6. **Before you stop working, run the sync protocol in `CLAUDE.md` → "Keeping the docs in sync."** It defines which file owns which fact, what to update when, and a four-item stop checklist. The whole point is that the next agent can pick up from this README alone — that only stays true if you maintain it as you go.
