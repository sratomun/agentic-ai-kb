---
type: entity
entity_type: benchmark
tags: [agents, benchmark]
created: 2026-06-21
updated: 2026-06-22
census_count: 21
---

# τ-bench (tau-bench)

*The original tool-agent-user benchmark for conversational tool use in customer-service settings — precursor to [[tau2-bench]].*

## What it is
τ-bench tests agents that must complete structured customer-service tasks through dialogue and tool calls in a single-control environment. Appears in ~21 of the 2026 H1 census papers as the baseline for service-agent evaluation; [[tau2-bench]] extends it with dual-control state and [[tau-trait]] adds human persona stress-testing.

## Why it matters
τ-bench is the evaluation foundation for a growing line of customer-service agent benchmarks — performance here is the baseline to beat, and it's directly relevant to enterprise deployments in HR service, payroll support, and customer-facing HCM workflows.

## Relationships
- evaluates [[tool-use]]
- successor [[tau2-bench]]
