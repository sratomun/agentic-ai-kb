---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "ProST: Progressive Sub-task Training for Pareto-Optimal Multi-agent Systems Using Small Language Models"
authors: Biddut Sarker Bijoy et al.
url: https://arxiv.org/abs/2509.04508v2
date: 2025-09-02
score: 7
primary: cs.CL
tags: [arxiv, auto-ingested, small-language-models, post-training, multi-agent-systems]
---

# ProST: Progressive Sub-task Training for Pareto-Optimal Multi-agent Systems Using Small Language Models

**arXiv:** [2509.04508v2](https://arxiv.org/abs/2509.04508v2) · 2025-09-02 · cs.CL
**Authors:** Biddut Sarker Bijoy et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-agent systems with smaller language models (SLMs) present a viable alternative to single agent systems powered by large language models (LLMs) for addressing complex problems. In this work, we study how these alternatives compare in terms of both effectiveness and efficiency. To study this trade-off, we instantiate single and multi-agent systems for the complex problems in the AppWorld environment using different sized language models. We find that difficulties with long-trajectory learning in smaller language models (SLMs) limit their performance. Even when trained for specialized roles, SLMs fail to learn all subtasks effectively. To address this issue, we introduce a simple progressive sub-task training strategy, which introduces new sub-tasks progressively in each training epoch. We find that this novel strategy, analogous to instance level curriculum learning, consistently improves the effectiveness of multi-agents at all configurations. Our Pareto analysis shows that fine-tuned multi-agent systems yield better effectiveness-efficiency trade-offs. Additional ablations and analyses shows the importance of our progressive training strategy and its ability to reduce subtask error rates.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[post-training]] · [[multi-agent-systems]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2509.04508v2)
