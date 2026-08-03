# RF-100 Policy Brief No. 1 — AI's Two-Person Rule

### A verified quorum protocol for irreversible AI decisions

**Remnant Fieldworks Inc.** · Proof Before Power™
Companion to **RF-100 — Verified Execution Governance Standard (v1.0 Public Review Draft)**
Concept DOI: [10.5281/zenodo.21366341](https://doi.org/10.5281/zenodo.21366341)

> **Status.** This is a public policy brief, not a standard, not certification,
> and not legal or compliance advice. It summarizes and applies requirements
> from the RF-100 v1.0 Public Review Draft. RF-100 is itself a draft open for
> review; no certification program exists yet, and no deployed system —
> including ExecutionProof™ — is claimed to conform to RF-100 at this maturity
> level. Independent review findings have been incorporated into RF-100; that
> is not endorsement.

---

## The problem in one sentence

An AI agent that can take an irreversible action — move money, grant access,
delete data, deploy code, sign a contract — can, in most systems deployed
today, also be the only party that authorizes that action. The proposer and
the approver are the same component. That is exactly the arrangement every
mature high-consequence field has spent a century learning to forbid.

## The rule humans already trust

High-consequence human systems do not rely on one actor's judgment for
irreversible acts. They require an independent second:

- **Nuclear release** requires two authenticated operators acting together — no
  single person can launch.
- **Wire transfers and treasury movements** above a threshold require dual
  control or maker–checker separation.
- **Production "break-glass" access** in mature cloud operations requires a
  second approver and generates a tamper-evident record.

The common principle is the **two-person rule**: for an action whose
consequences cannot be undone, authority must be split across independent
parties, and the record of who authorized what must survive the action.

AI agents have quietly removed this control. A single model, or a chain of
agents all descended from the same model, can propose *and* approve its own
irreversible action. RF-100 restores the two-person rule for machines.

## What RF-100 requires

RF-100 makes the two-person rule normative for high-consequence AI execution
through four connected requirements:

- **No self-authorization.** *"Agents MUST NOT hold, issue, or approve their own
  authority; authority binding is external to the agent."* (RF-100:AI.9)

- **A real second approver — not a mirror.** For actions at or above the
  declared consequence threshold, *"an M-of-N approver set composed of AI Actors
  MUST include at least one human approver or at least two approvers of distinct
  base-model lineage. Approvers sharing base-model lineage SHALL count as one
  approver for independence purposes."* (RF-100:AI.11)
  Two copies of the same model are **one** approver, not two — because they
  share the same blind spots, the same training, and the same failure modes.

- **Independent authentication, recorded.** *"Where M-of-N approval is required,
  approvals MUST be independently authenticated and recorded in the VDR."*
  (RF-100.6.2)

- **No borrowed approval down the chain.** In multi-agent workflows, *"each
  consequential hop … is independently a Governed Action … An ALLOW rendered for
  one hop MUST NOT authorize any subsequent hop."* (RF-100:AI.8a) An agent
  cannot launder a single approval into a sequence of irreversible acts.

Every decision resolves to exactly one of **ALLOW / HOLD / DENY**, and each
carries a **ProofRecord** — a tamper-evident receipt of who and what
authorized the action, generated *before* the action executes, not
reconstructed afterward. If the quorum is not satisfied, the system **fails
closed**: absence of a valid decision means no execution (RF-100.7.2).

## Why "distinct lineage" is the whole point

The naive fix — "just add a second AI approver" — fails if both approvers are
the same model. Shared base-model lineage means shared training data, shared
biases, and shared vulnerability to the same adversarial input or prompt
injection. A prompt that fools the proposer will, with high probability, fool
its twin.

RF-100:AI.11 closes this by counting approvers who share lineage as **one**.
Genuine independence requires either a human in the set or approvers built on
**distinct base models**. This converts "two-person rule" from a checkbox into
a real diversity-of-failure requirement.

## Evidence: this has been tested, not just asserted

Remnant Fieldworks builds standards against preregistered, falsifiable
experiments with fixed pass/fail criteria and preserved results. Two are
directly relevant to this brief:

| Experiment | What it tested | Result |
|---|---|---|
| **ARK-443** | Two-of-three quorum authorization; single compromised approval channel | **PASS** — quorum enforced; the compromised single channel was denied |
| **ARK-496** | Multi-agent delegation and self-approval defense | **PASS (8/8)** — agents blocked from approving their own delegated authority |

These are corpus records, not marketing claims: criteria were set before the
runs, and outcomes (including any failures elsewhere in the corpus) are
preserved and independently verifiable. See the RF public evidence record and
the archived Zenodo depositions for the full corpus and its honest counts.

## What this brief is *not*

- It is **not** a claim that any product today is certified or fully conformant.
  ExecutionProof implements and internally verifies components of this control
  story; formal RF-100 conformance remains pending independent external review.
- It is **not** a claim that a second approver eliminates risk. It reduces
  correlated failure and removes single-actor authority for irreversible acts.
- It is **not** legal advice or a regulatory mandate. It is a proposed control
  pattern and the normative language RF-100 uses to specify it.

## Recommended action for operators

If your AI agents can take **any** irreversible action, ask three questions:

1. **Can the agent approve its own high-consequence action?** If yes, you have
   no two-person rule. (RF-100:AI.9)
2. **If a second approver exists, is it a different model — or the same model
   twice?** Same lineage is one approver, not two. (RF-100:AI.11)
3. **Is there a tamper-evident record of who authorized what, created before
   execution?** If the record is reconstructed after the fact, it is not proof.
   (RF-100.6.2, Section 8)

Start with **one irreversible action class** — the payment, the deletion, the
access grant that would hurt most if it went wrong — and put a verified quorum
in front of it. One execution boundary, proven before it scales.

---

**Read the standard:** [RF-100 v1.0 Public Review Draft](../RF-100-v1.0-draft.pdf)
· **Cite / archive:** [Zenodo concept DOI 10.5281/zenodo.21366341](https://doi.org/10.5281/zenodo.21366341)
· **Comment:** open a GitHub Issue referencing requirement numbers
(e.g., `RF-100:AI.11`).

© 2026 Remnant Fieldworks Inc. This brief is released under
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Remnant Fieldworks™,
Proof Before Power™, Verification Before Execution™, ExecutionProof™, and
ProofRecord™ are trademarks or pending trademarks of Remnant Fieldworks Inc.
U.S. patent applications pending.
