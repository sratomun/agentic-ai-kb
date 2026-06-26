---
type: source
source_type: arxiv
title: "Text Before Vision: Staged Knowledge Injection Matters for Agentic RLVR in Ultra-High-Resolution Remote Sensing Understanding"
authors: Fengxiang Wang, Mingshuo Chen, Yueying Li, Yajie Yang et al.
url: https://arxiv.org/abs/2602.14225v1
date: 2026-02-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.AI
tags: [knowledge-graph, agentic-rl, agent-evaluation, arxiv, auto-ingested]
---

# Text Before Vision: Staged Knowledge Injection Matters for Agentic RLVR in Ultra-High-Resolution Remote Sensing Understanding

**arXiv:** [2602.14225v1](https://arxiv.org/abs/2602.14225v1) · 2026-02-15 · cs.AI
**Authors:** Fengxiang Wang, Mingshuo Chen, Yueying Li, Yajie Yang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multimodal reasoning for ultra-high-resolution (UHR) remote sensing (RS) is usually bottlenecked by visual evidence acquisition: the model necessitates localizing tiny task-relevant regions in massive pixel spaces. While Agentic Reinforcement Learning with Verifiable Rewards (RLVR) using zoom-in tools offers a path forward, we find that standard reinforcement learning struggles to navigate these vast visual spaces without structured domain priors. In this paper, we investigate the interplay between post-training paradigms: comparing Cold-start Supervised Fine-Tuning (SFT), RLVR, and Agentic RLVR on the UHR RS benchmark.Our controlled studies yield a counter-intuitive finding: high-quality Earth-science text-only QA is a primary driver of UHR visual reasoning gains. Despite lacking images, domain-specific text injects the concepts, mechanistic explanations, and decision rules necessary to guide visual evidence retrieval.Based on this, we propose a staged knowledge injection recipe: (1) cold-starting with scalable, knowledge-graph-verified Earth-science text QA to instill reasoning structures;and (2) "pre-warming" on the same hard UHR image-text examples during SFT to stabilize and amplify subsequent tool-based RL. This approach achieves a 60.40% Pass@1 on XLRS-Bench, significantly outperforming larger general purpose models (e.g., GPT-5.2, Gemini 3.0 Pro, Intern-S1) and establishing a new state-of-the-art.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]] · [[gemini]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.14225v1)
