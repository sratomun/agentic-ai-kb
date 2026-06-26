---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "On-Device Fine-Tuning via Backprop-Free Zeroth-Order Optimization"
authors: Prabodh Katti et al.
url: https://arxiv.org/abs/2511.11362v2
date: 2025-11-14
score: 4
primary: cs.LG
tags: [arxiv, auto-ingested, small-language-models, agent-memory, llm-as-judge, post-training]
---

# On-Device Fine-Tuning via Backprop-Free Zeroth-Order Optimization

**arXiv:** [2511.11362v2](https://arxiv.org/abs/2511.11362v2) · 2025-11-14 · cs.LG
**Authors:** Prabodh Katti et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
On-device fine-tuning is a critical capability for edge AI systems, which must support adaptation to different agentic tasks under stringent memory constraints. Conventional backpropagation (BP)-based training requires storing layer activations and optimizer states, a demand that can be only partially alleviated through checkpointing. In edge deployments in which the model weights must reside entirely in device memory, this overhead severely limits the maximum model size that can be deployed. Memory-efficient zeroth-order optimization (MeZO) alleviates this bottleneck by estimating gradients using forward evaluations alone, eliminating the need for storing intermediate activations or optimizer states. This enables significantly larger models to fit within on-chip memory, albeit at the cost of potentially longer fine-tuning wall-clock time. This paper first provides a theoretical estimate of the relative model sizes that can be accommodated under BP and MeZO training. We then numerically validate the analysis, demonstrating that MeZO exhibits accuracy advantages under on-device memory constraints, provided sufficient wall-clock time is available for fine-tuning.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[agent-memory]] · [[llm-as-judge]] · [[post-training]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2511.11362v2)
