---
type: entity
entity_type: benchmark
tags: [agents, benchmark]
created: 2026-06-21
updated: 2026-06-22
---

# EnterpriseOps-Gym

*A hard enterprise agent benchmark: containerized sandbox with 164 DB tables, 512 tools, and 1,150 expert tasks across 8 verticals — top frontier model scores 37.4%.*

## What it is
EnterpriseOps-Gym provides a containerized test environment that mimics a real enterprise backend: 164 database tables, 512 available tools, and 1,150 expert-curated tasks across 8 business verticals. Claude Opus 4.5 (the top-performing model) scores 37.4%; agents also rarely refuse infeasible tasks.

## Why it matters
The most realistic published bar for enterprise agent readiness — and at 37.4% for the best available model, agents are nowhere near production-ready for complex enterprise workflows. The infeasibility finding is equally concerning: agents that don't know when to stop are a liability in any regulated environment.

## Relationships
- evaluates [[multi-agent-systems]]
- part of [[agent-evaluation]]
- stresses [[tool-use]]

## Cited by
<!-- Auto-maintained by the kg-curator skill: the highest-cited source notes that reference this node. -->
- [[2026-03-13-arxiv-2603-13594v1-enterpriseops-gym-stateful-agentic-planning]]
