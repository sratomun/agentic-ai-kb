---
type: source
source_type: arxiv
title: "Trace Only What You Need: Structure-Aware On-Demand Hypergraph Memory for Long-Document Question Answering"
authors: Xiangjun Zai, Xingyu Tan, Chen Chen, Xiaoyang Wang et al.
url: https://arxiv.org/abs/2606.10921v1
date: 2026-06-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 6
primary: cs.CL
tags: [knowledge-graph, agentic-rag, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# Trace Only What You Need: Structure-Aware On-Demand Hypergraph Memory for Long-Document Question Answering

**arXiv:** [2606.10921v1](https://arxiv.org/abs/2606.10921v1) · 2026-06-09 · cs.CL
**Authors:** Xiangjun Zai, Xingyu Tan, Chen Chen, Xiaoyang Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Long-document question answering (QA) requires large language models (LLMs) to reason over evidence scattered across lengthy documents, where answers often depend on event order, section-level context, and cross-part evidence connections. Although retrieval-augmented generation (RAG) reduces the input context by retrieving relevant evidence, existing structured RAG methods still face three limitations: costly query-agnostic knowledge organization, insufficient use of original document structure, and no reuse of historical reasoning experience. To address these limitations, we propose DocTrace, a multi-agent RAG framework for long-document QA that supports query-triggered knowledge organization, document-structure-aware and experience-guided reasoning. DocTrace preserves document hierarchy with a lightweight document structural tree index, constructs agent-shared hypergraph-structured working memory on demand during reasoning, and stores successful reasoning plans in graph-structured experience memory for future reuse, enabling adaptive exploration across related long-document questions. Experiments on four long-document QA datasets show that DocTrace achieves the best performance on three datasets, surpassing the strongest baseline, ComoRAG, by up to 8.85% in F1 and 4.40% in EM, while reducing the overall computational cost by 53.32%

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.10921v1)
