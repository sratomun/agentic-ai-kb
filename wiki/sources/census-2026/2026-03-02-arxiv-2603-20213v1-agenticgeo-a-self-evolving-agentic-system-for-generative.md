---
type: source
source_type: arxiv
title: "AgenticGEO: A Self-Evolving Agentic System for Generative Engine Optimization"
authors: Jiaqi Yuan, Jialu Wang, Zihan Wang, Qingyun Sun et al.
url: https://arxiv.org/abs/2603.20213v1
date: 2026-03-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.AI
tags: [self-evolving-agents, arxiv, auto-ingested]
---

# AgenticGEO: A Self-Evolving Agentic System for Generative Engine Optimization

**arXiv:** [2603.20213v1](https://arxiv.org/abs/2603.20213v1) · 2026-03-02 · cs.AI
**Authors:** Jiaqi Yuan, Jialu Wang, Zihan Wang, Qingyun Sun et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Generative search engines represent a transition from traditional ranking-based retrieval to Large Language Model (LLM)-based synthesis, transforming optimization goals from ranking prominence towards content inclusion. Generative Engine Optimization (GEO), specifically, aims to maximize visibility and attribution in black-box summarized outputs by strategically manipulating source content. However, existing methods rely on static heuristics, single-prompt optimization, or engine preference rule distillation that is prone to overfitting. They cannot flexibly adapt to diverse content or the changing behaviors of generative engines. Moreover, effectively optimizing these strategies requires an impractical amount of interaction feedback from the engines. To address these challenges, we propose AgenticGEO, a self-evolving agentic framework formulating optimization as a content-conditioned control problem, which enhances intrinsic content quality to robustly adapt to the unpredictable behaviors of black-box engines. Unlike fixed-strategy methods, AgenticGEO employs a MAP-Elites archive to evolve diverse, compositional strategies. To mitigate interaction costs, we introduce a Co-Evolving Critic, a lightweight surrogate that approximates engine feedback for content-specific strategy selection and refinement, efficiently guiding both evolutionary search and inference-time planning. Through extensive in-domain and cross-domain experiments on two representative engines, AgenticGEO achieves state-of-the-art performance and demonstrates robust transferability, outperforming 14 baselines across 3 datasets. Our code and model are available at: https://github.com/AIcling/agentic_geo.

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.20213v1)
