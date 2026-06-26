---
type: source
source_type: arxiv
title: "ByteRover: Agent-Native Memory Through LLM-Curated Hierarchical Context"
authors: Andy Nguyen, Danh Doan, Hoang Pham, Bao Ha et al.
url: https://arxiv.org/abs/2604.01599v1
date: 2026-04-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.AI
tags: [knowledge-graph, agent-reliability, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# ByteRover: Agent-Native Memory Through LLM-Curated Hierarchical Context

**arXiv:** [2604.01599v1](https://arxiv.org/abs/2604.01599v1) · 2026-04-02 · cs.AI
**Authors:** Andy Nguyen, Danh Doan, Hoang Pham, Bao Ha et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Memory-Augmented Generation (MAG) extends large language models with external memory to support long-context reasoning, but existing approaches universally treat memory as an external service that agents call into, delegating storage to separate pipelines of chunking, embedding, and graph extraction. This architectural separation means the system that stores knowledge does not understand it, leading to semantic drift between what the agent intended to remember and what the pipeline actually captured, loss of coordination context across agents, and fragile recovery after failures. In this paper, we propose ByteRover, an agent-native memory architecture that inverts the memory pipeline: the same LLM that reasons about a task also curates, structures, and retrieves knowledge. ByteRover represents knowledge in a hierarchical Context Tree, a file-based knowledge graph organized as Domain, Topic, Subtopic, and Entry, where each entry carries explicit relations, provenance, and an Adaptive Knowledge Lifecycle (AKL) with importance scoring, maturity tiers, and recency decay. Retrieval uses a 5-tier progressive strategy that resolves most queries at sub-100 ms latency without LLM calls, escalating to agentic reasoning only for novel questions. Experiments on LoCoMo and LongMemEval demonstrate that ByteRover achieves state-of-the-art accuracy on LoCoMo and competitive results on LongMemEval while requiring zero external infrastructure, no vector database, no graph database, no embedding service, with all knowledge stored as human-readable markdown files on the local filesystem.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.01599v1)
