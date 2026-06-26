---
type: source
source_type: arxiv
title: "Signals: Trajectory Sampling and Triage for Agentic Interactions"
authors: Shuguang Chen, Adil Hafeez, Salman Paracha
url: https://arxiv.org/abs/2604.00356v1
date: 2026-04-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agentic-rl, agent-evaluation, arxiv, auto-ingested]
---

# Signals: Trajectory Sampling and Triage for Agentic Interactions

**arXiv:** [2604.00356v1](https://arxiv.org/abs/2604.00356v1) · 2026-04-01 · cs.AI
**Authors:** Shuguang Chen, Adil Hafeez, Salman Paracha

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic applications based on large language models increasingly rely on multi-step interaction loops involving planning, action execution, and environment feedback. While such systems are now deployed at scale, improving them post-deployment remains challenging. Agent trajectories are voluminous and non-deterministic, and reviewing each one, whether through human review or auxiliary LLMs, is slow and cost-prohibitive. We propose a lightweight, signal-based framework for triaging agentic interaction trajectories. Our approach computes cheap, broadly applicable signals from live interactions and attaches them as structured attributes for trajectory triage, identifying interactions likely to be informative without affecting online agent behavior. We organize signals into a coarse-grained taxonomy spanning interaction (misalignment, stagnation, disengagement, satisfaction), execution (failure, loop), and environment (exhaustion), designed for computation without model calls. In a controlled annotation study on $τ$-bench, a widely used benchmark for tool-augmented agent evaluation, we show that signal-based sampling achieves an 82\% informativeness rate compared to 74\% for heuristic filtering and 54\% for random sampling, with a 1.52x efficiency gain per informative trajectory. The advantage is robust across reward strata and task domains, confirming that signals provide genuine per-trajectory informativeness gains rather than merely oversampling obvious failures. These results show that lightweight signals can serve as practical sampling infrastructure for agentic systems, and suggest a path toward preference data construction and post-deployment optimization.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.00356v1)
