---
type: source
source_type: arxiv
title: "A Tale of Two Graphs: Separating Knowledge Exploration from Outline Structure for Open-Ended Deep Research"
authors: Zhuofan Shi, Ming Ma, Zekun Yao, Fangkai Yang et al.
url: https://arxiv.org/abs/2602.13830v1
date: 2026-02-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.IR
tags: [knowledge-graph, self-evolving-agents, agent-memory, arxiv, auto-ingested]
---

# A Tale of Two Graphs: Separating Knowledge Exploration from Outline Structure for Open-Ended Deep Research

**arXiv:** [2602.13830v1](https://arxiv.org/abs/2602.13830v1) · 2026-02-14 · cs.IR
**Authors:** Zhuofan Shi, Ming Ma, Zekun Yao, Fangkai Yang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Open-Ended Deep Research (OEDR) pushes LLM agents beyond short-form QA toward long-horizon workflows that iteratively search, connect, and synthesize evidence into structured reports. However, existing OEDR agents largely follow either linear ``search-then-generate'' accumulation or outline-centric planning. The former suffers from lost-in-the-middle failures as evidence grows, while the latter relies on the LLM to implicitly infer knowledge gaps from the outline alone, providing weak supervision for identifying missing relations and triggering targeted exploration. We present DualGraph memory, an architecture that separates what the agent knows from how it writes. DualGraph maintains two co-evolving graphs: an Outline Graph (OG), and a Knowledge Graph (KG), a semantic memory that stores fine-grained knowledge units, including core entities, concepts, and their relations. By analyzing the KG topology together with structural signals from the OG, DualGraph generates targeted search queries, enabling more efficient and comprehensive iterative knowledge-driven exploration and refinement. Across DeepResearch Bench, DeepResearchGym, and DeepConsult, DualGraph consistently outperforms state-of-the-art baselines in report depth, breadth, and factual grounding; for example, it reaches a 53.08 RACE score on DeepResearch Bench with GPT-5. Moreover, ablation studies confirm the central role of the dual-graph design.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-memory|Agent memory]]
- **Entities:** [[gpt-5]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.13830v1)
