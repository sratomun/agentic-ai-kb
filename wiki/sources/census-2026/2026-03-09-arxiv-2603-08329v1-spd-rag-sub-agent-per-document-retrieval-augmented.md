---
type: source
source_type: arxiv
title: "SPD-RAG: Sub-Agent Per Document Retrieval-Augmented Generation"
authors: Yagiz Can Akay, Muhammed Yusuf Kartal, Esra Alparslan, Faruk Ortakoyluoglu et al.
url: https://arxiv.org/abs/2603.08329v1
date: 2026-03-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.CL
tags: [agent-reliability, agentic-rag, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# SPD-RAG: Sub-Agent Per Document Retrieval-Augmented Generation

**arXiv:** [2603.08329v1](https://arxiv.org/abs/2603.08329v1) · 2026-03-09 · cs.CL
**Authors:** Yagiz Can Akay, Muhammed Yusuf Kartal, Esra Alparslan, Faruk Ortakoyluoglu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Answering complex, real-world queries often requires synthesizing facts scattered across vast document corpora. In these settings, standard retrieval-augmented generation (RAG) pipelines suffer from incomplete evidence coverage, while long-context large language models (LLMs) struggle to reason reliably over massive inputs. We introduce SPD-RAG, a hierarchical multi-agent framework for exhaustive cross-document question answering that decomposes the problem along the document axis. Each document is processed by a dedicated document-level agent operating only on its own content, enabling focused retrieval, while a coordinator dispatches tasks to relevant agents and aggregates their partial answers. Agent outputs are synthesized by merging partial answers through a token-bounded synthesis layer (which supports recursive map-reduce for massive corpora). This document-level specialization with centralized fusion improves scalability and answer quality in heterogeneous multidocument settings while yielding a modular, extensible retrieval pipeline. On the LOONG benchmark (EMNLP 2024) for long-context multi-document QA, SPD-RAG achieves an Avg Score of 58.1 (GPT-5 evaluation), outperforming Normal RAG (33.0) and Agentic RAG (32.8) while using only 38% of the API cost of a full-context baseline (68.0).

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.08329v1)
