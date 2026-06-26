---
type: source
source_type: arxiv
title: "Learning to Explore: Scaling Agentic Reasoning via Exploration-Aware Policy Optimization"
authors: Xingyuan Hua, Sheng Yue, Ju Ren
url: https://arxiv.org/abs/2605.08978v2
date: 2026-05-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.AI
tags: [agentic-rl, agent-evaluation, arxiv, auto-ingested]
---

# Learning to Explore: Scaling Agentic Reasoning via Exploration-Aware Policy Optimization

**arXiv:** [2605.08978v2](https://arxiv.org/abs/2605.08978v2) · 2026-05-09 · cs.AI
**Authors:** Xingyuan Hua, Sheng Yue, Ju Ren

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advancements in agentic test-time scaling allow models to gather environmental feedback before committing to final actions. A key limitation of existing methods is that they typically employ undifferentiated exploration strategies, lacking the ability to adaptively distinguish when exploration is truly required. In this paper, we propose an exploration-aware reinforcement learning framework that enables LLM agents to adaptively explore only when uncertainty is high. Our method introduces a fine-grained reward function via variational inference that explicitly evaluates exploratory actions by estimating their potential to improve future decision-making, together with an exploration-aware grouping mechanism that separates exploratory actions from task-completion actions during optimization. By targeting informational gaps, this design allows agents to explore selectively and transition to execution as soon as the task context is clear. Empirically, we demonstrate that our approach achieves consistent improvements across a range of challenging text-based and GUI-based agent benchmarks. Code is available at https://github.com/HansenHua/EAPO-ICML26 and models are available at https://huggingface.co/hansenhua/EAPO-ICML26.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.08978v2)
