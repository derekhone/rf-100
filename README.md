# RF-100 — Verified Execution Governance Standard

**Verification-first execution control for high-consequence systems.**

> "If it cannot be verified, it cannot execute."

---

> ## RF-100 v1.0 — Public Review Draft
>
> **Status: Draft; not yet a final standard or certification program.**
>
> This version incorporates findings from two independent structured-review
> memoranda. Publication does not imply endorsement, certification, or
> implementation conformance by any reviewer or outside organization.

---

## Status

- **Current Version:** v1.0 — Public Review Draft (second-pass corrected)
- **Published:** July 2026 (public review draft)
- **Publisher:** Remnant Fieldworks Inc.
- **Built on:** RF-000 (Proof Before Power™ Doctrine, published)
- **Certification:** None exists yet. RF-101 (assessment) and RF-102
  (certification) are under development. No party may claim RF-100
  certification or formal conformance at this maturity level. This draft is
  not final, frozen, certified, or approved by any external organization.

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
- **IPR commitment (draft):** [`IPR-COMMITMENT.md`](./IPR-COMMITMENT.md) — intended patent posture (royalty-free, scoped, reciprocal); draft pending counsel review
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
- ExecutionProof™ does not yet claim full RF-100 conformance. Asymmetric
  (8.4-conformant) signing and other required controls are not yet
  operational; a conformance claim will follow only when they are.
- No reviewer or outside organization has endorsed, certified, or approved
  this draft. Independent review findings were incorporated; that is not
  endorsement.

## License & Notices

© 2026 Remnant Fieldworks Inc. The **text of the RF-100 specification** is
released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/),
effective with this v1.0 release (see Section 0.1). This license applies
**only** to the specification text and grants **no** rights to Remnant
Fieldworks trademarks, service marks, certification marks, software, hosted
services, APIs, trade secrets, or patents — all of which are reserved.

Remnant Fieldworks™, Proof Before Power™, Verification Before Execution™,
ExecutionProof™, VaultProof™, and ProofRecord™ are trademarks or pending
trademarks of Remnant Fieldworks Inc. U.S. patent applications pending.

**Patent / IPR commitment (draft).** A draft IPR commitment describing the
intended patent posture — a **royalty-free, scoped, reciprocal (defensive)
non-assertion covenant** for conforming implementations, with all rights
reserved for trademarks, products, hosted services, reference code, and the
certification program — is published as
[`IPR-COMMITMENT.md`](./IPR-COMMITMENT.md). It is a **draft pending legal /
patent counsel review**; the binding version will be finalized before any
certification program (RF-101 / RF-102) launches. In short: **anyone may
implement RF-100 freely; no one may copy the ExecutionProof/VaultProof
products, brands, or certification authority.**

**Contact:** derek@ownerremnantfieldworks.com
