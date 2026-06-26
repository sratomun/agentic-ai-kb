---
type: source
source_type: arxiv
title: "SAGE: Structure Aware Graph Expansion for Retrieval of Heterogeneous Data"
authors: Prasham Titiya, Rohit Khoja, Tomer Wolfson, Vivek Gupta et al.
url: https://arxiv.org/abs/2602.16964v1
date: 2026-02-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.IR
tags: [knowledge-graph, agentic-rag, arxiv, auto-ingested]
---

# SAGE: Structure Aware Graph Expansion for Retrieval of Heterogeneous Data

**arXiv:** [2602.16964v1](https://arxiv.org/abs/2602.16964v1) · 2026-02-18 · cs.IR
**Authors:** Prasham Titiya, Rohit Khoja, Tomer Wolfson, Vivek Gupta et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Retrieval-augmented question answering over heterogeneous corpora requires connected evidence across text, tables, and graph nodes. While entity-level knowledge graphs support structured access, they are costly to construct and maintain, and inefficient to traverse at query time. In contrast, standard retriever-reader pipelines use flat similarity search over independently chunked text, missing multi-hop evidence chains across modalities. We propose SAGE (Structure Aware Graph Expansion) framework that (i) constructs a chunk-level graph offline using metadata-driven similarities with percentile-based pruning, and (ii) performs online retrieval by running an initial baseline retriever to obtain k seed chunks, expanding first-hop neighbors, and then filtering the neighbors using dense+sparse retrieval, selecting k' additional chunks. We instantiate the initial retriever using hybrid dense+sparse retrieval for implicit cross-modal corpora and SPARK (Structure Aware Planning Agent for Retrieval over Knowledge Graphs) an agentic retriever for explicit schema graphs. On OTT-QA and STaRK, SAGE improves retrieval recall by 5.7 and 8.5 points over baselines.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.16964v1)
