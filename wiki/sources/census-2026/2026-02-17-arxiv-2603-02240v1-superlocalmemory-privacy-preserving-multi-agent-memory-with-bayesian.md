---
type: source
source_type: arxiv
title: "SuperLocalMemory: Privacy-Preserving Multi-Agent Memory with Bayesian Trust Defense Against Memory Poisoning"
authors: Varun Pratap Bhardwaj
url: https://arxiv.org/abs/2603.02240v1
date: 2026-02-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [knowledge-graph, agent-security, agent-protocols, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# SuperLocalMemory: Privacy-Preserving Multi-Agent Memory with Bayesian Trust Defense Against Memory Poisoning

**arXiv:** [2603.02240v1](https://arxiv.org/abs/2603.02240v1) · 2026-02-17 · cs.AI
**Authors:** Varun Pratap Bhardwaj

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We present SuperLocalMemory, a local-first memory system for multi-agent AI that defends against OWASP ASI06 memory poisoning through architectural isolation and Bayesian trust scoring, while personalizing retrieval through adaptive learning-to-rank -- all without cloud dependencies or LLM inference calls. As AI agents increasingly rely on persistent memory, cloud-based memory systems create centralized attack surfaces where poisoned memories propagate across sessions and users -- a threat demonstrated in documented attacks against production systems. Our architecture combines SQLite-backed storage with FTS5 full-text search, Leiden-based knowledge graph clustering, an event-driven coordination layer with per-agent provenance, and an adaptive re-ranking framework that learns user preferences through three-layer behavioral analysis (cross-project technology preferences, project context detection, and workflow pattern mining). Evaluation across seven benchmark dimensions demonstrates 10.6ms median search latency, zero concurrency errors under 10 simultaneous agents, trust separation (gap =0.90) with 72% trust degradation for sleeper attacks, and 104% improvement in NDCG@5 when adaptive re-ranking is enabled. Behavioral data is isolated in a separate database with GDPR Article 17 erasure support. SuperLocalMemory is open-source (MIT) and integrates with 17+ development tools via Model Context Protocol.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.02240v1)
