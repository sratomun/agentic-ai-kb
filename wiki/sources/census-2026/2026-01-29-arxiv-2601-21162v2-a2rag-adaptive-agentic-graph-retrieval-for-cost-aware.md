---
type: source
source_type: arxiv
title: "A2RAG: Adaptive Agentic Graph Retrieval for Cost-Aware and Reliable Reasoning"
authors: Jiate Liu, Zebin Chen, Shaobo Qiao, Mingchen Ju et al.
url: https://arxiv.org/abs/2601.21162v2
date: 2026-01-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.IR
tags: [knowledge-graph, agent-reliability, agentic-rag, arxiv, auto-ingested]
---

# A2RAG: Adaptive Agentic Graph Retrieval for Cost-Aware and Reliable Reasoning

**arXiv:** [2601.21162v2](https://arxiv.org/abs/2601.21162v2) · 2026-01-29 · cs.IR
**Authors:** Jiate Liu, Zebin Chen, Shaobo Qiao, Mingchen Ju et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Graph Retrieval-Augmented Generation (Graph-RAG) enhances multihop question answering by organizing corpora into knowledge graphs and routing evidence through relational structure. However, practical deployments face two persistent bottlenecks: (i) mixed-difficulty workloads where one-size-fits-all retrieval either wastes cost on easy queries or fails on hard multihop cases, and (ii) extraction loss, where graph abstraction omits fine-grained qualifiers that remain only in source text. We present A2RAG, an adaptive-and-agentic GraphRAG framework for cost-aware and reliable reasoning. A2RAG couples an adaptive controller that verifies evidence sufficiency and triggers targeted refinement only when necessary, with an agentic retriever that progressively escalates retrieval effort and maps graph signals back to provenance text to remain robust under extraction loss and incomplete graphs. Experiments on HotpotQA and 2WikiMultiHopQA demonstrate that A2RAG achieves +9.9/+11.8 absolute gains in Recall@2, while cutting token consumption and end-to-end latency by about 50% relative to iterative multihop baselines.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agentic-rag|Agentic RAG]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.21162v2)
