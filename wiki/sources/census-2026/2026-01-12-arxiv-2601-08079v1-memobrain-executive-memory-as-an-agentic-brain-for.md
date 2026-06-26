---
type: source
source_type: arxiv
title: "MemoBrain: Executive Memory as an Agentic Brain for Reasoning"
authors: Hongjin Qian, Zhao Cao, Zheng Liu
url: https://arxiv.org/abs/2601.08079v1
date: 2026-01-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# MemoBrain: Executive Memory as an Agentic Brain for Reasoning

**arXiv:** [2601.08079v1](https://arxiv.org/abs/2601.08079v1) · 2026-01-12 · cs.AI
**Authors:** Hongjin Qian, Zhao Cao, Zheng Liu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Complex reasoning in tool-augmented agent frameworks is inherently long-horizon, causing reasoning traces and transient tool artifacts to accumulate and strain the bounded working context of large language models. Without explicit memory mechanisms, such accumulation disrupts logical continuity and undermines task alignment. This positions memory not as an auxiliary efficiency concern, but as a core component for sustaining coherent, goal-directed reasoning over long horizons. We propose MemoBrain, an executive memory model for tool-augmented agents that constructs a dependency-aware memory over reasoning steps, capturing salient intermediate states and their logical relations. Operating as a co-pilot alongside the reasoning agent, MemoBrain organizes reasoning progress without blocking execution and actively manages the working context. Specifically, it prunes invalid steps, folds completed sub-trajectories, and preserves a compact, high-salience reasoning backbone under a fixed context budget. Together, these mechanisms enable explicit cognitive control over reasoning trajectories rather than passive context accumulation. We evaluate MemoBrain on challenging long-horizon benchmarks, including GAIA, WebWalker, and BrowseComp-Plus, demonstrating consistent improvements over strong baselines.

## Graph
- **Concepts:** [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gaia-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.08079v1)
