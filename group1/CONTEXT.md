# Group 1 Agentic Ads Operating Layer

The language of the system Res AI is pitching to Group 1: an agentic layer that performs day-to-day Google Ads management across the dealership portfolio, bounded by corporate-set guardrails, escalating what it may not decide alone.

## Language

### People

**Operator**:
The Group 1 corporate person (or small team) who sets objectives and guardrails, works the exceptions queue, and reallocates at portfolio level — the role that replaces the agency's account team.
_Avoid_: admin, account manager, user

**Store**:
A single dealership as a unit of budget, guardrails, and performance.
_Avoid_: dealer, location, rooftop, account

### Autonomy

**Action**:
A single mutation an agent makes or proposes to Google Ads (a budget shift, a negative keyword, a target change, an asset swap, a structural edit), always classified into an Autonomy Tier and always recorded in the Decision Ledger.
_Avoid_: change, optimization, recommendation (that's Google's word)

**Guardrail**:
A limit or rule the agent must respect when deciding or acting, set by the Operator.
_Avoid_: rule, policy, constraint, limit

**Autonomy Tier**:
The classification of an action as Auto (execute and log), Review (prepare and escalate), or Never (refuse), determined by action type and magnitude against the guardrails.
_Avoid_: permission level, approval level

**Exception**:
A Review-tier action awaiting the Operator's decision, or a Circuit Breaker trip needing human attention.
_Avoid_: approval, ticket, alert, escalation (as a noun)

**Circuit Breaker**:
A performance guardrail that, when tripped, freezes Auto-tier actions for a Store, rolls back the likely-causal change, and raises an Exception.
_Avoid_: kill switch, safety stop

**Guardrail Scope**:
The level at which a guardrail is set — enterprise default, brand/region override, or Store override — with narrower scopes inheriting from wider ones.

### Agents

**Store Agent**:
The agent responsible for one Store: it holds that Store's guardrails, inventory and CDP signals, campaign state, and its own decision history, and runs the observe → decide → execute → measure → learn loop for the Store.
_Avoid_: dealer agent, campaign agent, bot

**Portfolio Agent**:
The single agent that sees across all Stores: reallocates budget between Stores within corporate limits, detects systemic patterns, and proposes guardrail changes to the Operator.
_Avoid_: master agent, orchestrator, supervisor

**Specialist**:
A shared capability a Store Agent invokes for one job function — search-term hygiene, keyword and match-type management, bidding targets, pacing, campaign structure, creative. A skill, not an independent agent with its own agenda.
_Avoid_: sub-agent, module, worker

**Decision Ledger**:
The single record of every observation → decision → action → outcome, with the reasoning, written by all agents; what the Operator reads and what learning feeds on.
_Avoid_: audit log, activity feed, history

### The loop

**Cycle**:
One scheduled or triggered run of a Store Agent's observe → decide → execute → measure → learn loop; daily (full review), intraday (pacing and anomalies only), or event-triggered (inventory delta, CDP signal, Operator flag, Portfolio reallocation).
_Avoid_: run, job, sweep, tick

**Evaluation Window**:
The period (7/14/28 days by action type) after an action during which its outcome is measured before being written back to the Decision Ledger.
_Avoid_: lookback, attribution window (that's Google's)

**Store Memory**:
A Store Agent's own decision → outcome history for its Store, supplied as context on every Cycle so decisions are made in light of what was tried and what happened.
_Avoid_: training data, model memory, fine-tuning

**Experiment**:
A controlled test run by the Portfolio Agent (Store or geo holdout, budget split) to measure the incremental effect of a tactic, isolating it from seasonality and Google's own automation.
_Avoid_: A/B test (too narrow), pilot

**Outcome**:
The downstream business result of an action measured over its Evaluation Window — leads, appointments, showroom visits, sold units from the CDP — as distinct from Google Ads proxy metrics.
_Avoid_: result, conversion, KPI

### Data and execution

**Signal**:
Any input a Store Agent observes that is not a Google Ads metric — CDP outcomes, inventory feed, Business Conditions, guardrails.
_Avoid_: data point, feed (as the generic term)

**Business Condition**:
A flag entered by the Operator or a Store's GM describing something the agent cannot see in data — a sale event, OEM incentive, BDC staffing gap, closure.
_Avoid_: note, override, annotation

**Co-op Campaign**:
A campaign co-funded under OEM rules; treated as Review-tier (or locked) by default because changes carry compliance and reimbursement consequences.
_Avoid_: brand campaign, OEM campaign

**Execution Gateway**:
The single path through which any agent mutates Google Ads: it enforces the Autonomy Tier, checks guardrails, writes the Decision Ledger, and can roll back. Nothing writes to the CDP or DMS.
_Avoid_: API wrapper, connector, integration layer

### The console

**Console**:
The Operator's application: Portfolio, Exceptions, Store view, Guardrails, Objectives.
_Avoid_: dashboard, platform, tool, portal

**Objective**:
What the agents optimize toward for a brand, region, or Store — an Outcome target with its constraints (e.g., sold units at a cost-per-sale ceiling; aged-inventory priority; used/new spend mix) plus the monthly budget envelope.
_Avoid_: goal, KPI, target (that's a Google bid setting)

**Ask**:
The Operator's short back-and-forth with a Store Agent about an Exception before deciding.
_Avoid_: chat, comment, query

**North Star**:
Cost per sold unit (from the CDP), the Outcome every Objective is ultimately written against.
_Avoid_: ROAS, CPA, CPL as the primary metric

**Leading Indicator**:
Leads and appointments — the faster-moving Outcomes a Store Agent steers by day-to-day, reconciled to sold units when the Evaluation Window closes.
_Avoid_: proxy metric, conversion
