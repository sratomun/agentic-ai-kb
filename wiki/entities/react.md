---
type: entity
entity_type: method
tags: [method, agents, orchestration, tool-use, baseline]
created: 2026-06-21
updated: 2026-06-22
---

# ReAct

*The default LLM agent orchestration pattern: interleave reasoning and action in a continuous loop without upfront planning.*

## What it is
ReAct (Reasoning and Acting; Yao et al., 2023) is the baseline orchestration architecture for LLM agents — a single model emits a tool call, observes the result, reasons about the next step, and iterates until done. No upfront DAG planning. In the SAP enterprise study, ReAct on PydanticAI with parallel tool calling was compared against DAG Plan & Execute across 208 production-derived scenarios.

## Why it matters
At production scale, ReAct's incremental failure handling proved more robust than DAG planning — but it exposes deterministic stoppage points the SAP study used for Task-Manager preemption and merging. Any enterprise pipeline that needs safe interruption of running agents needs explicit hooks built on top of ReAct.

## Relationships
- used in [[multi-agent-systems]]
- baseline in [[2026-06-18-arxiv-2606-20058v1-event-driven-multi-agent-orchestration-enterprise]]
- relates to [[tool-use]]

## Cited by
<!-- Auto-maintained by the kg-curator skill: the highest-cited source notes that reference this node. -->
- [[2026-06-18-arxiv-2606-20058v1-event-driven-multi-agent-orchestration-enterprise]]
