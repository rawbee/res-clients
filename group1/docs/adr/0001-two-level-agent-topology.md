# Two-level agent topology: one Store Agent per dealership, one Portfolio Agent, Specialists as skills

The system must hold each dealership's business context (guardrails, inventory, CDP outcomes, its own decision history) while still reallocating across 147 stores. We chose one **Store Agent** per Store that owns that context and runs the observe → decide → execute → measure → learn Cycle, calling shared **Specialist** capabilities (search-term hygiene, keywords/match types, bidding targets, pacing, structure, creative) as skills — plus a single **Portfolio Agent** for cross-store reallocation, systemic pattern detection, threshold calibration, and Experiments.

## Considered Options

- **Per-function agents portfolio-wide** (a Budget Agent, a Keyword Agent, …): simple to explain, but no agent holds the store's business context — the thing Google lacks and the whole point of the ask.
- **147 monolithic Store Agents with no portfolio layer**: full local context, but cross-store reallocation and portfolio-level pattern detection have no home.
- **Specialists as independent sub-agents with their own agendas**: more "agentic" on a slide, more moving parts to reason about, and conflicting proposals with no owner. Rejected in favor of skills invoked by the Store Agent, which stays the single decision-maker for its Store.
