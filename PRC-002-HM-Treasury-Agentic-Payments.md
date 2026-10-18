# PRC-002 — HM Treasury: Agentic Payments

> **Draft review material. Not approved for public release.** This is an SBJ-authored summary of recommendations in the formal contribution; it is not an HM Treasury position or endorsement.

**Formal contribution:** [SBJ-hosted submission](https://hm-treasury-agentic-payments-uk.solutionsbyjewelaigovernance.workers.dev/)

## Technical substance identified

The submission organizes agentic payment governance around the sequence **identity → authority → execution** and makes five recommendations, including:

- distinguish authentication from authority;
- express prospective authority within explicit parameters, such as amount limits, transaction categories, purpose, payee, time, frequency, delegation, expiry, and revocation;
- retain delegation provenance;
- assess authority at consequential execution; and
- preserve transaction traceability for material authority events.

The parameter list summarizes the submission's examples; it is not a published schema or a claim that all payment systems expose these fields.

## Reuse opportunity

The sequence and recommendations provide a reusable framing for reviewing delegated transaction authority. This note does not claim a tested payment-control implementation or a validated transaction model.

## SBJ architecture references

Related concepts may be compared with SBJ's [AI Governance Decision Record](https://github.com/solutionsbyjewel/sbj-ai-governance-decision-record) and [AI Governance Architecture V1 repository](https://github.com/solutionsbyjewel/sbj-ai-governance-architecture-v1). These are references only; canonical materials are not copied.
