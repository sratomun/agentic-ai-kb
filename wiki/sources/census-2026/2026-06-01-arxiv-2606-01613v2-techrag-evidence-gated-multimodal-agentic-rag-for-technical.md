---
type: source
source_type: arxiv
title: "TechRAG: Evidence-Gated Multimodal Agentic RAG for Technical Literature Reasoning"
authors: Kanwar Bharat Singh
url: https://arxiv.org/abs/2606.01613v2
date: 2026-06-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.IR
tags: [knowledge-graph, agentic-rag, multi-agent-systems, arxiv, auto-ingested]
---

# TechRAG: Evidence-Gated Multimodal Agentic RAG for Technical Literature Reasoning

**arXiv:** [2606.01613v2](https://arxiv.org/abs/2606.01613v2) · 2026-06-01 · cs.IR
**Authors:** Kanwar Bharat Singh

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
This paper presents an agentic multimodal retrieval-augmented generation (RAG) framework for domain-specific literature reasoning, instantiated on a curated corpus of several thousand papers in intelligent tires, vehicle dynamics, vehicle control, sensing, estimation, and machine learning. Unlike conventional single-pass RAG systems, the proposed architecture uses an autonomous, evidence-gated pipeline that classifies query intent, generates separate text and visual query rewrites, performs hybrid text retrieval with FAISS and BM25 followed by cross-encoder reranking, expands evidence through graph-guided chunk traversal over a Neo4j knowledge graph, and retrieves visual document evidence using ColSmol late-interaction embeddings with MUVERA fixed-dimensional encoding, approximate nearest-neighbor search, and MaxSim reranking. The framework scores evidence sufficiency using a 100-point rubric with hybrid rule-based/LLM review, retries retrieval through drift-guarded reformulation, searches external academic databases through optimize--search--vet loops, merges and deduplicates multimodal evidence, verifies citation integrity, and generates cited answers through Planner, Researcher, Writer, and Critic agents with self-correcting revision. Key contributions include: (i) a scalable multimodal retrieval architecture combining text, graph, and visual evidence over 40,000 document pages; (ii) an interpretable evidence sufficiency and retry mechanism; (iii) a multi-agent generation pipeline with evidence mapping and critic-driven revision; (iv) a domain knowledge graph with LLM-based entity extraction, OpenAlex author validation, and intra-corpus citation resolution; and (v) a route-dependent external search architecture for targeted literature expansion. The result is a practical, evidence-gated, multimodal agentic RAG architecture for technical reasoning over specialized research corpora.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.01613v2)
