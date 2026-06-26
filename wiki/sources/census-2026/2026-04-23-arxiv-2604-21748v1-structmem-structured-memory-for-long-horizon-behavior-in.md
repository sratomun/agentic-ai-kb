---
type: source
source_type: arxiv
title: "StructMem: Structured Memory for Long-Horizon Behavior in LLMs"
authors: Buqiang Xu, Yijun Chen, Jizhan Fang, Ruobin Zhong et al.
url: https://arxiv.org/abs/2604.21748v1
date: 2026-04-23
ingested: 2026-06-21
depth: abstract
auto: true
score: 2
primary: cs.CL
tags: [knowledge-graph, agent-memory, arxiv, auto-ingested]
---

# StructMem: Structured Memory for Long-Horizon Behavior in LLMs

**arXiv:** [2604.21748v1](https://arxiv.org/abs/2604.21748v1) · 2026-04-23 · cs.CL
**Authors:** Buqiang Xu, Yijun Chen, Jizhan Fang, Ruobin Zhong et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Long-term conversational agents need memory systems that capture relationships between events, not merely isolated facts, to support temporal reasoning and multi-hop question answering. Current approaches face a fundamental trade-off: flat memory is efficient but fails to model relational structure, while graph-based memory enables structured reasoning at the cost of expensive and fragile construction. To address these issues, we propose \textbf{StructMem}, a structure-enriched hierarchical memory framework that preserves event-level bindings and induces cross-event connections. By temporally anchoring dual perspectives and performing periodic semantic consolidation, StructMem improves temporal reasoning and multi-hop performance on \texttt{LoCoMo}, while substantially reducing token usage, API calls, and runtime compared to prior memory systems, see https://github.com/zjunlp/LightMem .

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.21748v1)
