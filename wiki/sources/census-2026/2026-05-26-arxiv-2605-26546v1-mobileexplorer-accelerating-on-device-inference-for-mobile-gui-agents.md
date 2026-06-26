---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "MobileExplorer: Accelerating On-Device Inference for Mobile GUI Agents via Online Exploration"
authors: Runxi Huang et al.
url: https://arxiv.org/abs/2605.26546v1
date: 2026-05-26
score: 9
primary: cs.AI
tags: [arxiv, auto-ingested, small-language-models, agent-memory, llm-as-judge, post-training, reasoning-models]
---

# MobileExplorer: Accelerating On-Device Inference for Mobile GUI Agents via Online Exploration

**arXiv:** [2605.26546v1](https://arxiv.org/abs/2605.26546v1) · 2026-05-26 · cs.AI
**Authors:** Runxi Huang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Mobile graphical user interface (GUI) agents enable AI models to autonomously operate smartphones on behalf of users. However, most existing systems focus primarily on optimizing task accuracy and rely on cloud-hosted models for inference, which introduces privacy concerns and network-dependent latency. As a result, fully on-device deployment of mobile GUI agents remains underexplored. We propose MobileExplorer, a new framework that accelerates on-device inference for vision-based mobile GUI agents via online exploration. The key idea is to exploit the long per-step reasoning time of vision-language models (VLMs) by performing lightweight, parallel exploration of UI elements. During model inference, the agent proactively probes semantically relevant UI elements and records these exploration traces as structured memory. To ensure reliable execution in live mobile environments, we design a two-level rollback mechanism that robustly restores the initial UI state when a fast but naive backtracking strategy fails. The collected exploration traces are then summarized into concise contextual hints and injected into the prompt to enhance the subsequent reasoning step. We evaluate MobileExplorer on multiple off-the-shelf devices using the AndroidWorld benchmark, as well as newly designed, more complex tasks and dynamic on-device environments. MobileExplorer reduces the average number of reasoning steps and end-to-end latency by 23\%, while maintaining or improving task success rates by up to 5\%. A video demonstration of MobileExplorer performance in the real world is available at https://youtu.be/thK7MJmdlvM .

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[agent-memory]] · [[llm-as-judge]] · [[post-training]] · [[reasoning-models]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.26546v1)
