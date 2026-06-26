---
type: source
source_type: arxiv
title: "PlugMem: A Task-Agnostic Plugin Memory Module for LLM Agents"
authors: Ke Yang, Zixi Chen, Xuan He, Jize Jiang et al.
url: https://arxiv.org/abs/2603.03296v1
date: 2026-02-06
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.CL
tags: [computer-use-agents, knowledge-graph, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# PlugMem: A Task-Agnostic Plugin Memory Module for LLM Agents

**arXiv:** [2603.03296v1](https://arxiv.org/abs/2603.03296v1) · 2026-02-06 · cs.CL
**Authors:** Ke Yang, Zixi Chen, Xuan He, Jize Jiang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Long-term memory is essential for large language model (LLM) agents operating in complex environments, yet existing memory designs are either task-specific and non-transferable, or task-agnostic but less effective due to low task-relevance and context explosion from raw memory retrieval. We propose PlugMem, a task-agnostic plugin memory module that can be attached to arbitrary LLM agents without task-specific redesign. Motivated by the fact that decision-relevant information is concentrated as abstract knowledge rather than raw experience, we draw on cognitive science to structure episodic memories into a compact, extensible knowledge-centric memory graph that explicitly represents propositional and prescriptive knowledge. This representation enables efficient memory retrieval and reasoning over task-relevant knowledge, rather than verbose raw trajectories, and departs from other graph-based methods like GraphRAG by treating knowledge as the unit of memory access and organization instead of entities or text chunks. We evaluate PlugMem unchanged across three heterogeneous benchmarks (long-horizon conversational question answering, multi-hop knowledge retrieval, and web agent tasks). The results show that PlugMem consistently outperforms task-agnostic baselines and exceeds task-specific memory designs, while also achieving the highest information density under a unified information-theoretic analysis. Code and data are available at https://github.com/TIMAN-group/PlugMem.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.03296v1)
