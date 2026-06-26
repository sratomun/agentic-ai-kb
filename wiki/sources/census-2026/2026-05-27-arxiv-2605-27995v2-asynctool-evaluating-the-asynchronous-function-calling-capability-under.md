---
type: source
source_type: arxiv
title: "AsyncTool: Evaluating the Asynchronous Function Calling Capability under Multi-Task Scenarios"
authors: Kou Shi, Ziao Zhang, Shiting Huang, Avery Nie et al.
url: https://arxiv.org/abs/2605.27995v2
date: 2026-05-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# AsyncTool: Evaluating the Asynchronous Function Calling Capability under Multi-Task Scenarios

**arXiv:** [2605.27995v2](https://arxiv.org/abs/2605.27995v2) · 2026-05-27 · cs.AI
**Authors:** Kou Shi, Ziao Zhang, Shiting Huang, Avery Nie et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language model (LLM)-based agents have shown strong capabilities in using external tools to solve complex tasks. However, existing evaluations often overlook the temporal dimension of tool use, especially the impact of tool response latency, and are usually limited to single-task settings. In real-world applications, multiple tasks often need to be executed concurrently, and overall efficiency depends on whether an agent can use idle time while waiting for tool responses. We refer to this capability as asynchronous tool calling. To evaluate it, we propose AsyncTool, a benchmark for assessing LLM-based agents in interactive multi-task tool-use environments with delayed tool feedback. AsyncTool presents multiple heterogeneous tasks simultaneously and simulates realistic tool response latency during execution. Using a hybrid data evolution strategy, we construct a diverse asynchronous multitasking dataset that covers multiple scenarios and tool-use patterns. We evaluate models at the step, sub-task, and task levels, and introduce efficiency-oriented metrics to measure task coordination and completion efficiency. Extensive experiments show that delayed tool feedback poses substantial challenges to current agents and leads to clear performance degradation. Models that better coordinate task switching, dependency tracking, and state maintenance achieve stronger performance on AsyncTool. Our analysis identifies key failure modes of current tool-using agents and provides practical insights for designing future systems with stronger temporal reasoning and coordination capabilities.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.27995v2)
