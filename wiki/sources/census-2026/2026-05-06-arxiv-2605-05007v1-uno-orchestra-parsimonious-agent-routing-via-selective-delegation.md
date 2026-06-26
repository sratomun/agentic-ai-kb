---
type: source
source_type: arxiv
title: "Uno-Orchestra: Parsimonious Agent Routing via Selective Delegation"
authors: Zhiqing Cui, Haotong Xie, Jiahao Yuan, Cheng Yang et al.
url: https://arxiv.org/abs/2605.05007v1
date: 2026-05-06
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Uno-Orchestra: Parsimonious Agent Routing via Selective Delegation

**arXiv:** [2605.05007v1](https://arxiv.org/abs/2605.05007v1) · 2026-05-06 · cs.AI
**Authors:** Zhiqing Cui, Haotong Xie, Jiahao Yuan, Cheng Yang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language model (LLM) multi-agent systems typically rely on rigid orchestration, committing either to flat per-query routing or to hand-engineered task decomposition, so decomposition depth, worker choice, and inference budget are not jointly optimized under one objective. We introduce Uno-Orchestra, a unified orchestration policy that selectively decomposes a task and dispatches each subtask to an admissible (model, primitive) pair, with both decisions learned together from curated RL trajectories grounded in real worker interactions. Against 22 baselines on a 13-benchmark suite spanning math, code, knowledge, long-context, and agentic tool-use, Uno-Orchestra reaches 77.0% macro pass@1, roughly 16% above the strongest workflow baseline, at roughly an order of magnitude lower per-query cost, advancing the accuracy-efficiency frontier of selective delegation.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.05007v1)
