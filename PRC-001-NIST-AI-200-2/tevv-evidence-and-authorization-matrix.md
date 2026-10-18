# PRC-001 — NIST AI 200-2: TEVV Evidence and Authorization Matrix

**Source contribution:** *Comments on NIST AI 200-2: The TEVV-Athlon Framework for Evaluating AI Systems*, submitted by Solutions by Jewel on October 6, 2026.  
**SBJ-hosted submission:** https://nist-ai-200-2-tevv-athlon-agentic-ai-evaluation-sbj-2026.solutionsbyjewelaigovernance.workers.dev/

This matrix extracts the four targeted enhancements in the submission and the evidence conditions it names. It records proposed additions to NIST AI 200-2; it is not a test result, benchmark, or claim of NIST adoption.

| Submission section | Proposed TEVV element | Evidence or evaluation conditions identified in the submission | Decision supported |
|---|---|---|---|
| 1. Associate TEVV evidence with system and operational context | Associate evaluation evidence with enough context to establish the conditions under which it applies. | System or model version; lifecycle stage; operational environment; material system configuration; enabled tools and external dependencies; relevant data or retrieval configuration; applicable permissions or action authority; other conditions needed to interpret the evaluated property. | Determine whether evidence generated under one configuration applies to the system and conditions under review. |
| 2. Treat authorization adherence as a measurable agentic-system property | Evaluate authorization adherence during ordinary operation where an agent can invoke tools, access external resources, delegate activity, or initiate consequential actions. | Whether an action was authorized; whether the authority was appropriate to the assigned objective; whether tool invocation stayed within permissions; whether delegated authority stayed within the originating boundary; whether approval or escalation conditions were observed; and whether downstream systems accepted or rejected actions consistently with applicable authority. | Assess adherence to the assigned action boundary alongside agent/tool-abuse testing. The submission proposes this as a candidate measurement concept or Metrology Block; it does not provide a validated metric or results. |
| 3. Operationalize material-change reassessment of existing TEVV evidence | Define conditions that trigger an evidence-applicability determination after system or deployment changes. | Changes potentially relevant to applicability include model version, enabled tools, permissions or action authority, delegation capability, operational environment, external dependencies, relevant retrieval or data sources, human-oversight configuration, or other characteristics materially related to the measurement concept. | Record one of four outcomes: existing evidence remains applicable; remains applicable subject to documented limitations; targeted reevaluation is necessary; or additional evaluation is required before the evidence can support the decision. |
| 4. Preserve sufficient execution provenance for agentic TEVV | Treat agentic execution provenance as supporting evidence within TEVV-Athlon. | Preserve provenance proportionate to the evaluation objective and risk so reviewers can interpret consequential evidence, establish represented systems and conditions, reproduce or investigate material results where feasible, identify relevant tools and dependencies, trace consequential actions, and support accountability across downstream components. | Establish how an outcome was produced and what configuration, authority, environment, and dependencies the evidence represents. |
| Application example: Physical and Embodied AI | Use a decision-to-effect chain to illustrate how evidence applicability, authority boundaries, reassessment, and provenance can converge. | Perception → planning → task/motion → low-level controller → actuator → physical effect; identify which portion of the chain the evaluation represents and the material conditions under which its evidence applies. | Illustrates the submission's proposed concepts; it is not presented as a separate validated test method. |

## Placement in the existing TEVV-Athlon stages

The submission places its recommendations within NIST AI 200-2's four-stage structure:

1. **Articulate & Organize:** identify material system and operational conditions, including authority conditions when the system can initiate consequential actions.
2. **Define & Construct:** where relevant, define authorization adherence, delegation integrity, consequential-action boundaries, or related characteristics as measurement concepts or Metrology Blocks.
3. **Apply & Measure:** associate results with sufficient system, execution, environmental, configuration, and authority context.
4. **Synthesize & Interrogate:** determine whether evidence remains applicable to the system under consideration and whether material changes require reassessment.

These are the submission's proposed applications of the existing stages, not a claim that NIST has incorporated them.

## Relationship to SBJ architecture

The submission links these proposals to SBJ governance concepts. This file records the contribution-specific mapping and does not reproduce or amend canonical materials:

- [SBJ AI Governance Decision Record](https://github.com/solutionsbyjewel/sbj-ai-governance-decision-record)
- [SBJ AI Governance Architecture V1 repository](https://github.com/solutionsbyjewel/sbj-ai-governance-architecture-v1)
