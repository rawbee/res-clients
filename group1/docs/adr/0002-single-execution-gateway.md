# All Google Ads mutations go through one Execution Gateway; the Never tier is enforced in code, not prompts

Autonomy is only safe if the boundary is mechanical. Every Action any agent takes reaches Google Ads through a single **Execution Gateway** that classifies the Action's Autonomy Tier against the applicable Guardrails (enterprise → brand/region → Store), executes Auto, queues Review as an Exception, refuses Never, writes the Decision Ledger, and can roll back. Guardrails and the Never list live in configuration the gateway reads at execution time — an agent cannot be talked past them because the model never holds the credentials to bypass the gateway. The system writes only to Google Ads; the CDP and DMS are read-only.

## Consequences

- Prompts describe intent and context; they are never the safety mechanism.
- Dry-run mode, idempotency, rate-limit/quota handling, and rollback are gateway concerns, implemented once.
- Every Action, including refused ones, is in the Ledger — which is what makes the Operator's console and the learn step possible.
