---
type: source
source_type: arxiv
title: "Healthcare AI GYM for Medical Agents"
authors: Minbyul Jeong
url: https://arxiv.org/abs/2605.02943v1
date: 2026-05-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.LG
tags: [clinical-agents, agentic-rl, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Healthcare AI GYM for Medical Agents

**arXiv:** [2605.02943v1](https://arxiv.org/abs/2605.02943v1) · 2026-05-01 · cs.LG
**Authors:** Minbyul Jeong

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Clinical reasoning demands multi-step interactions -- gathering patient history, ordering tests, interpreting results, and making safe treatment decisions -- yet a unified training environment provides the breadth of clinical domains and specialized tools to train generalizable medical AI agents through reinforcement learning remains elusive. We present a comprehensive empirical study of multi-turn agentic RL for medical AI, built on \gym{}, a gymnasium-compatible environment spanning 10 clinical domains with 3.6K+ tasks, 135 domain-specific tools, and a knowledge base of 828K medical passages. Our analysis reveals that agentic multi-turn structure degrades into verbose single-turn monologues, characterized by monotonic length explosion and a simultaneous erosion of tool-use frequency. We characterize how this collapse, alongside distillation instability, stems from the misalignment of sparse terminal rewards with sequential clinical trajectories. We find that vanilla GRPO achieves strong final accuracy on some benchmarks but suffers from training instability, evidenced by significant oscillations in response length and prolonged convergence periods. To improve training efficiency and stability, we propose Turn-level Truncated On-Policy Distillation (TT-OPD), a self-distillation framework where a gradient-free EMA teacher leverages outcome-privileged information to provide dense, outcome-aware KL regularization at every conversation turn. TT-OPD achieves the best performance on 10 of 18 benchmarks with an average +3.9~pp improvement over the non-RL baseline with faster early convergence, controlled response length, and sustained multi-turn tool use.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.02943v1)
