---
type: source
source_type: arxiv
title: "Trust-Aware Multi-Agent Traceability: Confidence-Calibrated Knowledge Graphs for Consistent Software Artifact Management"
authors: Mohamed Essam, Kareem Wael, Azza Hassan, Ahmed Haitham et al.
url: https://arxiv.org/abs/2606.17203v1
date: 2026-06-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.SE
tags: [coding-agents, knowledge-graph, agent-security, agent-protocols, agent-memory, arxiv, auto-ingested]
---

# Trust-Aware Multi-Agent Traceability: Confidence-Calibrated Knowledge Graphs for Consistent Software Artifact Management

**arXiv:** [2606.17203v1](https://arxiv.org/abs/2606.17203v1) · 2026-06-15 · cs.SE
**Authors:** Mohamed Essam, Kareem Wael, Azza Hassan, Ahmed Haitham et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-agent AI systems are increasingly used to automate software engineering tasks including requirements analysis, architecture design, test generation, and traceability linking. When these agents operate as a sequential pipeline over shared software artifacts, errors and low-confidence decisions made by upstream agents propagate to downstream stages, producing orphaned requirements, contradictory links, and compliance gaps that pose significant risks in safety-critical domains. We propose a trust-aware coordination framework where a shared knowledge graph serves as both centralized semantic memory and a coordination surface through which agents assess and build upon each other's contributions using calibrated confidence scores. Our approach introduces a two-stage traceability link prediction pipeline combining embedding-based retrieval with LLM-based multi-criteria analysis, a traceability seeding mechanism that enables comparison between derivation-time and validation-time confidence, and a consistency protocol governing pipeline interactions through confidence threshold gating, confidence divergence detection, and conflict resolution. We evaluate on an automotive software engineering case study measuring link prediction calibration, protocol effectiveness, threshold sensitivity, and the impact of traceability seeding. Ablation studies confirm that confidence calibration is essential for effective pipeline coordination.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.17203v1)
