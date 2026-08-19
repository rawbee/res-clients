# DECK-COPY.md — Copy master for PITCH-DECK.html

> **This file owns every string in the deck.** `PITCH-DECK.html` is a rendering of it — edit here, then ask an agent to re-sync the deck (it does not auto-update). Numbers come from `SIM-FACTS.md` (illustrative) and the InvestPR README's sourced credentials (D7); nothing else is invented. Vocabulary follows `CONTEXT.md`.
>
> Conventions: `EYEBROW` = small mono label top-left. `FOOT` = the numeral · Latin · italic descriptor strip. Divider slides are dark. Part system (Roman numeral · Latin label):

| Part | Latin | Gloss | Covers |
| :--- | :--- | :--- | :--- |
| I | Fieri Potest | it can be done | feasibility |
| II | Ordo | the order of things | operating model, the agent's day, the twelve functions |
| III | Tvtela | guardianship | autonomy, bounded; what the Operator sees |
| IV | Discere | to learn | measurement and learning; working with Google |
| V | Machina | the machine | architecture; the path |
| VI | Qvi Svmvs | who we are | why Res; next step |

- **Draft bar (screen-only):** DRAFT · FOR HAI'S REVIEW — "Illustrative numbers throughout (SIM-FACTS.md). Fictional store names. Bar and internal notes don't print."

---

## Slide 1 — Cover

- EYEBROW: A response to Group 1 · in six parts
- HEADLINE: Agents as the operating layer.
- SUB: Day-to-day Google Ads management across 147 dealerships, performed by agents. Strategy, budgets, guardrails and exceptions kept by Group 1.
- FACTS: Prepared for · Group 1 Automotive — Prepared by · Hai Tran, Res AI — Date · August 2026 — In reply to · "another agentic AI use case"

## Slide 2 — We heard you

- EYEBROW: Avdivimvs · we heard you
- HEADLINE: You didn't ask for a smarter dashboard.
- LEDE: You asked whether agents could *be* the operating layer — perform the day-to-day management your agency does today, working with Google's auction automation, informed by your own first-party data, inside rules and limits you set.
- THE TWELVE (grid, verbatim from the ask): Manage budgets and pacing · Analyze search terms, add/remove negatives · Manage keywords and match types · Manage bidding strategies and targets · Identify wasted spend and underperformers · Adjust campaign and ad group structure · Manage targeting and settings · Optimize ads, messaging and creative · React to inventory, demand and business conditions · Reallocate spend across campaigns · Execute through the Google Ads API · Measure downstream impact and learn from it
- OPERATING MODEL (three lines): Group 1 sets strategy, objectives, budgets and guardrails. · Agents perform the day-to-day management. · Humans manage strategy and exceptions, not campaigns.
- CLOSING LINE: And not Skai — not another platform your team would still have to operate.
- FOOT: Avdivimvs · *the ask, restated*

## Slide 3 — Our answer

- EYEBROW: Responsvm · our answer
- HEADLINE: Yes. It's buildable now — and the hard part isn't the AI.
- THREE STATEMENTS:
  1. **Feasible.** Every one of the twelve functions is a Google Ads API operation an agent can perform with the business context Google doesn't have. The model is not the bottleneck.
  2. **Not a platform.** An operating layer: one Store Agent per dealership, one Portfolio Agent across all 147, a single console for the humans who set strategy and decide exceptions.
  3. **Bounded.** Autonomy is mechanical, not a promise: every action is classified Auto, Review or Never against guardrails you own, enforced in code before it reaches Google.
- KICKER LINE: Group 1 corporate runs the show. The agents do the work.
- FOOT: Responsvm · *in one breath*

## Slide 4 — Divider I (dark)

- KICKER: I · Fieri Potest
- DISPLAY WORD: FEASIBLE
- QUOTE: The question isn't whether an agent can change a bid. It's whether you can trust it to.
- ATTRIB: Part I · Feasibility
- FOOT: I · Fieri Potest · *it can be done*

## Slide 5 — The feasibility perspective

- EYEBROW: I · Feasibility
- HEADLINE: What's proven, what's actually hard, and where we'll be honest.
- COL 1 — PROVEN TODAY: Agents that read data, reason, and act through tools are in production across industries. The Google Ads API is mature and complete — budgets, bids, keywords, negatives, assets, structure, reporting, change history. Model context is large enough to hold a store's whole picture: guardrails, inventory, outcomes, its own history.
- COL 2 — ACTUALLY HARD (and where the work is): **Guardrails** — enforced mechanically, in code, not by asking the model nicely. **Measurement** — joining ad activity to leads, appointments and sold units from your CDP, with lag. **Trust** — every decision explained, every outcome written back, autonomy widened as it's earned.
- COL 3 — HONEST LIMITS: Performance Max exposes few levers; the agent works the ones it has (budgets, asset groups, signals, exclusions). Smart Bidding relearns after big moves — the agent moves deliberately and watches. Google's API and policies change; that's maintenance, not magic. Agent judgment is evaluated against your history before it's allowed to act alone.
- FOOT: I · Fieri Potest · *the perspective you asked for*

## Slide 6 — Divider II (dark)

- KICKER: II · Ordo
- DISPLAY WORD: MODEL
- QUOTE: One agent per store. One across all of them. One console for the humans.
- ATTRIB: Part II · The operating model
- FOOT: II · Ordo · *the order of things*

## Slide 7 — The operating model

- EYEBROW: II · Operating model
- HEADLINE: Operator, Portfolio Agent, Store Agents.
- THREE TIERS (diagram):
  - **The Operator** — Group 1 corporate. Sets objectives, budgets and guardrails; works the exceptions queue; reallocates at portfolio level. A role sized in single digits, not the headcount centralization would have cost.
  - **The Portfolio Agent** — one for Group 1. Sees across stores: moves budget between them within corporate limits, spots systemic patterns, proposes guardrail changes to the Operator.
  - **Store Agents** — one per dealership, 147 of them. Each holds its store's guardrails, inventory, first-party outcomes, campaign state and its own decision history — and runs the day-to-day.
- LINE: Every observation, decision, action and outcome lands in one Decision Ledger. That's what the Operator reads and what learning feeds on.
- FOOT: II · Ordo · *three roles*

## Slide 8 — A Store Agent's day

- EYEBROW: II · The cycle
- HEADLINE: Observe, decide, execute, measure, learn — on three rhythms.
- RHYTHMS (three columns):
  - **Daily** — after yesterday's data settles: full review of the store — pacing, search terms, keyword and bid health, ads, structure. Decide the day's actions; execute the Auto ones; queue the Review ones as Exceptions.
  - **Intraday** — every few hours: pacing and anomalies only. A campaign burning budget, a CPC spike, zero impressions where there should be many.
  - **On events** — an inventory delta lands, a CDP signal fires, a GM flags a tent sale, the Portfolio Agent reallocates. The agent re-plans that store now.
- MEASURE LINE: Measure is decoupled from execute: each action carries an evaluation window — 7, 14 or 28 days — and its outcome is written back when the window closes. That is what makes "learn" real.
- FOOT: II · Ordo · *what a day looks like*

## Slide 9 — Your twelve functions, answered

- EYEBROW: II · The twelve
- HEADLINE: Every line of your list, and which part of the system does it.
- TABLE (function → done by → tier by default):
  | Manage budgets and pacing | Store Agent · pacing | Auto within cap; cross-store = Portfolio Agent |
  | Search terms; add/remove negatives | Store Agent · search-term hygiene | Auto |
  | Keywords, match types, components | Store Agent · keyword management | Auto; overhauls = Review |
  | Bidding strategies and targets | Store Agent · bidding | Auto within ±15%; strategy switch = Review |
  | Wasted spend, underperformers | Store Agent · daily review | Auto pause; campaign pause = Review |
  | Campaign and ad group structure | Store Agent · structure | Review |
  | Targeting and settings | Store Agent · settings | Auto within bounds; geo expansion = Review |
  | Ads, messaging, creative assets | Store Agent · creative | Auto for variants; new messaging = Review |
  | Inventory, demand, business conditions | Store Agent · event cycles | — (input, not action) |
  | Reallocate across campaigns / stores | Store + Portfolio Agent | Auto ≤ threshold; above = Review |
  | Execute via the Google Ads API | Execution Gateway | every action, one path |
  | Measure downstream impact; learn | Ledger + Portfolio Agent | continuous |
- FOOT: II · Ordo · *nothing left off the list*

## Slide 10 — Divider III (dark)

- KICKER: III · Tvtela
- DISPLAY WORD: BOUNDED
- QUOTE: Requiring approval for every action defeats the purpose. So does approval for none.
- ATTRIB: Part III · Autonomy, bounded
- FOOT: III · Tvtela · *guardianship*

## Slide 11 — Autonomy, bounded

- EYEBROW: III · Guardrails
- HEADLINE: Auto. Review. Never.
- THREE TIERS:
  - **Auto** — executes now, logged. Negatives; budget shifts ≤ 10% within the store's monthly cap; target moves ±15%; pausing an ad that's statistically worse.
  - **Review** — the agent prepares the change with its evidence and waits for the Operator. Budget moves above threshold or across stores; pausing or creating campaigns; structural changes; anything touching an OEM co-op campaign.
  - **Never** — refused in code. Exceed a store's monthly cap; edit locked campaigns; touch conversion tracking.
- SCOPES LINE: Guardrails are set at three scopes that inherit — enterprise defaults, brand or region overrides, store overrides — and edited by the Operator, not by us.
- CIRCUIT BREAKER: If a store's cost per lead, pace, or lead volume drifts past a bound over a lookback window, the agent freezes its own Auto actions for that store, rolls back the likely cause, and raises an Exception.
- FOOTNOTE: Thresholds shown are illustrative defaults. Group 1 tunes them; the sim shows how.
- FOOT: III · Tvtela · *the boundary is mechanical*

## Slide 12 — What the Operator sees

- EYEBROW: III · The console
- HEADLINE: A morning's work, not 147 dashboards.
- STILL 1 — Portfolio, 7:05am: Yesterday · $148,900 spent vs $151,600 plan · 98% pace · 1,204 actions · 1,167 Auto · 31 Exceptions · 6 Circuit Breakers · Cost per sold unit $296.
- STILL 2 — An Exception card: Bayou City Toyota · Shift $420/day from New · Tacoma to Used · Trucks & SUVs. Why: Tacoma inventory 31 → 4; aged used 29 → 47. Last time (May 12): used leads +22%, CPL flat. Crosses the 10% Auto threshold → Review. Approve · Modify · Reject · Ask.
- STILL 3 — A guardrail moves: Toyota stores · 38 Exceptions in 30 days for "budget shift 10–15%" · 38 of 38 approved. Raise the Auto threshold to 15%? Projected Exceptions per week: 11 → 4.
- LINE: The interactive walkthrough shows the whole morning: 22 minutes, five decisions, 1,204 actions.
- FOOT: III · Tvtela · *from the walkthrough*

## Slide 13 — Divider IV (dark)

- KICKER: IV · Discere
- DISPLAY WORD: LEARN
- QUOTE: Not "self-improving AI." Memory, calibration, and experiments you can inspect.
- ATTRIB: Part IV · Measure and learn
- FOOT: IV · Discere · *to learn*

## Slide 14 — Learn, concretely

- EYEBROW: IV · Learning
- HEADLINE: Three mechanisms, all inspectable. The model itself is not retrained.
- MECHANISMS:
  1. **Store memory** — each Store Agent decides in light of its own decision-and-outcome history for that store. "The last time we shifted into used here, leads rose 22% at flat CPL."
  2. **Calibrated thresholds** — how aggressive a bid move, how much pacing headroom, when a term is waste: parameters the Portfolio Agent re-tunes from measured outcomes across stores, proposing changes to the Operator when they'd cross a guardrail.
  3. **Designed experiments** — store and geo holdouts, budget splits — so learning measures incrementality, not seasonality or Google's own automation.
- NORTH STAR: Outcomes come from your CDP — leads, appointments, showroom visits, sold units — not Google's proxy metrics. The north star is cost per sold unit; leads and appointments are the leading indicators the agents steer by day-to-day.
- FOOT: IV · Discere · *what "learn" means*

## Slide 15 — Working with Google, not against it

- EYEBROW: IV · Division of labor
- HEADLINE: Google runs the auction. The agent runs the business context.
- TWO COLUMNS:
  - **Google's automation keeps** — Smart Bidding's auction-time bids; Performance Max's channel and asset mixing; responsive search ad assembly; audience expansion.
  - **The agent decides** — targets, budgets and pacing; structure and negatives; which assets and which messages; what inventory to push and when; what a store's business conditions mean this week; and whether any of it is working, measured in sold units.
- LINE: Exactly the layer you described: the broader day-to-day decisions Google doesn't have the context to make.
- FOOT: IV · Discere · *with, not against*

## Slide 16 — Divider V (dark)

- KICKER: V · Machina
- DISPLAY WORD: SYSTEM
- QUOTE: One path in, one path out, everything on the record.
- ATTRIB: Part V · Architecture and the path
- FOOT: V · Machina · *the machine*

## Slide 17 — Architecture

- EYEBROW: V · Architecture
- HEADLINE: Reads from everything. Writes to one place.
- DIAGRAM: Sources — Google Ads API · your CDP · inventory feed · business conditions · guardrails → Store Agents (×147) with Specialists · Portfolio Agent → Execution Gateway (tier check · guardrail check · ledger · rollback) → Google Ads. Ledger → Store memory · Portfolio calibration · Operator console.
- LINES: Every mutation goes through one Execution Gateway that enforces the tier, checks the guardrail, writes the ledger, and can roll back. Nothing writes to your CDP or DMS. The Never list lives in code, not in a prompt.
- FOOT: V · Machina · *one gateway*

## Slide 18 — The path to the end-state

- EYEBROW: V · The path
- HEADLINE: Autonomy is earned, by tier and by store.
- THREE STAGES (a single line, not a plan):
  - **Shadow** — agents decide, humans still execute; we measure agreement and would-have-been outcomes.
  - **Assisted** — agents execute Auto-tier actions; everything else is an Exception.
  - **Autonomous** — the end-state: Auto widens as guardrails prove out, store by store, brand by brand.
- LINE: The Operator's "make this Auto going forward" is the mechanism. How fast, and in what order, is a conversation for after we've agreed to do this together.
- FOOT: V · Machina · *earned, not assumed*

## Slide 19 — Divider VI (dark)

- KICKER: VI · Qvi Svmvs
- DISPLAY WORD: RES
- QUOTE: Operators who have run the spend, running agents they built themselves.
- ATTRIB: Part VI · Who we are
- FOOT: VI · Qvi Svmvs · *who we are*

## Slide 20 — Why Res

- EYEBROW: VI · Why Res
- HEADLINE: We've run the spend, built the stack, and we already ship agents that act.
- THREE BLOCKS:
  - **Run the spend.** Hai Tran built Masterworks' marketing organization from zero to 25 people and up to $4M a month in paid media as co-founder and CMO, then CPO. He knows what an account team does all day — and what it shouldn't have to.
  - **Built the stack.** Robby Abaya spent two decades as the engineer behind marketing systems — principal engineer on Zocdoc's growth team and marketing stack; the Masterworks data and automation stack; payroll and financial APIs at Pinwheel.
  - **Ship agents that act.** Res is what we do now: hand-authored agents that don't just recommend — they publish straight into a client's own systems, under human sign-off. The same execute-with-guardrails pattern this system needs. Our own site says it: *"Selling more used cars off a lot in Houston."*
- LINE: Twenty years working together across four companies. The people you meet are the people who build it.
- FOOT: VI · Qvi Svmvs · *the argument from continuity*

## Slide 21 — Next step

- EYEBROW: VI · Next
- HEADLINE: A working session, not a proposal.
- BODY: Half a day with your marketing, data and agency leads. Your guardrails on a whiteboard, one store's real numbers, your CDP's shape. We come back with the build as it would actually be for Group 1 — and the walkthrough you've seen, running on your data.
- WHAT WE'D BRING: The interactive Operator walkthrough · The builder's view of the architecture · Our honest read on your data readiness.
- SIGNOFF: Hai Tran · Res AI · tryres.ai
- FOOT: VI · Qvi Svmvs · *the next conversation*
