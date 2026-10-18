# PRC-005 — NIST SP 800-239: AI Data Center Authorization Controls Matrix

**Source contribution:** *AI Data Center Security Analysis: A High-Performance Computing (HPC) Driven Approach — Technical Comments on Authorization in AI Data Center Environments*, submitted September 22, 2026, on the initial public draft of NIST SP 800-239.  
**SBJ-hosted submission:** https://nist-sp-800-239-ai-data-center-security-public-comment.solutionsbyjewelaigovernance.workers.dev/

The submission contains six comments on authorization in AI data center environments. This matrix maps each comment to its NIST target, issue, and recommended action. It does not restate the submission's broader technical analysis or claim that NIST adopted the recommendations.

| Comment | NIST SP 800-239 target | Issue identified in the submission | Recommended action stated in the submission |
|---|---|---|---|
| 1 — Execution Instance Identity for Autonomous Agents | §3.9, Insider Threats (p. 15) | Treating autonomous agents as insiders does not bind a model or agent to a specific execution context or verify identity at the point of action. | Distinguish non-person actors from human insiders; require instance-level identity bound to execution context; acknowledge that non-person entity authentication remains an open issue in existing NIST zero-trust guidance. |
| 2 — Recovery, Replay, and Resumption Authorization | §4.5, Fault-Tolerant Workflow (p. 20) | Recovery, replay, and migration are addressed as correctness issues, without establishing whether resumed execution retains, inherits, or must re-establish prior authorization. | Add authorization to fault-tolerant workflow guidance and specify whether resumed executions operate under retained or re-established authorization. |
| 3 — Continuous Authorization and Authorization Invalidation | §4.3, Zero-Trust vs. Nurturing Trust (p. 19) | Continuous authorization is asserted without defining how authorization ends or reconciling that concept with the long-lived authorization model in the HPC overlay. | Reconcile with SP 800-234 re-authentication tailoring; distinguish invalidation from authentication; define invalidation conditions and their enforcement points. |
| 4 — Evidence Sufficiency and Decision-to-Action Traceability | §3.3, Regulatory and Compliance Challenges (pp. 11–12); §4.2 (pp. 18–19) | The submission identifies a chain-of-custody requirement without sufficient evidence or linkage from an authorization decision to an action. It also questions inherited HPC guidance that assigns compute-zone logging the lowest priority. | Link the authorization decision to the executing instance, action, and effect; reassess the priority of zone logging for AI data centers. |
| 5 — Environment as an Authorization Condition | §3.8, Multi-Tenant Threats (pp. 14–15) | Isolation is treated as a containment property, while execution environment is not treated as an input to the authorization decision at the granularity where resources are shared. | Treat execution environment as an authorization condition; address authorization validity when a workload is placed in or moved to a different execution environment. |
| 6 — Human-in-the-Loop Transition Authority | §4.4, Human-In-The-Loop Oversight (p. 19) | The submission identifies a human-approval mechanism without specifying which actions require approval, who holds authority, what evidence supports the decision, how it is recorded, or when authority lapses. | Specify the oversight mechanism's components and note the absence of an instantiating control in the inherited baseline. |

## Reusable review dimensions

Across the six comments, the submission identifies questions that can be applied when reviewing AI data center authorization controls:

- Is actor identity bound to the execution instance and context at the point of action?
- What authorization state governs recovery, replay, migration, and resumed execution?
- Which conditions invalidate or require reassessment of authorization, and where are they enforced?
- Can a consequential action be traced from its authorization decision through the execution instance to the effect?
- Does a change in execution environment alter the validity of the authorization decision?
- Are approval authority, evidence, recording, and lapse conditions specified for human-in-the-loop transitions?

## Relationship to SBJ architecture

The submission relates these comments to existing SBJ governance concepts. This matrix captures the contribution-specific mapping and does not reproduce or amend canonical materials:

- [SBJ AI Governance Decision Record](https://github.com/solutionsbyjewel/sbj-ai-governance-decision-record)
- [SBJ AI Governance Architecture V1 repository](https://github.com/solutionsbyjewel/sbj-ai-governance-architecture-v1)
