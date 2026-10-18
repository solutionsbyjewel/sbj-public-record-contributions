# PRC-028 — BEREC Generative AI and Internet Openness: Governance Control Matrix

Source: *Comments on the Draft BEREC Report on the Impact of Generative AI on Internet Openness, BoR (26) 141*, submitted October 17, 2026.  
SBJ-hosted submission: https://berec-generative-ai.solutionsbyjewelaigovernance.workers.dev/  
BEREC draft report: https://www.berec.europa.eu/en/all-documents/berec/reports/draft-berec-report-on-the-impact-of-generative-ai-on-internet-openness

The matrix maps SBJ's five proposals to the comment references and the observable control or evidence properties stated in the submission. It does not add implementation requirements or imply BEREC adoption.

| Proposal in the submission | Comment references | Control or recommendation stated | Observable property stated in the submission |
|---|---|---|---|
| Control of delegated agent action as part of internet openness | 1.1, 2.1 | Users should be able to understand, bound, observe, stop, and reassess delegated agent action; assess deployments through agent identity, bounded authority, action records, independent stop, and reassessment after material changes. | Agent and execution-instance identity; action, target, tool, credential, time-window, and consequence bounds; user-reviewable consequential-action records; independent pause or revocation; review after model, tool, permission, or environment changes. |
| Control of delegated agent action as part of internet openness | 2.2, 4.1, 4.2, 6.1 | Account for agent configuration defaults and selection behavior; pair trust in delegation with verifiability; monitor how authority is defined, revoked, and evidenced. | Tools, connectors, service integrations, and permissions enabled at setup; accessible history of consequential actions, selected services, and relied-upon sources; point-of-selection disclosure of commercial relationships for consequential transactions; record of selection criteria. |
| Attributable authorization in agent protocols such as MCP and WebMCP | 3.2, 3.5 | For consequential MCP actions, authorization should be scoped to the user's grant, attributable to an agent and principal, revocable, and recorded server-side. Shared sessions should distinguish user actions from agent actions. | Authorization scope, agent/principal attribution, user revocation, server-side record; action attribution in shared sessions, confirmation before consequential steps, and a user-accessible session record. |
| Verifiable identification of automated clients and access purpose | 3.4, 3.6 | Identify the agent, operator, and access purpose; distinguish real-time retrieval on a user's instruction from training and search-indexing purposes. | Machine-readable client/operator identity and declared purpose; the submission also recommends records linking crawler identity, declared purpose, and the rights reservation observed at access. It notes that client authentication does not itself establish authorization. |
| A defined minimum set of user controls for AI agents | 5.1, 5.2 | Address transparency to both the delegating user and people or services contacted by the agent; make agent settings and controls concrete. | User visibility of authorized actions, services, and data; user-set limits; confirmation before consequential or irreversible actions; prompt revocation; accessible history; consideration of disclosure when an agent interacts with natural persons on the user's behalf. |
| Agent protocols in BEREC standards work and monitoring | 3.1, 3.3, 5.3, 6.1 | Extend protocol openness and standards engagement to governance of agent protocols and the forums that develop them; include agent authorization practices in follow-up monitoring. | Published decision procedures; voting allocation; contributor distribution; change records identifying who proposed and approved changes; process for security-relevant changes; monitoring of identification, delegated authority and revocation, and consequential-action records. |

## Relationship to SBJ architecture

The submission identifies related SBJ supporting practice. This matrix records the PRC-specific recommendations and does not reproduce or amend canonical architecture or Decision Record materials:

- [SBJ AI Governance Decision Record](https://github.com/solutionsbyjewel/sbj-ai-governance-decision-record)
- [SBJ AI Governance Architecture V1 repository](https://github.com/solutionsbyjewel/sbj-ai-governance-architecture-v1)

## Scope

This is an extraction from SBJ's submitted comments, not a separate standard, validated protocol, implementation specification, or validation result. It does not claim BEREC accepted, endorsed, or implemented the recommendations.
