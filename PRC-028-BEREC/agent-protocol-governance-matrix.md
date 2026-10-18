# PRC-028 — BEREC Generative AI and Internet Openness: Governance Control Matrix

This matrix extracts the governance controls stated in SBJ's comments on the draft BEREC report. It is a navigational aid to the submitted recommendations, not a separate standard, validated protocol, or statement of BEREC adoption.

**Source contribution:** *Comments on the Draft BEREC Report on the Impact of Generative AI on Internet Openness, BoR (26) 141*  
**SBJ-hosted submission:** https://berec-generative-ai.solutionsbyjewelaigovernance.workers.dev/

| Source reference | Control stated in the submission | Context identified by the submission | Evidence or user-facing property stated in the submission |
|---|---|---|---|
| Comment 2.1 | Five observable elements for agent deployments: identity, bounded authority, action record, independent stop, and reassessment. | Agent deployments. | The deployment can be assessed against the five named elements; this row does not add thresholds or a test procedure. |
| Comment 3.2 | MCP authorization should be scoped to the user's grant, attributable to an identified agent and principal, revocable by the user, and recorded at the server. | Model Context Protocol (MCP) authorization. | Scope, attribution, revocation, and server-side record are the properties named in the comment. |
| Comment 3.5 | Attribute each action to the user or agent; require explicit confirmation before consequential steps; make the session record available to the user. | WebMCP and shared-session interactions. | Action attribution, confirmation before consequential steps, and an accessible session record. |
| Comment 3.6 | Make automated clients and their access purposes verifiably identifiable. | Automated clients accessing online services. | Verifiable client identification and stated access purpose. |
| Comment 5.2 | Provide visibility into granted authority, user-set limits, confirmation before irreversible actions, prompt revocation, and accessible history. | User controls for agent activity. | The five user controls enumerated in the comment. |
| Comment 3.3 | Make protocol governance observable through voting allocation, contributor diversity, and the adoption process for security-relevant changes. | Governance of relevant protocols. | Disclosure or examination of the three governance aspects named in the comment; no scoring method is specified here. |
| Comment 6.1 | Continue BEREC follow-up monitoring of the issues discussed in the submission. | BEREC's ongoing consideration of generative AI and internet openness. | Follow-up monitoring is the recommendation; this matrix does not assert that monitoring has been adopted or performed. |

## Relationship to SBJ architecture

The submission's recommendations intersect with SBJ's existing governance concepts. This file records the PRC-specific control statements and does not reproduce or amend canonical architecture or Decision Record materials:

- [SBJ AI Governance Decision Record](https://github.com/solutionsbyjewel/sbj-ai-governance-decision-record)
- [SBJ AI Governance Architecture V1 repository](https://github.com/solutionsbyjewel/sbj-ai-governance-architecture-v1)

## Scope

The matrix is limited to the statements identified above in the SBJ submission. It does not claim that BEREC accepted, endorsed, or implemented them. It does not introduce implementation details, metrics, test results, or validation findings beyond the source contribution.
