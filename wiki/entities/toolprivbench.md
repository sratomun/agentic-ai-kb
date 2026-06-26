---
type: entity
entity_type: benchmark
tags: [benchmark, agents, security, tool-use, least-privilege, evaluation]
created: 2026-06-21
updated: 2026-06-22
---

# ToolPrivBench

*A 544-scenario benchmark for over-privileged tool selection — measuring whether agents unnecessarily reach for higher-privilege tools when lower-privilege alternatives suffice.*

## What it is
ToolPrivBench covers 544 scenarios across 8 application domains (Database and Business largest) and 5 risk types: Authority Escalation, Scope Expansion, Temporal Persistence, Safety Bypass, and Data Over-Exposure. Scenarios inject transient failures to test premature escalation; metrics are Over-Privileged Tool Use Rate (OPUR@k) and Pre-Escalation Exploration Depth (PED). All tools in each scenario are independently sufficient — only privilege level differs.

## Why it matters
Least-privilege tool use is to agents what IAM hygiene is to cloud: over-privileged agents in enterprise environments hand attackers unnecessary blast radius. The key finding — that safety alignment (AgentAlign) that lowers AgentHarm scores does not transfer to privilege discipline — means this risk can't be fixed by existing safety training.

## Relationships
- introduced by [[2026-06-18-arxiv-2606-20023v1-over-privileged-tool-selection]]
- evaluates [[agent-security]]
- evaluates [[tool-use]]

## Cited by
<!-- Auto-maintained by the kg-curator skill: the highest-cited source notes that reference this node. -->
- [[2026-06-18-arxiv-2606-20023v1-over-privileged-tool-selection]]
