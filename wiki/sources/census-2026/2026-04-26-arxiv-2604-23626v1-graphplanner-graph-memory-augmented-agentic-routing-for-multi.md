---
type: source
source_type: arxiv
title: "GraphPlanner: Graph Memory-Augmented Agentic Routing for Multi-Agent LLMs"
authors: Tao Feng, Haozhen Zhang, Zijie Lei, Peixuan Han et al.
url: https://arxiv.org/abs/2604.23626v1
date: 2026-04-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.CL
tags: [knowledge-graph, agentic-rl, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# GraphPlanner: Graph Memory-Augmented Agentic Routing for Multi-Agent LLMs

**arXiv:** [2604.23626v1](https://arxiv.org/abs/2604.23626v1) · 2026-04-26 · cs.CL
**Authors:** Tao Feng, Haozhen Zhang, Zijie Lei, Peixuan Han et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM routing has achieved promising results in integrating the strengths of diverse models while balancing efficiency and performance. However, to support more realistic and challenging applications, routing must extend into agentic LLM settings, where task planning, multi-round cooperation among heterogeneous agents, and memory utilization are indispensable. To address this gap, we propose GraphPlanner, a heterogeneous graph memory-augmented agentic router for multi-agent LLMs that generates routing workflows for each query and supports both inductive and transductive inference. GraphPlanner formulates workflow generation as a Markov Decision Process (MDP), where at each step it selects both the LLM backbone and the agent role, including Planner, Executor, and Summarizer. By leveraging a heterogeneous graph, denoted as GARNet, to capture interaction memories among queries, agents, and responses, GraphPlanner integrates historical memory and workflow memory into richer state representations. The entire pipeline is optimized with reinforcement learning, jointly improving task-specific performance and computational efficiency. We evaluate GraphPlanner across 14 diverse LLM tasks and demonstrate that: (1) GraphPlanner outperforms strong single-round and multi-round routers, improving accuracy by up to 9.3% while reducing GPU cost from 186.26 GiB to 1.04 GiB; (2) GraphPlanner generalizes robustly to unseen tasks and LLMs, exhibiting strong zero-shot capabilities; and (3) GraphPlanner effectively leverages historical memories, supporting both inductive and transductive inference for more adaptive routing. Our code for GraphPlanner is released at https://github.com/ulab-uiuc/GraphPlanner.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.23626v1)
