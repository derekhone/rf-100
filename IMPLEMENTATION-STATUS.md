# RF-100 Implementation Status Notes

**Status date:** 2026-08-01

This document is informational. It does not amend RF-100 normative requirements and does not create a certification or conformance claim.

## ExecutionProof ProofRecord signing status

ExecutionProof has implemented and internally verified hardware-backed ML-DSA-65 signing for newly generated ProofRecords using AWS KMS.

The updated public wording is:

> ExecutionProof has implemented and internally verified hardware-backed ML-DSA-65 signing for newly generated ProofRecords using AWS KMS. A formal RF-100 §8.4 conformance claim remains pending independent external review.

## Relationship to RF-100

RF-100 §8.4 requires VDRs to be signed with an asymmetric digital signature scheme drawn from a documented, current national or international standard. RF-100 §8.8 requires gate signing keys to be protected in an HSM or equivalent isolation. Those normative requirements remain unchanged.

This implementation-status update removes the stale publisher note that ExecutionProof still needed to migrate from HMAC-only integrity or that hardened key custody remained pending. Hardened custody is now reported as implemented for newly generated ProofRecords through AWS KMS; independent external review remains pending.

## External review items still pending

Independent review should confirm:

- exactly which canonical ProofRecord payload is hashed;
- deterministic canonical serialization;
- algorithm and encoding identifiers;
- domain separation so the SHA-256 digest cannot be reused in another signing context;
- replay protection;
- key-version binding;
- active and retired public-key discovery;
- rotation, retirement, and revocation behavior;
- tamper-failure behavior for modified ProofRecords.

## Non-claim boundary

This note does not assert formal RF-100 §8.4 conformance. A formal claim remains pending independent external review and any other required controls assessment.
