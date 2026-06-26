---
type: source
source_type: arxiv
title: "Lemon Agent Technical Report"
authors: Haipeng Jiang, Kailong Ren, Zimo Yin, Zhetao Sun et al.
url: https://arxiv.org/abs/2602.07092v1
date: 2026-02-06
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.MA
tags: [self-evolving-agents, agent-protocols, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Lemon Agent Technical Report

**arXiv:** [2602.07092v1](https://arxiv.org/abs/2602.07092v1) · 2026-02-06 · cs.MA
**Authors:** Haipeng Jiang, Kailong Ren, Zimo Yin, Zhetao Sun et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advanced LLM-powered agent systems have exhibited their remarkable capabilities in tackling complex, long-horizon tasks. Nevertheless, they still suffer from inherent limitations in resource efficiency, context management, and multimodal perception. Based on these observations, Lemon Agent is introduced, a multi-agent orchestrator-worker system built on a newly proposed AgentCortex framework, which formalizes the classic Planner-Executor-Memory paradigm through an adaptive task execution mechanism. Our system integrates a hierarchical self-adaptive scheduling mechanism that operates at both the overall orchestrator layer and workers layer. This mechanism can dynamically adjust computational intensity based on task complexity. It enables orchestrator to allocate one or more workers for parallel subtask execution, while workers can further improve operational efficiency by invoking tools concurrently. By virtue of this two-tier architecture, the system achieves synergistic balance between global task coordination and local task execution, thereby optimizing resource utilization and task processing efficiency in complex scenarios. To reduce context redundancy and increase information density during parallel steps, we adopt a three-tier progressive context management strategy. To make fuller use of historical information, we propose a self-evolving memory system, which can extract multi-dimensional valid information from all historical experiences to assist in completing similar tasks. Furthermore, we provide an enhanced MCP toolset. Empirical evaluations on authoritative benchmarks demonstrate that our Lemon Agent can achieve a state-of-the-art 91.36% overall accuracy on GAIA and secures the top position on the xbench-DeepSearch leaderboard with a score of 77+.

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]] · [[gaia-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.07092v1)
