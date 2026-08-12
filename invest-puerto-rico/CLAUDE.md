# Project: InvestPR RFP Response

Read `README.md` first — it has the goal, deadlines, file map, and current status.

Quick orientation: **Res AI, LLC** (Robby Abaya + Hai Tran) is bidding Invest Puerto Rico's CRM/systems-integration RFP. `rfp/PROPOSAL.md` is the deliverable (gaps tagged `[G-##]`), `rfp/GATHER.md` is the interview guide that fills them and whose **Open Items table is the live tracker**, `rfp/gather-assets/` holds the principals' resumes, `rfp/TECH-BRIEF.html` is the technical research. Proposal due **Aug 28, 2026, 6 PM AST**; internal target **Aug 26**.

**Read README.md's "Decisions already made" section before editing the proposal.** Two are easy to reverse by accident:
- Platform neutrality applies to *InvestPR's* stack (inferred, never assert it) — **not** to our own platform history. The Salesforce/HubSpot experience paragraph in §A is intentional and is our strongest fit signal.
- The Nike/Adidas/Sony-class client list is the principals' career work, never Res engagements.

---

## Keeping the docs in sync (required)

This repo is a relay. Any agent must be able to stop mid-task, and any other agent — or the human, days later — must be able to resume from `README.md` alone. That only holds if every change is written to its home file **as you go, not batched for the end of a session.** An interrupted session is the normal case, not the exception.

### One home per fact — never duplicate, always point

| Fact type | Home | Do not restate elsewhere |
| :--- | :--- | :--- |
| RFP requirements | `rfp/IPR-RFP-…FINAL.md` | Cite it; never re-assert requirements as authority |
| Proposal content | `rfp/PROPOSAL.md` | — |
| Open work, owners, due dates | `rfp/GATHER.md` → **Open Items** table | README may link to it, not copy it |
| Strategy & positioning calls | `README.md` → **Decisions** (`D##`) | — |
| Current status & frontier | `README.md` → **Where things stand** | — |
| Facts about the firm & principals | `README.md` → **Who we are** (sourced from `gather-assets/`) | — |

### Triggers — what to update, and when

| When you… | Immediately… |
| :--- | :--- |
| Resolve a `[G-##]` | Replace the token in PROPOSAL.md · tick its GATHER.md session checkbox · strike or remove its Open Items row |
| Hit a question the human can't answer now | Add an Open Items row with an **owner and a due date**, then keep working. Never stall on it; never guess an answer into the proposal |
| Make or reverse a positioning/strategy call | Add a new `D##` to README with the date **and the reasoning**. To reverse an existing decision, amend it in place with the date — never delete one silently, or the next agent will re-make the mistake it was preventing |
| Edit anything in `gather-assets/` | Record it as a `D##` (see D7 for the pattern). These are source documents the human and other agents rely on being unchanged |
| Learn a new fact about the firm or a principal | Update README → Who we are |
| Change anything at all | Run the stop checklist below before ending the turn |

### Stop checklist

1. **Token count:** `grep -o '\[G-' rfp/PROPOSAL.md | wc -l` — subtract 1 for the `[G-##: …]` example inside the file's own how-to-use note. Update the number in README → Where things stand.
2. **README status is true:** what's done, what's blocked, who owes what — and name the single most important next action explicitly.
3. **No orphaned questions:** anything you asked the human that went unanswered is an Open Items row, not a line in a chat transcript that dies with the session.
4. **No unsupported claims:** anything newly written into PROPOSAL.md is backed by `gather-assets/` or an explicit statement from the human — or is tagged as needing support. Per D6, a claim the attached resumes contradict is worse than no claim.
