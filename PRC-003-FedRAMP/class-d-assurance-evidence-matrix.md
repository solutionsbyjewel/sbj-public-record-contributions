# PRC-003 — FedRAMP RFC-0033: Class D Assurance Evidence Matrix

**Source contribution:** *Response to FedRAMP RFC-0033: 20x Phase 4 Development Tracks for 20x Class D*, dated October 7, 2026.  
**SBJ-hosted submission:** https://fedramp-rfc-0033-20x-class-d-assurance-governance-sbj-2026.solutionsbyjewelaigovernance.workers.dev/

This matrix extracts SBJ's five recommendations concerning operating-history continuity, inherited assurance, third-party resource dependencies, evidence provenance, and hosting-classification changes. The recommendations address anticipated Class D requirements and proposed Phase 4 work; they are SBJ's comments, not current FedRAMP requirements or adopted changes.

| Submission section | Proposed record or determination | Fields or conditions identified in the submission |
|---|---|---|
| 1. Operating History and Assurance-State Continuity | For each material assurance-state event, record whether operating-history evidence remains representative; document whether review is full or scoped and how the determination was reached. | Events include material changes to inherited security capabilities, the mechanisms producing Key Security Indicator measures, control responsibility, or a FedRAMP Reportable Incident affecting certification evidence. Examples discussed include adding, removing, or replacing a critical third-party service, replacing underlying management planes, and datacenter migration. |
| 2. Bounded Inheritance from Class D IaaS/PaaS | For each FedRAMP rule or Key Security Indicator relying on inherited assurance, identify the bounded inheritance and its reassessment conditions in the dependent provider's Security Decision Record. | Upstream offering; inherited rule, KSI, or capability; applicable resources and operating environment; responsibilities remaining with the dependent provider; supporting evidence; dependence on the upstream certification remaining in force; conditions requiring reassessment. The submission specifies machine-identifiable entries in the Security Decision Record JSON schema. |
| 3. Third-Party Resource Dependency Traceability | Associate each material third-party information resource with a structured dependency record. | Resource function; federal customer data or security property it could affect; capability or authority it holds relative to the cloud offering; assurance relied upon, including certification class; evidence establishing that assurance; compensating controls limiting dependency risk; and changes requiring reassessment. |
| 4. Evidence Provenance, Applicability, and Validity | Define minimum evidence-level fields for material Class D assurance evidence entering agency GRC systems. | The submission identifies record-level version, last-update date/time, and update source, and calls for evidence-level information including the applicable FedRAMP rule or KSI; generation method; verification and validation status; independent verification/validation status; dependency or inherited-assurance entry; period or conditions of validity; and the event or condition requiring regeneration or review. |
| 5. Hosting-Classification Changes | When hosting classification or physical-infrastructure responsibility changes materially, record a determination and resulting Security Decision Record updates. | Changed responsibilities; changed dependencies; changed inherited assurance; affected information flows; affected evidence; required independent reassessment; resulting Security Decision Record updates. The submission recommends a scoped review where existing evidence may remain applicable. |

## Cross-cutting evidence questions

The proposed records support these determinations, as stated in the submission:

- Does a material change alter the evidentiary basis for certification, and what evidence is needed to evaluate its effect?
- Which assurance is inherited, from what upstream offering, for which resources and conditions, and with what remaining dependent-provider responsibility?
- What material third-party resources affect customer data or security properties, and what assurance and compensating controls support reliance on them?
- Can evidence consumers distinguish provider verification/validation from independent verification/validation?
- After a hosting or responsibility transition, which prior assurance conclusions remain applicable, require scoped reassessment, or require new evaluation?

## Relationship to SBJ architecture

The submission applies concepts from SBJ's existing architecture and Decision Record materials. This file captures the RFC-0033-specific recommendations and does not reproduce or amend canonical materials:

- [SBJ AI Governance Decision Record](https://github.com/solutionsbyjewel/sbj-ai-governance-decision-record)
- [SBJ AI Governance Architecture V1 repository](https://github.com/solutionsbyjewel/sbj-ai-governance-architecture-v1)
