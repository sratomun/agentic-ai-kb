---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "SOD: Step-wise On-policy Distillation for Small Language Model Agents"
authors: Qiyong Zhong et al.
url: https://arxiv.org/abs/2605.07725v1
date: 2026-05-08
score: 10
primary: cs.CL
tags: [arxiv, auto-ingested, small-language-models, tool-use, llm-as-judge, distillation, post-training]
---

# SOD: Step-wise On-policy Distillation for Small Language Model Agents

**arXiv:** [2605.07725v1](https://arxiv.org/abs/2605.07725v1) · 2026-05-08 · cs.CL
**Authors:** Qiyong Zhong et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Tool-integrated reasoning (TIR) is difficult to scale to small language models due to instability in long-horizon tool interactions and limited model capacity. While reinforcement learning methods like group relative policy optimization provide only sparse outcome-level rewards. Recently, on-policy distillation (OPD) has gained popularity by supplying dense token-level supervision from a teacher on student-generated trajectories. However, our experiments indicate that applying OPD to TIR leads to a critical failure mode: erroneous tool calls tend to cascade across subsequent reasoning steps, progressively amplifying student-teacher divergence and rendering the teacher's token-level supervision increasingly unreliable. To address this, we propose SOD, a step-wise on-policy distillation framework for small language model agents, which adaptively reweights distillation strength at each step based on step-level divergence. Therefore, SOD can attenuate potentially misleading teacher signals in high-divergence regions while preserving dense guidance in well-aligned states. Experiments on challenging math, science, and code benchmarks show that SOD achieves up to 20.86% improvement over the second-best baseline. Notably, our 0.6B student achieves 26.13% on AIME 2025, demonstrating effective transfer of agentic reasoning to lightweight models. Our code is available at https://github.com/YoungZ365/SOD.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[tool-use]] · [[llm-as-judge]] · [[distillation]] · [[post-training]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.07725v1)
