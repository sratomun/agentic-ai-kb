---
type: source
source_type: arxiv
title: "Do We Still Need GraphRAG? Benchmarking RAG and GraphRAG for Agentic Search Systems"
authors: Dongzhe Fan, Zheyi Xue, Siyuan Liu, Qiaoyu Tan
url: https://arxiv.org/abs/2604.09666v1
date: 2026-04-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 14
primary: cs.IR
tags: [knowledge-graph, agentic-rag, agent-evaluation, arxiv, auto-ingested]
---

# Do We Still Need GraphRAG? Benchmarking RAG and GraphRAG for Agentic Search Systems

**arXiv:** [2604.09666v1](https://arxiv.org/abs/2604.09666v1) · 2026-04-01 · cs.IR
**Authors:** Dongzhe Fan, Zheyi Xue, Siyuan Liu, Qiaoyu Tan

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Retrieval-augmented generation (RAG) and its graph-based extensions (GraphRAG) are effective paradigms for improving large language model (LLM) reasoning by grounding generation in external knowledge. However, most existing RAG and GraphRAG systems operate under static or one-shot retrieval, where a fixed set of documents is provided to the LLM in a single pass. In contrast, recent agentic search systems enable dynamic, multi-round retrieval and sequential decision-making during inference, and have shown strong gains when combined with vanilla RAG by introducing implicit structure through interaction. This progress raises a fundamental question: can agentic search compensate for the absence of explicit graph structure, reducing the need for costly GraphRAG pipelines? To answer this question, we introduce RAGSearch, a unified benchmark that evaluates dense RAG and representative GraphRAG methods as retrieval infrastructures under agentic search. RAGSearch covers both training-free and training-based agentic inference across multiple question answering benchmarks. To ensure fair and reproducible comparison, we standardize the LLM backbone, retrieval budgets, and inference protocols, and report results on full test sets. Beyond answer accuracy, we report offline preprocessing cost, online inference efficiency, and stability. Our results show that agentic search substantially improves dense RAG and narrows the performance gap to GraphRAG, particularly in RL-based settings. Nevertheless, GraphRAG remains advantageous for complex multi-hop reasoning, exhibiting more stable agentic search behavior when its offline cost is amortized. Together, these findings clarify the complementary roles of explicit graph structure and agentic search, and provide practical guidance on retrieval design for modern agentic RAG systems.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.09666v1)
