# SIM-FACTS — the fictional dataset every deliverable must agree on

> All numbers here are **illustrative** (D4/D12). Store names are fictional; OEM brands and Group 1 markets are real. USER-SIM generates the 147-store dataset deterministically from these seeds; PITCH-DECK and STAFF-SIM copy numbers from here, never invent new ones.

## Portfolio
- 147 Stores. Markets (real Group 1 US footprint): Houston (HQ), Dallas–Fort Worth, Austin, San Antonio, Oklahoma City, Tulsa, Boston / New England, Atlanta, South Florida, Tampa, Jacksonville, New Jersey, Maryland, Los Angeles, Kansas, Louisiana, Mississippi, Alabama, South Carolina, New Mexico.
- Brands: Toyota (23 stores), Honda, BMW, Mercedes-Benz, Ford, Chevrolet, Nissan, Lexus, Audi, Hyundai, Kia, Acura, Subaru, Volkswagen, CDJR, GMC.
- Google Ads budget: **$4.6M / month** portfolio (~$31K per Store avg; range $12K–$85K).
- Yesterday: spend **$148,900** vs plan $151,600 (**98% pace**). Month-to-date pace 99%.
- Overnight (one daily Cycle across all Stores): **1,204 Actions · 1,167 Auto · 31 Exceptions · 6 Circuit Breakers**. 30-day average: ~1,150 Actions/day, 96–97% Auto.
- Outcomes MTD: leads 18,240 (+6% vs plan), appointments 7,910, sold units attributed 2,384; **cost per sold unit $296** (objective ceiling $310 used / $260 new).
- Illustrative default Guardrails (enterprise scope): Auto budget shift ≤10% of campaign daily budget within monthly cap; target (tCPA/tROAS) moves ±15%; negatives Auto; pause/create campaign = Review; structure changes = Review; Co-op Campaigns = Review (locked at some Stores); exceed monthly cap / touch conversion tracking / edit locked campaigns = Never. Circuit Breaker: CPL or cost/lead-indicator +35% over 3-day window vs 14-day baseline → freeze + rollback + Exception.

## Objectives (example, Toyota / Texas)
- Used: ≤ $310 per sold unit · New: ≤ $260 per sold unit · Aged inventory (≥ 60 days) prioritized · Used ≥ 40% of spend · Monthly envelope per Store.

## Beat 2 — Exception: inventory-driven reallocation
- **Bayou City Toyota** (Houston, TX). New Tacoma inventory **31 → 4 units** (shipment ETA unknown, 3+ weeks). Used aged inventory ≥60 days **29 → 47 units**.
- Proposal: shift **$420/day** from "New · Tacoma" campaign to "Used · Trucks & SUVs" = **14%** of source campaign budget → crosses the 10% Auto threshold → **Review**.
- Evidence: Tacoma search impressions still strong but no inventory to sell; used truck CPL $41 (7-day), aged units carrying floorplan cost. Store Memory: **May 12** similar shift → used leads **+22%**, CPL flat, 6 aged units sold in 14 days.
- Ask ("why not wait for the shipment?") → "ETA is unconfirmed; every day of Tacoma spend at 4 units is ~$300 of impressions on unavailable inventory; I'll propose reversing when inventory > 12."
- Expected impact: used leads +15–25% at this Store over 14 days; new leads −8%. Evaluation Window 14 days.
- Reject path shown as alternative: agent acknowledges, keeps current split, sets a reminder to re-propose if inventory < 4 or aged > 55.

## Beat 3 — Circuit Breaker
- **Sooner Ridge Honda** (Oklahoma City, OK). CPL **$38 → $53 (+40%)** over Aug 14–16 after a tCPA change **$40 → $46** on Aug 13 (Auto, within ±15%).
- Agent rolled back to $40 on Aug 16, froze Auto for the Store, raised the Exception. Suspects Smart Bidding relearning + competitor "0% APR CR-V" event (search-term evidence: "cr-v 0% apr" queries **+180%**, competitor name terms up).
- Proposal: resume Auto; set tCPA **$42**, watch 7 days; add competitor-incentive terms to a watch list rather than negatives.

## Beat 4 — Business Condition
- **Commonwealth BMW** (Norwood, MA). Operator flags: "Tent sale Sat–Sun Aug 22–23, certified pre-owned focus."
- Store Agent re-plan (streams in): pull forward **$2,100** into Sat/Sun within monthly cap (Auto); add event RSA headlines + sitelinks "CPO Tent Sale · Aug 22–23" (Auto); event keywords + negatives (Auto); increase used CPO campaign target lift +10% Fri–Sun (Auto); **geo radius 15 → 25 mi Fri–Sun** (Review — outside default targeting guardrail).

## Beat 5 — Guardrail change (autonomy grows)
- Portfolio Agent: in 30 days, Toyota Stores (23) generated **38 Exceptions** for "budget shift 10–15%"; **38/38 approved**, median approval 4h 12m.
- Proposal: raise Auto threshold **10% → 15%** for brand scope = Toyota. Projected Exceptions/week for Toyota: **11 → 4**. Operator drags slider; saves.

## Beat 6 — Portfolio Agent weekly
- Reallocation: move **$18,400/week** from **9 Stores** pacing under plan with soft demand (New Mexico, Kansas, Mississippi) to **12 Stores** in DFW/Houston with aged used inventory rising. Within corporate limits (no Store below 85% of envelope, none above 110%).
- Experiment readout: 12-week **24-Store holdout**; aged-inventory prioritization tactic → **used sold units +9.4%** vs holdout, **cost per sold unit −11%**. Recommendation: make aged-inventory priority an enterprise default.

## Close
- **22 minutes.** Operator decided **5** things (approve reallocation, approve breaker resume, flag tent sale + approve radius, raise Toyota threshold, approve weekly reallocation). Agents took **1,204** Actions.
