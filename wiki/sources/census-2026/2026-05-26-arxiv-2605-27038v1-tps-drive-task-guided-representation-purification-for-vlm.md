---
type: source
source_type: arxiv
title: "TPS-Drive: Task-Guided Representation Purification for VLM-based Autonomous Driving"
authors: Jiaxiang Li, Yumao Liu, Ke Ma
url: https://arxiv.org/abs/2605.27038v1
date: 2026-05-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.RO
tags: [autonomous-driving-agents, agentic-rl, agent-security, agent-evaluation, arxiv, auto-ingested]
---

# TPS-Drive: Task-Guided Representation Purification for VLM-based Autonomous Driving

**arXiv:** [2605.27038v1](https://arxiv.org/abs/2605.27038v1) · 2026-05-26 · cs.RO
**Authors:** Jiaxiang Li, Yumao Liu, Ke Ma

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Vision-Language Models (VLMs) provide a promising foundation for autonomous driving planning, yet bridging semantic reasoning and precise 3D spatial forecasting remains a critical challenge. Existing representation strategies generally follow two paths: text-aligned methods flatten continuous spatial states into symbols, which compromises geometric structure and induces "spatial hallucinations"; dense visual methods preserve spatial topology but overwhelm standard tokenizers with redundant background textures, leading to "representation interference". To address these limitations, we introduce TPS-Drive, a novel framework centered on Task-Guided Representation Purification that empowers VLMs to Think in Purified Space. At its core, an Agent-Centric Tokenizer utilizes a task-guided vector quantization mechanism supervised by a frozen 3D detection head, which explicitly reallocates limited codebook capacity from pervasive static backgrounds to critical dynamic agents and effectively isolates spatial redundancy. Leveraging this purified spatial vocabulary, TPS-Drive employs a decoupled reasoning pipeline that sequentially performs scene understanding, future forecasting, and action generation. The framework is optimized via a progressive three-stage training paradigm, culminating in reward-driven refinement that surpasses pure imitation learning. Extensive experiments validate our approach: TPS-Drive achieves accurate agent spatial state forecasting and reduces collision rates in open-loop nuScenes evaluations, while establishing new safety records on the rigorous closed-loop NAVSIMv1 and NAVSIMv2 benchmarks.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.27038v1)
