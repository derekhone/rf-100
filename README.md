# RF-100 — ExecutionProof Governance Standard (v0.9 DRAFT)

**Verification-first execution control for high-consequence systems.**

> "If it cannot be verified, it cannot execute."

## Status

- **Version:** v0.9 — PUBLIC DRAFT FOR REVIEW
- **Published:** July 2026
- **Publisher:** Remnant Fieldworks Inc.
- **Built on:** RF-000 (Proof Before Power™ Doctrine, published)
- **Certification:** None exists yet. RF-101 (assessment) and RF-102
  (certification) are under development. No party may claim RF-100
  certification or formal conformance at this maturity level.

## What RF-100 Is

RF-100 defines the minimum normative structure a high-consequence system —
AI agent, automated workflow, financial execution system, infrastructure
controller — MUST satisfy **before** a governed action executes.

It specifies ten elements, expressed as 39 numbered core requirements in
RFC 2119 (MUST/SHOULD/MAY) language, plus nine additional requirements in
the RF-100:AI conformance profile (Annex A):

1. Actor Identity
2. Authority (capability ≠ authority; self-approval blocking)
3. Policy
4. Evidence (stale evidence = absent; fail to HOLD/DENY)
5. System State (fail-closed)
6. Risk
7. Decision (ALLOW / HOLD / DENY — always before execution)
8. Proof Record (signed, tamper-evident, generated pre-execution)
9. Execution Outcome
10. Review Path

**Annex A** defines RF-100:AI, a conformance profile for AI agents and
autonomous systems, including agent-distinct identity, per-tool scoped
authority, extended self-approval blocking, intent records, consequence
thresholds, and velocity limits.

## Documents

- [`RF-100-v0.9-draft.pdf`](./RF-100-v0.9-draft.pdf) — the full draft standard
- Archived / citable version: Zenodo DOI — [LINK AFTER ZENODO UPLOAD]

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
