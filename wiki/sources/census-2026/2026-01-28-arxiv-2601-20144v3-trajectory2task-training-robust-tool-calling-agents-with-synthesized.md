---
type: source
source_type: arxiv
title: "Trajectory2Task: Training Robust Tool-Calling Agents with Synthesized Yet Verifiable Data for Complex User Intents"
authors: Ziyi Wang, Yuxuan Lu, Yimeng Zhang, Pei Chen et al.
url: https://arxiv.org/abs/2601.20144v3
date: 2026-01-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.CL
tags: [tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Trajectory2Task: Training Robust Tool-Calling Agents with Synthesized Yet Verifiable Data for Complex User Intents

**arXiv:** [2601.20144v3](https://arxiv.org/abs/2601.20144v3) · 2026-01-28 · cs.CL
**Authors:** Ziyi Wang, Yuxuan Lu, Yimeng Zhang, Pei Chen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Tool-calling agents are increasingly deployed in real-world customer-facing workflows. Yet most studies on tool-calling agents focus on idealized settings with general, fixed, and well-specified tasks. In real-world applications, user requests are often (1) ambiguous, (2) changing over time, or (3) infeasible due to policy constraints, and training and evaluation data that cover these diverse, complex interaction patterns remain under-represented. To bridge the gap, we present Trajectory2Task, a verifiable data generation pipeline for studying tool use at scale under three realistic user scenarios: ambiguous intent, changing intent, and infeasible intents. The pipeline first conducts multi-turn exploration to produce valid tool-call trajectories. It then converts these trajectories into user-facing tasks with controlled intent adaptations. This process yields verifiable task that support closed-loop evaluation and training. We benchmark seven state-of-the-art LLMs on the generated complex user scenario tasks and observe frequent failures. Finally, using successful trajectories obtained from task rollouts, we fine-tune lightweight LLMs and find consistent improvements across all three conditions, along with better generalization to unseen tool-use domains, indicating stronger tool-calling ability.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.20144v3)
