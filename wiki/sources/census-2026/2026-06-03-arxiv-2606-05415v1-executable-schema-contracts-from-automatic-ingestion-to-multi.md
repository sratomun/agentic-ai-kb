---
type: source
source_type: arxiv
title: "Executable Schema Contracts: From Automatic Ingestion to Multi-Source Retrieval"
authors: Padmaja Jonnalagedda, Yuguang Yao, Xiang Gao, Hilaf Hasson et al.
url: https://arxiv.org/abs/2606.05415v1
date: 2026-06-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 3
primary: cs.CL
tags: [knowledge-graph, agent-protocols, agent-evaluation, arxiv, auto-ingested]
---

# Executable Schema Contracts: From Automatic Ingestion to Multi-Source Retrieval

**arXiv:** [2606.05415v1](https://arxiv.org/abs/2606.05415v1) · 2026-06-03 · cs.CL
**Authors:** Padmaja Jonnalagedda, Yuguang Yao, Xiang Gao, Hilaf Hasson et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Real-world data spans tables, documents, and semi-structured files with implicit semantics. Querying this data requires integrating evidence across inconsistent schemas and formats, yet existing approaches either demand costly manual engineering or bypass structure entirely. We present a system that automatically discovers an executable schema from raw multi-source data and uses it as a shared contract for knowledge graph construction and query-time retrieval. A closed-world field catalog constrains LLM-based schema discovery to attested fields; deterministic structural analysis infers identity keys, foreign keys, and source hierarchy; and the resulting schema drives extraction, deduplication, and cross-source linking into a provenance-aware knowledge graph. At query time the schema -- optionally extended via a monotonic protocol -- conditions a multi-tool agent routing retrieval across structured lookup, graph traversal, and vector search, returning grounded answers with traceable citations. In controlled zero-shot comparisons using the same LLM, data, and evaluation harness, the system improves over retrieval-only and decomposition-based baselines across four QA benchmarks, with ablations showing that schema-conditioned routing, structural intelligence, and schema-guided construction each contribute to the gains.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-protocols|Agent protocols]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.05415v1)
