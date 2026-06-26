---
type: source
source_type: arxiv
title: "Samyama: A Unified Graph-Vector Database with In-Database Optimization, Agentic Enrichment, and Hardware Acceleration"
authors: Madhulatha Mandarapu, Sandeep Kunkunuru
url: https://arxiv.org/abs/2603.08036v2
date: 2026-03-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.DB
tags: [agent-reliability, agent-security, agentic-rag, agent-memory, arxiv, auto-ingested]
---

# Samyama: A Unified Graph-Vector Database with In-Database Optimization, Agentic Enrichment, and Hardware Acceleration

**arXiv:** [2603.08036v2](https://arxiv.org/abs/2603.08036v2) · 2026-03-09 · cs.DB
**Authors:** Madhulatha Mandarapu, Sandeep Kunkunuru

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Modern data architectures are fragmented across graph databases, vector stores, analytics engines, and optimization solvers, resulting in complex ETL pipelines and synchronization overhead. We present Samyama, a high-performance graph-vector database written in Rust that unifies these workloads into a single engine. Samyama combines a RocksDB-backed persistent store with a versioned-arena MVCC model, a vectorized query executor with 35 physical operators, a cost-based query planner with plan enumeration and predicate pushdown, a dedicated CSR-based analytics engine, and native RDF/SPARQL support. The system integrates 22 metaheuristic optimization solvers directly into its query language, implements HNSW vector indexing with Graph RAG capabilities, and introduces Agentic Enrichment for autonomous graph expansion via LLMs. The Enterprise Edition adds GPU acceleration via wgpu, production-grade observability, point-in-time recovery, and hardened high availability with HTTP/2 Raft transport. Our evaluation on commodity hardware (Mac Mini M4, 16 GB RAM) demonstrates: ingestion at 255K nodes/s (CPU) and 412K nodes/s (GPU-accelerated); 115K Cypher queries/sec at 1M nodes; 4.0-4.7x latency reduction from late materialization on multi-hop traversals; 8.2x GPU PageRank speedup at 1M nodes; and 100% LDBC Graphalytics validation (28/28 tests). These results demonstrate that a unified graph-vector-optimization engine can achieve competitive performance on commodity hardware while maintaining Rust's memory safety guarantees.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.08036v2)
