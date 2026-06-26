---
type: source
source_type: arxiv
title: "SAGE-32B: Agentic Reasoning via Iterative Distillation"
authors: Basab Jha, Firoj Paudel, Ujjwal Puri, Ethan Henkel et al.
url: https://arxiv.org/abs/2601.04237v2
date: 2026-01-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-reliability, agent-evaluation, arxiv, auto-ingested]
---

# SAGE-32B: Agentic Reasoning via Iterative Distillation

**arXiv:** [2601.04237v2](https://arxiv.org/abs/2601.04237v2) · 2026-01-04 · cs.AI
**Authors:** Basab Jha, Firoj Paudel, Ujjwal Puri, Ethan Henkel et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We demonstrate SAGE-32B, a 32 billion parameter language model that focuses on agentic reasoning and long range planning tasks. Unlike chat models that aim for general conversation fluency, SAGE-32B is designed to operate in an agentic loop, emphasizing task decomposition, tool usage, and error recovery. The model is initialized from the Qwen2.5-32B pretrained model and fine tuned using Iterative Distillation, a two stage training process that improves reasoning performance through rigorously tested feedback loops. SAGE-32B also introduces an inverse reasoning approach, which uses a meta cognition head to forecast potential failures in the planning process before execution. On agentic reasoning benchmarks including MMLU-Pro, AgentBench, and MATH-500, SAGE-32B achieves higher success rates in multi tool usage scenarios compared to similarly sized baseline models, while remaining competitive on standard reasoning evaluations. Model weights are publicly released at https://huggingface.co/sagea-ai/sage-reasoning-32b

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[qwen]] · [[agentbench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.04237v2)
