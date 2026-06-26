---
type: entity
entity_type: benchmark
tags: [benchmark, agents, tool-use, customer-service, evaluation]
created: 2026-06-21
updated: 2026-06-22
---

# τ²-Bench (tau2-bench)

*A customer-service tool-calling benchmark with dual-control state — both agent and user can change the underlying database, making tasks far harder than single-actor settings.*

## What it is
τ²-Bench (Barres et al., 2025) tests conversational agents in a dual-control environment where both the agent and the user can modify the underlying state. Each task provides a user goal, initial database state, domain policy, and a tool set; the agent completes it through structured dialogue and tool calls. LedgerAgent draws its Airline, Retail, and Telecom domains from τ²-Bench and reports pass^k (run-to-run consistency) as the primary metric.

## Why it matters
The dual-control design is the most realistic published simulation of enterprise service workflows — performance here maps directly to real-world agent reliability in customer-facing HCM or payroll support scenarios where customer actions invalidate agent assumptions mid-task.

## Relationships
- used by [[2026-06-18-arxiv-2606-20529v1-ledgeragent-policy-adherent-tool-calling]]
- evaluates [[tool-use]]
- evaluates [[agent-security]]
- precursor [[tau-bench]]

## Cited by
<!-- Auto-maintained by the kg-curator skill: the highest-cited source notes that reference this node. -->
- [[2026-06-18-arxiv-2606-20529v1-ledgeragent-policy-adherent-tool-calling]]
