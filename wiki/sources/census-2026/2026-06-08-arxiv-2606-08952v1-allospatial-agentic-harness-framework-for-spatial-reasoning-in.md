---
type: source
source_type: arxiv
title: "AlloSpatial: Agentic Harness Framework for Spatial Reasoning in Foundation Models"
authors: Shouwei Ruan, Bin Wang, Zhenyu Wu, Qihui Zhu et al.
url: https://arxiv.org/abs/2606.08952v1
date: 2026-06-08
ingested: 2026-06-21
depth: abstract
auto: true
score: 22
primary: cs.AI
tags: [agent-reliability, agentic-rl, tool-use, arxiv, auto-ingested]
---

# AlloSpatial: Agentic Harness Framework for Spatial Reasoning in Foundation Models

**arXiv:** [2606.08952v1](https://arxiv.org/abs/2606.08952v1) · 2026-06-08 · cs.AI
**Authors:** Shouwei Ruan, Bin Wang, Zhenyu Wu, Qihui Zhu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multimodal Foundation Models (MFMs) have made substantial progress, yet remain fragile in spatial reasoning over the physical world. A key bottleneck lies in their inability to transform local egocentric observations into a global allocentric spatial representation. To address this, we propose AlloSpatial, an agentic framework for allocentric spatial cognition in foundation models. AlloSpatial introduces World2Mind, a plug-and-play cognitive mapping sandbox that converts egocentric observations into structured allocentric priors, including Allocentric-Spatial Trees and route maps that support querying object topology, geometric relations, passability, and trajectories. To utilize these priors reliably under noisy reconstruction and ambiguous visual evidence, AlloSpatial introduces a Spatial Reasoning Harness for tool-use judgment, modality-decoupled cue collection, and geometry-semantic arbitration. We further internalize this process in Qwen3-VL through cold-start reinforcement learning with a harness-gated trajectory-level reward. Experiments on VSI-Bench and MindCube show that AlloSpatial improves proprietary models by 5%-18% in a training-free setting, while ASTs alone support strong spatial reasoning even when visual inputs are removed. The trained AlloSpatial agents further outperform larger general-purpose models and competitive spatial baselines, suggesting that structured allocentric representations, active tool use, and verifiable reasoning offer a promising route toward spatially capable foundation models.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.08952v1)
