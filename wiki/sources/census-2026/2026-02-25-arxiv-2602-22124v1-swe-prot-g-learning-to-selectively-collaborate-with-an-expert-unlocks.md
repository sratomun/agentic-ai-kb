---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "SWE-Protégé: Learning to Selectively Collaborate With an Expert Unlocks Small Language Models as Software Engineering Agents"
authors: Patrick Tser Jern Kon et al.
url: https://arxiv.org/abs/2602.22124v1
date: 2026-02-25
score: 9
primary: cs.SE
tags: [arxiv, auto-ingested, small-language-models, post-training, coding-agents]
---

# SWE-Protégé: Learning to Selectively Collaborate With an Expert Unlocks Small Language Models as Software Engineering Agents

**arXiv:** [2602.22124v1](https://arxiv.org/abs/2602.22124v1) · 2026-02-25 · cs.SE
**Authors:** Patrick Tser Jern Kon et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Small language models (SLMs) offer compelling advantages in cost, latency, and adaptability, but have so far lagged behind larger models on long-horizon software engineering tasks such as SWE-bench, where they suffer from pervasive action looping and low resolution rates. We introduce SWE-Protégé, a post-training framework that reframes software repair as an expert-protégé collaboration problem. In SWE-Protégé, an SLM remains the sole decision-maker while learning to selectively seek guidance from a strong expert model, recognize stalled states, and follow through on expert feedback. Our approach combines supervised fine-tuning on expert-augmented trajectories with agentic reinforcement learning that explicitly discourages degenerative looping and unproductive expert collaboration. We lightly post-train Qwen2.5-Coder-7B-Instruct to achieve 42.4% Pass@1 on SWE-bench Verified, a +25.4% improvement over the prior SLM state of the art, while using expert assistance sparsely (~4 calls per task and 11% of total tokens).

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[post-training]] · [[coding-agents]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.22124v1)
