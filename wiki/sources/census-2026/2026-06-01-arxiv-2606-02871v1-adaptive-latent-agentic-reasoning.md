---
type: source
source_type: arxiv
title: "Adaptive Latent Agentic Reasoning"
authors: Dongwon Jung, Peng Shi, Yi Zhang, Junshan Zhang et al.
url: https://arxiv.org/abs/2606.02871v1
date: 2026-06-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.CL
tags: [tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Adaptive Latent Agentic Reasoning

**arXiv:** [2606.02871v1](https://arxiv.org/abs/2606.02871v1) · 2026-06-01 · cs.CL
**Authors:** Dongwon Jung, Peng Shi, Yi Zhang, Junshan Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large reasoning models improve performance by generating extended chain-of-thought (CoT) reasoning, but this behavior becomes inefficient when applied to LLM agents. Current LLM agents often generate verbose textual reasoning at every decision step and allocate reasoning effort nearly uniformly across turns, leading to substantial inefficiency in multi-turn agentic trajectories. We propose Adaptive Latent Agentic Reasoning (ALAR), a dual-mode framework that uses compact latent reasoning for routine turns and selectively escalates to explicit chain-of-thought when deeper deliberation is needed. ALAR learns latent reasoning by using the agent's actions as supervision anchors and is further optimized to use latent reasoning when it is sufficient for task success and reserve explicit CoT for harder decisions. Experiments on agentic search and tool-use benchmarks show that ALAR maintains comparable or better task accuracy while substantially reducing generated tokens by up to 43.6% in search and 84.6% in tool use. These results demonstrate that ALAR improves the accuracy-efficiency trade-off of LLM agents by reducing unnecessary textual reasoning while preserving explicit deliberation for harder decision steps.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.02871v1)
