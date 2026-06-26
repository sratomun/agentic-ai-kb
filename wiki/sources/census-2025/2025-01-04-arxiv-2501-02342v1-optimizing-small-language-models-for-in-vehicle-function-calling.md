---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Optimizing Small Language Models for In-Vehicle Function-Calling"
authors: Yahya Sowti Khiabani et al.
url: https://arxiv.org/abs/2501.02342v1
date: 2025-01-04
score: 1
primary: cs.LG
tags: [arxiv, auto-ingested, small-language-models, tool-use, post-training, autonomous-driving-agents]
---

# Optimizing Small Language Models for In-Vehicle Function-Calling

**arXiv:** [2501.02342v1](https://arxiv.org/abs/2501.02342v1) · 2025-01-04 · cs.LG
**Authors:** Yahya Sowti Khiabani et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We propose a holistic approach for deploying Small Language Models (SLMs) as function-calling agents within vehicles as edge devices, offering a more flexible and robust alternative to traditional rule-based systems. By leveraging SLMs, we simplify vehicle control mechanisms and enhance the user experience. Given the in-vehicle hardware constraints, we apply state-of-the-art model compression techniques, including structured pruning, healing, and quantization, ensuring that the model fits within the resource limitations while maintaining acceptable performance. Our work focuses on optimizing a representative SLM, Microsoft's Phi-3 mini, and outlines best practices for enabling embedded models, including compression, task-specific fine-tuning, and vehicle integration. We demonstrate that, despite significant reduction in model size which removes up to 2 billion parameters from the original model, our approach preserves the model's ability to handle complex in-vehicle tasks accurately and efficiently. Furthermore, by executing the model in a lightweight runtime environment, we achieve a generation speed of 11 tokens per second, making real-time, on-device inference feasible without hardware acceleration. Our results demonstrate the potential of SLMs to transform vehicle control systems, enabling more intuitive interactions between users and their vehicles for an enhanced driving experience.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[tool-use]] · [[post-training]] · [[autonomous-driving-agents]]
- **Entities:** [[phi]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2501.02342v1)
