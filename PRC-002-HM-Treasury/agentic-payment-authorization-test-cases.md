# PRC-002 — HM Treasury Agentic Payments: Authorization and Evidence Test Cases

**Source contribution:** *Agentic Payments and AI Governance in UK Payments Regulation*, response to HM Treasury's *Modernising Payment Services Regulation Consultation*, Question 15 — Agentic Payments; submitted September 28, 2026.  
**SBJ-hosted submission:** https://hm-treasury-agentic-payments-uk.solutionsbyjewelaigovernance.workers.dev/

This artifact extracts the submission's five regulatory adaptation areas and its three illustrative agentic-payment pressure tests. The scenarios are proposed examples for testing evidence and authority questions; they are not executed tests, legal determinations, or observed payment incidents.

## Authorization and evidence model

The submission distinguishes three questions:

| Stage | Question | Evidence focus in the submission |
|---|---|---|
| Identity | Which autonomous actor or execution instance performed the action? | Agent identity, execution-instance attribution, and the actors in any delegation chain. |
| Authority | What was that actor permitted to do at that time? | The principal's grant and any applicable bounds, narrowing, expiry, revocation, delegation permission, or other material authority event. |
| Execution | What action actually occurred? | The payment instruction, transaction data, timestamps, and downstream execution evidence. |

Authentication or valid credentials alone do not establish that a particular execution remained within the authority granted by the payer.

## Five proposed clarification areas

| Submission recommendation | Governance or evidence question |
|---|---|
| Preserve the distinction between authentication and authority. | Can the record distinguish successful authentication from proof that the payer authorized the specific transaction or autonomous execution? |
| Clarify bounded prospective authority for autonomous agents. | Can the grant express relevant limits such as monetary or cumulative ceilings, transaction categories, purpose, payee or merchant restrictions, time limits, geographic restrictions, material commercial conditions, delegation permissions, expiry, and revocation? |
| Preserve delegated-authority provenance. | Can the origin, material scope, and relevant delegation history be established across principals, agents, services, and execution instances? |
| Evaluate authority at consequential execution. | Can the system determine whether the proposed execution remains within the authority currently applicable to that autonomous actor, including after narrowing, expiry, revocation, exhaustion, or material condition change? |
| Extend traceability to material authority events. | Can existing transaction traceability be extended, where necessary, to reconstruct the authority state and execution chain for dispute resolution, supervision, audit, or liability determination? |

## Illustrative pressure tests in the submission

| Scenario | Conditions stated in the submission | Question to resolve from evidence |
|---|---|---|
| A — Material condition drift | The payer authorizes an airfare up to GBP 1,200, nonstop, refundable, departing after 15:00. The agent buys a GBP 1,187 ticket from an acceptable merchant, but the fare is non-refundable and requires a connection. | Did the execution remain within the full grant, including conditions beyond the spending ceiling and merchant identity? |
| B — Delegated autonomous execution | Principal → Agent A → Agent B → payment service → execution. | Did Agent A have authority to delegate; what scope reached Agent B; did Agent B remain within that scope; and which execution instance performed the consequential action? |
| C — Authority invalidation | A business grants an autonomous procurement agent authority to make qualifying purchases up to GBP 10,000, later narrows the limit to GBP 5,000 while the workflow is offline, and the agent later attempts a GBP 7,800 payment using otherwise valid credentials. | Which authority state governed execution? The example distinguishes credential validity from current authority and tests propagation of a material authority change. |

## Evidence chain

The submission's representative traceability chain is:

**Principal → Authority Grant → Agent / Execution Instance → Delegation, if applicable → Authority Modification or Invalidation → Authority State at Execution → Payment Execution → Outcome**

The purpose is not indiscriminate logging. The submission calls for enough evidence to reconstruct the material authority and execution chain when needed.

## Regulatory placement

The submission proposes distributing outcomes across existing regulatory architecture: payment-services legislation and regulations for legal principles; FCA rules and technical standards for operational and evidentiary expectations; and industry standards for interoperable agent identity, machine-readable authority, delegation, revocation, and communication mechanisms. This file records the proposal and does not state that any change has been adopted.

## Relationship to SBJ architecture

The submission's authorization and evidence concepts align with existing SBJ materials. This artifact does not reproduce or amend those canonical materials:

- [SBJ AI Governance Decision Record](https://github.com/solutionsbyjewel/sbj-ai-governance-decision-record)
- [SBJ AI Governance Architecture V1 repository](https://github.com/solutionsbyjewel/sbj-ai-governance-architecture-v1)
