# RF-100 — Verified Execution Governance Standard

**Verification-first execution control for high-consequence systems.**

> "If it cannot be verified, it cannot execute."

## Status

- **Current Version:** v1.0 — UNIFIED DRAFT (second-pass corrected)
- **Published:** July 2026
- **Publisher:** Remnant Fieldworks Inc.
- **Built on:** RF-000 (Proof Before Power™ Doctrine, published)
- **Certification:** None exists yet. RF-101 (assessment) and RF-102
  (certification) are under development. No party may claim RF-100
  certification or formal conformance at this maturity level.

**Review history:**
- v0.9 (July 15, 2026): public draft
- v1.0 unified draft (July 15, 2026): integrated structured peer review findings G-01 through G-18 (James A. Bex, BxTech Systems Solutions LLC)
- v1.0 second-pass corrected (July 16, 2026): integrated second-pass findings F-01 through F-06

## What RF-100 Is

RF-100 defines the minimum normative structure a high-consequence system —
AI agent, automated workflow, financial execution system, infrastructure
controller — MUST satisfy **before** a governed action executes.

The standard specifies requirements for governing consequential actions ("Governed Actions") proposed by human or AI Actors, such that:
- No Governed Action takes effect without independent verification of authority, evidence, policy compliance, and system state
- Every decision is durably and verifiably recorded
- The proposing Actor cannot modify the verification gate, policy, evidence, or decision

**Core elements (Sections 1-13):**
1. Policy and Execution Boundary Profile (EBP)
2. Evidence
3. Verification and Decision Inputs
4. Authority
5. Decisions: Rendering, Validity, and Failure Posture
6. Verification Decision Records (VDRs)
7. Execution Integrity
8. Auditability and Reconstruction
9. Enforcement Architecture (E1/E2/E3)
10. Gate Governance
11. Trusted Time

**AI Actor Profile (RF-100:AI)** defines elevated requirements for AI agents and autonomous systems, including:
- Agent identity (model/version/lineage in every VDR)
- Scoped capability and authority
- Intent Records (untrusted context, never Evidence)
- Consequence thresholds and velocity limits
- Prompt/input-injection detection
- Chained-agent per-hop governance
- Model/prompt-update re-versioning and re-evaluation

## Documents

- **Current:** [`RF-100-v1.0-draft.pdf`](./RF-100-v1.0-draft.pdf) ([markdown](./RF-100-v1.0-draft.md)) — v1.0 unified draft, second-pass corrected
- **Prior version:** [`RF-100-v0.9-draft.pdf`](./RF-100-v0.9-draft.pdf) — v0.9 public draft
- **Archived / citable versions:** [Zenodo concept DOI 10.5281/zenodo.21366341](https://doi.org/10.5281/zenodo.21366341) (stable link across all versions)

## How to Review / Comment

This draft is open for public review. The draft is strongest where it
gets attacked.

- **Open a GitHub Issue** in this repository for any critique, ambiguity,
  missing requirement, conflict with existing standards (NIST AI RMF,
  ISO 42001, SOC 2, etc.), or implementation concern.
- Please reference requirement numbers (e.g., `RF-100.7.2`, `RF-100:AI.3`)
  where possible.
- Substantive feedback will be credited in the v1.0 revision history
  unless you request otherwise.

## What This Is Not

- Not a certification program (yet)
- Not legal or compliance advice
- Not a claim that any deployed system currently conforms

## License & Notices

© 2026 Remnant Fieldworks Inc. All rights reserved. The text of this draft
may be quoted and cited for review and critique purposes.
Remnant Fieldworks™, Proof Before Power™, Verification Before Execution™,
ExecutionProof™, and ProofRecord™ are trademarks or pending trademarks of
Remnant Fieldworks Inc. U.S. patent applications pending.

**Contact:** derek@ownerremnantfieldworks.com
