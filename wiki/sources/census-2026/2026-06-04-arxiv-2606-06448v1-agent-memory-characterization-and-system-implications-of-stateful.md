---
type: source
source_type: arxiv
title: "Agent Memory: Characterization and System Implications of Stateful Long-Horizon Workloads"
authors: Yasmine Omri, Ziyu Gan, Zachary Broveak, Robin Geens et al.
url: https://arxiv.org/abs/2606.06448v1
date: 2026-06-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 13
primary: cs.AI
tags: [recommendation-agents, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# Agent Memory: Characterization and System Implications of Stateful Long-Horizon Workloads

**arXiv:** [2606.06448v1](https://arxiv.org/abs/2606.06448v1) · 2026-06-04 · cs.AI
**Authors:** Yasmine Omri, Ziyu Gan, Zachary Broveak, Robin Geens et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM agents are increasingly deployed on long-horizon tasks requiring sustained reasoning over extended interaction histories. Realizing this at scale requires agents to persistently store, retrieve, and update their own memory across sessions. A rich ecosystem of agent memory systems has emerged spanning flat retrieval, LLM-mediated extraction, consolidating fact stores, and agentic control flows. Yet, their system-level behavior remains uncharacterized. We present the first systems characterization of agent memory. First, we introduce a system-oriented taxonomy classifying agent memory systems along four axes. Second, we build a phase-aware profiling harness attributing cost to construction, retrieval, and generation. Third, we characterize ten representative systems across two benchmark suites, uncovering how design choices shift cost across the write and read paths. Finally, we derive 10 system recommendations covering construction scheduling, capability floors, amortization via query volume, freshness-latency tradeoffs, and fleet-scale management.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.06448v1)
