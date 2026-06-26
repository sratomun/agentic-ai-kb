---
type: source
source_type: arxiv
title: "Xiaomi OneVL: One-Step Latent Reasoning and Planning with Vision-Language Explanation"
authors: Jinghui Lu, Jiayi Guan, Zhijian Huang, Jinlong Li et al.
url: https://arxiv.org/abs/2604.18486v3
date: 2026-04-20
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.CV
tags: [autonomous-driving-agents, embodied-agents, agent-evaluation, arxiv, auto-ingested]
---

# Xiaomi OneVL: One-Step Latent Reasoning and Planning with Vision-Language Explanation

**arXiv:** [2604.18486v3](https://arxiv.org/abs/2604.18486v3) · 2026-04-20 · cs.CV
**Authors:** Jinghui Lu, Jiayi Guan, Zhijian Huang, Jinlong Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Chain-of-Thought (CoT) reasoning has become a powerful driver of trajectory prediction in VLA-based autonomous driving, yet its autoregressive nature imposes a latency cost that is prohibitive for real-time deployment. Latent CoT methods attempt to close this gap by compressing reasoning into continuous hidden states, but consistently fall short of their explicit counterparts. We suggest that this is due to purely linguistic latent representations compressing a symbolic abstraction of the world, rather than the causal dynamics that actually govern driving. Thus, we present OneVL (One-step latent reasoning and planning with Vision-Language explanations), a unified VLA and World Model framework that routes reasoning through compact latent tokens supervised by dual auxiliary decoders. Alongside a language decoder that reconstructs text CoT, we introduce a visual world model decoder that predicts future-frame tokens, forcing the latent space to internalize the causal dynamics of road geometry, agent motion, and environmental change. A three-stage training pipeline progressively aligns these latents with trajectory, language, and visual objectives, ensuring stable joint optimization. In inference, the auxiliary decoders are discarded, and all latent tokens are prefilled in a single parallel pass, matching the speed of answer-only prediction. Across four benchmarks, OneVL becomes the first latent CoT method to surpass explicit CoT, delivering superior accuracy at answer-only latency. These results show that with world model supervision, latent CoT produces more generalizable representations than verbose token-by-token reasoning. Code has been open-sourced to the community. Project Page: https://xiaomi-embodied-intelligence.github.io/OneVL

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[embodied-agents|Embodied agents]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[vla]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.18486v3)
