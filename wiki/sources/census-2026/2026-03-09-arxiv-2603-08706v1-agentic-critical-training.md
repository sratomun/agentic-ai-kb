---
type: source
source_type: arxiv
title: "Agentic Critical Training"
authors: Weize Liu, Minghui Liu, Sy-Tuyen Ho, Souradip Chakraborty et al.
url: https://arxiv.org/abs/2603.08706v1
date: 2026-03-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 23
primary: cs.AI
tags: [agentic-rl, agent-evaluation, arxiv, auto-ingested]
---

# Agentic Critical Training

**arXiv:** [2603.08706v1](https://arxiv.org/abs/2603.08706v1) · 2026-03-09 · cs.AI
**Authors:** Weize Liu, Minghui Liu, Sy-Tuyen Ho, Souradip Chakraborty et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Training large language models (LLMs) as autonomous agents often begins with imitation learning, but it only teaches agents what to do without understanding why: agents never contrast successful actions against suboptimal alternatives and thus lack awareness of action quality. Recent approaches attempt to address this by introducing self-reflection supervision derived from contrasts between expert and alternative actions. However, the training paradigm fundamentally remains imitation learning: the model imitates pre-constructed reflection text rather than learning to reason autonomously. We propose Agentic Critical Training (ACT), a reinforcement learning paradigm that trains agents to identify the better action among alternatives. By rewarding whether the model's judgment is correct, ACT drives the model to autonomously develop reasoning about action quality, producing genuine self-reflection rather than imitating it. Across three challenging agent benchmarks, ACT consistently improves agent performance when combined with different post-training methods. It achieves an average improvement of 5.07 points over imitation learning and 4.62 points over reinforcement learning. Compared to approaches that inject reflection capability through knowledge distillation, ACT also demonstrates clear advantages, yielding an average improvement of 2.42 points. Moreover, ACT enables strong out-of-distribution generalization on agentic benchmarks and improves performance on general reasoning benchmarks without any reasoning-specific training data, highlighting the value of our method. These results suggest that ACT is a promising path toward developing more reflective and capable LLM agents.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.08706v1)
