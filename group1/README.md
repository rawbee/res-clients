# Group 1 — Agentic Google Ads Operating Layer (pitch)

**Goal:** answer the ask in `ask.md` with a pitch that Res AI builds the system. Three HTML deliverables (planned): a Group 1 user simulation, a staff/builder simulation, and a non-interactive pitch deck.

## Decisions already made — do not silently reverse these

**D1 — Pitch the all-in end-state, not a pilot.** (Aug 18, 2026, Robby.) The deck sells agents as the operating layer across all 147 dealerships, and covers the path to get there only enough to be credible. Implementation/phasing strategy is a post-win conversation. *Consequence:* the user simulation shows the steady-state system, not a shadow-mode pilot.

## File map

| File | What it is |
| :--- | :--- |
| `ask.md` | Group 1's email — the ask. Reference only |
| `CONTEXT.md` | Glossary of the system's language (Operator, Store Agent, Guardrail, Autonomy Tier, Exception, …). Definitions only, no implementation |
| `docs/adr/` | 0001 two-level agent topology · 0002 single Execution Gateway, Never enforced in code · 0003 learning = memory + calibration + experiments |
| `SIM-FACTS.md` | The fictional dataset seeds and the numbers every deliverable must agree on. Illustrative only |
| `DECK-COPY.md` | Copy master for the deck — every string on the slides. Edit here, then re-sync the deck |
| `USER-SIM.html` | Guided interactive walkthrough of the Operator's morning (persona 1, D3/D4): seven beats, real interactions (Ask/Approve/Modify/Reject, Circuit Breaker, Business Condition stream, guardrail slider, weekly reallocation), plus a browsable console (Portfolio · Exceptions · Stores · Guardrails · Objectives) over a deterministic 147-store dataset. `open USER-SIM.html` (`?beat=N`). Also at <https://claude.ai/code/artifact/7d6a2fc4-cf02-40e1-84ed-58548bcfa24f> |
| `PITCH-DECK.html` | 21-slide 16:9 non-interactive deck in the tryres.ai brand system (D6) — a rendering of DECK-COPY.md. `open PITCH-DECK.html`; `?slide=N` shows one slide (screen only); ⌘P prints widescreen PDF. Also at <https://claude.ai/code/artifact/38d9ac9f-2975-4053-b7b7-66787a9226c1> |
| `STAFF-SIM.html` | Internal builder walkthrough (D5): clickable architecture map, one Cycle traced end-to-end (Bayou City Toyota), Circuit Breaker interactive, Portfolio Agent, safety engineering, reference stack (*reference, not decided*), candid build risks. `open STAFF-SIM.html` (`?theme=light|dark`, `?step=N`). Also at <https://claude.ai/code/artifact/64dec847-5dbb-4fd5-b159-eda84e14ad00>. **Internal — not for Group 1** |

## Where things stand (Aug 18, 2026)
- [x] Design interview complete (D1–D11, glossary, three ADRs)
- [x] All three deliverables built, render-verified in headless Chrome, and published as private artifacts (URLs in the file map). Every number traces to `SIM-FACTS.md`
- [ ] **NEXT: Hai reads the deck end-to-end** (`DECK-COPY.md` is the editable master) and clicks through USER-SIM once before anything goes to Group 1
- [ ] Font licensing (carried over from InvestPR D10) before the deck is shared publicly
- [ ] Nothing here is committed to git yet (`git status` shows `group1/` untracked)

**D2 — CDP stays unnamed; OEM co-op campaigns are in scope as a Review-tier/locked category.** (Aug 18, Robby.) We don't know Group 1's CDP vendor; the pitch says "your CDP." Co-op is included because every franchise dealer has it and it's the most credible example of a Never/Review boundary.

**D3 — The user simulation is a guided walkthrough with real interactivity at key beats** (Aug 18, Robby): approve/modify/reject an Exception, edit a guardrail threshold and watch the tier boundary move, flag a Business Condition and watch the Store Agent react. Not a free-roam mock app.

**D4 — User-sim scenario: one Operator morning in seven beats** (Aug 18, Robby): Portfolio roll-up → inventory-driven reallocation Exception (Ask, then Approve; Reject path shown) → Circuit Breaker review → Business Condition flag with live re-plan → guardrail slider that grows autonomy → Portfolio Agent weekly reallocation + Experiment readout → close ("22 minutes"). Store names are **fictional, with real OEM brands in real Group 1 markets** — never Group 1's actual store names.

**D5 — Staff sim traces one Cycle end-to-end on a clickable architecture map, names a reference stack (Claude Agent SDK, Postgres ledger, durable workflow runner, official Google Ads API client, event bus) labeled *reference, not decided*, and ends with a candid build-risk list.** (Aug 18, Robby.) Audience assumed internal (Res + contractors) — if Group 1 technical staff will see it, soften the risk section.

**D6 — Deck: ~18–22 slides, 16:9, tryres.ai brand system (same as the InvestPR deck: paper `#F2F1EC`, ink `#151512`, accent `#FF4E00`, blue `#1355D8`, Roman-numeral + Latin motif, inlined fonts). No pricing, timeline, team plan, or phasing detail — those are post-win. Path-to-end-state is a single credibility slide.** (Aug 18, Robby.) Font licensing question from the InvestPR project carries over before anything is shared publicly.

**D7 — Deck is from Hai Tran (Res); the custom-agent credential is tryres.ai itself** (Aug 18, Robby): hand-authored agents that act (publish into the client's CMS) under human sign-off — the same execute-with-guardrails pattern. tryres.ai's own copy already says "Selling more used cars off a lot in Houston" — reuse it. Sourced credentials from the InvestPR README (Hai: $4M/mo paid media, HubSpot; Robby: Zocdoc growth/marketing stack, Masterworks stack) are safe to reuse; nothing else gets invented.

**D8 — Agency stance: agents take over the day-to-day management; judgment moves to Group 1 corporate Operators; the deck never attacks the agency.** (Aug 18, Robby.) Whether the agency remains for creative/OEM relationships is Group 1's call and is acknowledged in one line.

**D9 — Sim visual language** (Aug 18, Robby): user sim = product-UI console (neutral light SaaS chrome, system sans, brand palette only as accents: orange = primary action/attention, blue = agent proposals) inside a thin tryres-branded guide chrome (narrator panel, Back/Next, progress rail, "illustrative data" footer); staff sim = TECH-BRIEF-style brand brief with an inline-SVG interactive architecture map. Commercial fonts inlined only in the deck; sims use system stacks.

**D10 — Files and build order** (Aug 18, Robby): `USER-SIM.html`, `STAFF-SIM.html`, `PITCH-DECK.html` in `group1/`, all self-contained, published as private artifacts with URLs recorded here. `DECK-COPY.md` is the single copy master for the deck (the deck is a rendering of it); sims carry their own narration. Build order: user sim → deck → staff sim. One deterministic fictional dataset (147 stores) generated in JS inside the user sim; the deck's numbers are hand-copied from it.

**D11 — North star is cost per sold unit; leads/appointments are leading indicators the agents steer by; the Ledger reconciles them to sales.** (Aug 18, Robby.) Skai is mentioned only on the "we heard you" slide because Group 1 raised it — one line, no comparison slide.
