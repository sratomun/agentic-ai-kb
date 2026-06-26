---
type: source
source_type: arxiv
title: "VibeSearchBench: Benchmarking Long-horizon Proactive Search in the Wild"
authors: Xiaohongshu Inc
url: https://arxiv.org/abs/2605.27882v1
date: 2026-05-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 3
primary: cs.CL
tags: [knowledge-graph, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# VibeSearchBench: Benchmarking Long-horizon Proactive Search in the Wild

**arXiv:** [2605.27882v1](https://arxiv.org/abs/2605.27882v1) · 2026-05-27 · cs.CL
**Authors:** Xiaohongshu Inc

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM-based agents score well on search benchmarks, yet real users consistently find results unsatisfying, revealing a persistent evaluation-experience gap. We attribute this gap to existing benchmarks' reliance on over-specified queries, single-turn interactions, and fixed-schema evaluation, none of which reflect real search behavior where users and agents collaboratively refine vague intent through multi-turn dialogue. We term this paradigm VibeSearch and introduce VibeSearchBench, a benchmark comprising 200 manually curated bilingual (Chinese and English) tasks across 20 domains, split into VibeSearch-Pro (professional) and VibeSearch-Daily (daily-life) subsets. Each task pairs a user persona with a schema-free ground-truth knowledge graph, and is evaluated through a progressive-disclosure user simulator and a graph-matching evaluation framework. We benchmark seven frontier models under both the ReAct framework and the OpenClaw agent harness. Results show that all models remain substantially inadequate for VibeSearch (best F1: 30.30), highlighting the need for fundamental advances in long-context reasoning, proactive intent elicitation, and structured knowledge construction.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.27882v1)
