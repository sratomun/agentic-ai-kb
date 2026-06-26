---
type: source
source_type: arxiv
title: "RAGA: Reading-And-Graph-building-Agent for Autonomous Knowledge Graph Construction and Retrieval-Augmented Generation"
authors: Chengrui Han, Zesheng Cheng
url: https://arxiv.org/abs/2605.17072v1
date: 2026-05-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 5
primary: cs.AI
tags: [knowledge-graph, agentic-rag, governance-gap, arxiv, auto-ingested]
---

# RAGA: Reading-And-Graph-building-Agent for Autonomous Knowledge Graph Construction and Retrieval-Augmented Generation

**arXiv:** [2605.17072v1](https://arxiv.org/abs/2605.17072v1) · 2026-05-16 · cs.AI
**Authors:** Chengrui Han, Zesheng Cheng

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Existing LLM-driven knowledge graph (KG) construction methods predominantly employ stateless batch processing pipelines, exhibiting structural deficiencies in cross-chunk semantic relation capture, entity disambiguation, and construction process interpretability. These limitations undermine KG quality, retrieval precision, and deployment trust in high-stakes domains. We propose RAGA (Reading And Graph-building Agent), an LLM-based autonomous KG construction and retrieval fusion framework. RAGA provides an atomic toolset supporting full KG lifecycle CRUD operations and embeds a Read-Search-Verify-Construct cognitive constraint into a ReAct tool loop. A KG-vector synchronization mechanism enables hybrid symbolic-vector retrieval, while evidence-anchored verification links every knowledge entry to its source text for auditable provenance. Preliminary experiments on a subset of the QASPER scientific QA dataset indicate that RAGA's fusion retrieval outperforms zero-shot baselines, with KG integration providing measurable gains in both answer and evidence quality. The framework design and experimental baseline serve as a reference for agent-driven autonomous KG construction.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.17072v1)
