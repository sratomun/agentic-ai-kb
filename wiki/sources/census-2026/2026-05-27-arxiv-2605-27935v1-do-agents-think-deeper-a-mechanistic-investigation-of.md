---
type: source
source_type: arxiv
title: "Do Agents Think Deeper? A Mechanistic Investigation of Layer-Wise Dynamics in Sequential Planning"
authors: Zhenyu Cui, Xiangzhong Luo
url: https://arxiv.org/abs/2605.27935v1
date: 2026-05-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [coding-agents, tool-use, arxiv, auto-ingested]
---

# Do Agents Think Deeper? A Mechanistic Investigation of Layer-Wise Dynamics in Sequential Planning

**arXiv:** [2605.27935v1](https://arxiv.org/abs/2605.27935v1) · 2026-05-27 · cs.AI
**Authors:** Zhenyu Cui, Xiangzhong Luo

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent mechanistic studies suggest that large language models (LLMs) may utilize their depth inefficiently in standard single-turn tasks. Whether this still holds in autonomous agent settings, where models must perform multi-turn planning, tool use, and iterative state updates, remains unclear. We study this question through a systematic layer-wise analysis of complete user-agent trajectories spanning three domains: Deep Research, Code Generation, and Tabular Processing. Using residual stream probes, causal layer-skipping interventions, and effective-depth measurements, we show that agentic reasoning exhibits a distinct depth profile from static tasks. As trajectories unfold, models progressively recruit more and deeper layers, with stronger long-range inter-layer dependencies emerging in later turns. At the same time, residual updates become increasingly correction-dominant, indicating a shift from stable feature accumulation toward repeated recalibration. Effective-depth analysis further reveals a substantial construction-refinement gap: semantic direction often forms relatively early, while deep layers remain necessary for stabilizing final outputs. Across model families, this gap is pronounced in Qwen and Minimax, whereas GLM shows a more domain-dependent depth allocation pattern. These results provide mechanistic evidence that autonomous LLM agents allocate depth adaptively as reasoning complexity grows.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[tool-use|Tool use]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.27935v1)
