# "Learn" means Store Memory + calibrated thresholds + designed Experiments — the model is not retrained

The ask wants the system to "measure the downstream impact of decisions and use the results to inform future actions." We define learning as three concrete, inspectable mechanisms: (1) **Store Memory** — each Store Agent's own decision → Outcome history is supplied as context on every Cycle; (2) **calibrated thresholds** — Specialist heuristics are parameters the Portfolio Agent re-tunes from measured Outcomes across Stores, proposing changes to the Operator when they would cross a Guardrail; (3) **Experiments** — Store/geo holdouts and budget splits run by the Portfolio Agent to measure incrementality apart from seasonality and Google's own automation. Outcomes come from the CDP (leads, appointments, sold units), reconciled over each Action's Evaluation Window.

## Considered Options

- **Fine-tuning / retraining the model on outcomes**: opaque, slow, hard to audit, and not what makes the system better — the model is not the bottleneck; store context and measurement are. Rejected. It also lets us say something defensible in the pitch instead of "self-improving AI."
