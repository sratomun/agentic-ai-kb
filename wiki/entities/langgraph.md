---
type: entity
entity_type: framework
tags: [agents, framework]
created: 2026-06-21
updated: 2026-06-22
census_count: 39
---

# LangGraph

*A graph-based orchestration framework for stateful multi-agent LLM workflows — the practical default for teams building production pipelines that need explicit state management.*

## What it is
LangGraph models multi-agent workflows as directed graphs: nodes are agents or functions, edges are transitions, and the framework handles state persistence and control flow across parallel and sequential execution. It appears in ~39 of the 2026 H1 census papers as one of the most-cited named MAS frameworks.

## Why it matters
LangGraph's explicit state model addresses a key gap in simpler agent loops — it makes long-running, resumable, and human-in-the-loop workflows tractable. That makes it the framework to watch for enterprise deployments where workflow auditability and interruption are requirements.

## Relationships
- framework for [[multi-agent-systems]]
- relates to [[agent-protocols]]
