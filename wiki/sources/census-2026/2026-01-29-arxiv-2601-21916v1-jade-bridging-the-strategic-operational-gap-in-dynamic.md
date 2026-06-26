---
type: source
source_type: arxiv
title: "JADE: Bridging the Strategic-Operational Gap in Dynamic Agentic RAG"
authors: Yiqun Chen, Erhan Zhang, Tianyi Hu, Shijie Wang et al.
url: https://arxiv.org/abs/2601.21916v1
date: 2026-01-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 25
primary: cs.AI
tags: [agentic-rl, agentic-rag, multi-agent-systems, arxiv, auto-ingested]
---

# JADE: Bridging the Strategic-Operational Gap in Dynamic Agentic RAG

**arXiv:** [2601.21916v1](https://arxiv.org/abs/2601.21916v1) · 2026-01-29 · cs.AI
**Authors:** Yiqun Chen, Erhan Zhang, Tianyi Hu, Shijie Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The evolution of Retrieval-Augmented Generation (RAG) has shifted from static retrieval pipelines to dynamic, agentic workflows where a central planner orchestrates multi-turn reasoning. However, existing paradigms face a critical dichotomy: they either optimize modules jointly within rigid, fixed-graph architectures, or empower dynamic planning while treating executors as frozen, black-box tools. We identify that this \textit{decoupled optimization} creates a ``strategic-operational mismatch,'' where sophisticated planning strategies fail to materialize due to unadapted local executors, often leading to negative performance gains despite increased system complexity. In this paper, we propose \textbf{JADE} (\textbf{J}oint \textbf{A}gentic \textbf{D}ynamic \textbf{E}xecution), a unified framework for the joint optimization of planning and execution within dynamic, multi-turn workflows. By modeling the system as a cooperative multi-agent team unified under a single shared backbone, JADE enables end-to-end learning driven by outcome-based rewards. This approach facilitates \textit{co-adaptation}: the planner learns to operate within the capability boundaries of the executors, while the executors evolve to align with high-level strategic intent. Empirical results demonstrate that JADE transforms disjoint modules into a synergistic system, yielding remarkable performance improvements via joint optimization and enabling a flexible balance between efficiency and effectiveness through dynamic workflow orchestration.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.21916v1)
