---
type: source
source_type: arxiv
title: "Query-Efficient Agentic Graph Extraction Attacks on GraphRAG Systems"
authors: Shuhua Yang, Jiahao Zhang, Yilong Wang, Dongwon Lee et al.
url: https://arxiv.org/abs/2601.14662v2
date: 2026-01-21
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.AI
tags: [clinical-agents, knowledge-graph, agent-security, agentic-rag, agent-memory, arxiv, auto-ingested]
---

# Query-Efficient Agentic Graph Extraction Attacks on GraphRAG Systems

**arXiv:** [2601.14662v2](https://arxiv.org/abs/2601.14662v2) · 2026-01-21 · cs.AI
**Authors:** Shuhua Yang, Jiahao Zhang, Yilong Wang, Dongwon Lee et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Graph-based retrieval-augmented generation (GraphRAG) systems construct knowledge graphs over document collections to support multi-hop reasoning. While prior work shows that GraphRAG responses may leak retrieved subgraphs, the feasibility of query-efficient reconstruction of the hidden graph structure remains unexplored under realistic query budgets. We study a budget-constrained black-box setting where an adversary adaptively queries the system to steal its latent entity-relation graph. We propose AGEA (Agentic Graph Extraction Attack), a framework that leverages a novelty-guided exploration-exploitation strategy, external graph memory modules, and a two-stage graph extraction pipeline combining lightweight discovery with LLM-based filtering. We evaluate AGEA on medical, agriculture, and literary datasets across Microsoft-GraphRAG and LightRAG systems. Under identical query budgets, AGEA significantly outperforms prior attack baselines, recovering up to 90% of entities and relationships while maintaining high precision. These results demonstrate that modern GraphRAG systems are highly vulnerable to structured, agentic extraction attacks, even under strict query limits. The code is available at https://github.com/shuashua0608/AGEA.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-security|Agent security]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.14662v2)
