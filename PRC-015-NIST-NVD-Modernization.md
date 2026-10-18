# PRC-015 — NIST NVD Modernization in the Age of AI

> **Private review draft. Not approved for public release.** This SBJ-authored summary describes recommendations in SBJ’s contribution; it is not a NIST position, adopted control, or implementation result.

**Contribution reviewed:** Solutions by Jewel, response to the NIST RFI on Modernizing the National Vulnerability Database in the Age of Artificial Intelligence (Docket NIST-2026-0100). The SBJ-hosted public URL has not yet been verified for this draft and must be added before any public release.

## Technical substance identified

The response distinguishes the stages of AI-enabled vulnerability management:

**Identify → Enrich → Prioritize → Recommend → Authorize → Execute → Verify → Reassess**

Its central recommendation is that authority to identify, classify, prioritize, or recommend remediation does not by itself confer authority to execute a production change. It further recommends scaling authority to consequence; preserving decision-relevant evidence and provenance; reassessing decisions when relevant source, asset, dependency, or operating conditions materially change; and making consequential remediation bounded, traceable, verifiable, and interruptible.

For consequential decisions, the response lists information a reviewer may need, including evidence currency and source, affected product/version/environment, threat information, uncertainty, expected effects, validation, and rollback or termination mechanisms. It also proposes machine-readable provenance expectations for downstream systems.

## Gate assessment

**Provisional 4/5 — selective candidate.** The workflow separation and change-sensitive decision trace are reusable in vulnerability-management settings. The contribution contains concrete requirements but does not provide a tested schema or implementation. Publication readiness remains unverified: the source URL and any rights/attribution wording must be checked before publication.

## Reuse boundary

This note summarizes recommendations; it does not claim a tested remediation workflow or NIST adoption. Link to canonical SBJ architecture and Decision Record materials rather than copying them.
