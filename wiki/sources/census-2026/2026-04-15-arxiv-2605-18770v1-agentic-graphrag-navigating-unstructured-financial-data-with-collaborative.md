---
type: source
source_type: arxiv
title: "Agentic GraphRAG: Navigating Unstructured Financial Data with Collaborative AI"
authors: Arthur Capozzi, Dirk Helbing
url: https://arxiv.org/abs/2605.18770v1
date: 2026-04-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.IR
tags: [finance-agents, knowledge-graph, human-agent-interaction, agent-protocols, agentic-rag, arxiv, auto-ingested]
---

# Agentic GraphRAG: Navigating Unstructured Financial Data with Collaborative AI

**arXiv:** [2605.18770v1](https://arxiv.org/abs/2605.18770v1) · 2026-04-15 · cs.IR
**Authors:** Arthur Capozzi, Dirk Helbing

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We present a collaborative agentic GraphRAG framework for expert analysis of commercial registry data. Public registries are often formally accessible, yet difficult to use in practice because they combine structured records with large volumes of unstructured legal text. This limits conventional keyword and vector-only retrieval, especially for multi-hop, temporal, and entity-centric investigations. Our approach builds a Neo4j knowledge graph through a three-phase pipeline: (i) deterministic ingestion of strong nodes from verified structured fields, (ii) LLM-based extraction of weak nodes from unstructured notices, and (iii) deterministic identity resolution and deduplication. On top of this graph, we introduce an analytical modular agent that integrates zero-shot intent routing, a bounded reflection loop, secure tool-mediated graph access, and state-aware response synthesis. A human-in-the-loop dashboard exposes evidence and execution traces to support transparency and auditability. We evaluate the framework on the Swiss Official Gazette of Commerce, a multilingual corpus of more than seven million publications over seven years. We further contribute a multi-tier evaluation protocol covering entity-resolution precision, tool-routing behavior, answer quality, and multi-turn conversational performance. Across automated, human-curated, and conversational benchmarks, the proposed agentic GraphRAG system consistently outperforms a standard agentic vector-RAG baseline, with strong gains in correctness, answer relevance, information recall, turn success rate, and context carryover accuracy. The architecture is modular, reproducible, and transferable to other commercial gazettes and public-sector registry systems.

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[knowledge-graph|Knowledge graphs]] · [[human-agent-interaction|Human-agent interaction]] · [[agent-protocols|Agent protocols]] · [[agentic-rag|Agentic RAG]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.18770v1)
