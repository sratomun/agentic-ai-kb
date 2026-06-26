---
type: source
source_type: arxiv
title: "Timely Machine: Awareness of Time Makes Test-Time Scaling Agentic"
authors: Yichuan Ma, Linyang Li, Yongkang chen, Peiji Li et al.
url: https://arxiv.org/abs/2601.16486v1
date: 2026-01-23
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.CL
tags: [agentic-rl, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Timely Machine: Awareness of Time Makes Test-Time Scaling Agentic

**arXiv:** [2601.16486v1](https://arxiv.org/abs/2601.16486v1) · 2026-01-23 · cs.CL
**Authors:** Yichuan Ma, Linyang Li, Yongkang chen, Peiji Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As large language models (LLMs) increasingly tackle complex reasoning tasks, test-time scaling has become critical for enhancing capabilities. However, in agentic scenarios with frequent tool calls, the traditional generation-length-based definition breaks down: tool latency decouples inference time from generation length. We propose Timely Machine, redefining test-time as wall-clock time, where models dynamically adjust strategies based on time budgets. We introduce Timely-Eval, a benchmark spanning high-frequency tool calls, low-frequency tool calls, and time-constrained reasoning. By varying tool latency, we find smaller models excel with fast feedback through more interactions, while larger models dominate high-latency settings via superior interaction quality. Moreover, existing models fail to adapt reasoning to time budgets. We propose Timely-RL to address this gap. After cold-start supervised fine-tuning, we use reinforcement learning to enhance temporal planning. Timely-RL improves time budget awareness and consistently boosts performance across Timely-Eval. We hope our work offers a new perspective on test-time scaling for the agentic era.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.16486v1)
