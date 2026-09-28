# Phase 5: AI and Agent Layer

## Objective
Add AI/agents after the deterministic platform is proven.

## Pattern
Event + Context -> AI/Agent -> Interpretation / Controlled Tool Call -> Rule or Human Approval -> Action

## Evaluation
- Usefulness
- Accuracy
- Latency
- Cost
- Privacy
- Reliability
- Failure behavior
- Auditability

## Open decisions
AI provider, local model, cloud model, context store, agent framework and tool permissions are TBD.

## Guardrail
AI should not have unrestricted authority to perform home actions. Actions pass through explicit policy, rule or approval boundaries.
