---
type: source
source_type: arxiv
title: "Exploring Agentic Tool-Calling Decisions via Uncertainty-Aligned Reinforcement Learning"
authors: Yijin Zhou, Linqian Zeng, Xiaoya Lu, Wenyuan Xie et al.
url: https://arxiv.org/abs/2606.06976v1
date: 2026-06-05
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [agent-reliability, agentic-rl, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Exploring Agentic Tool-Calling Decisions via Uncertainty-Aligned Reinforcement Learning

**arXiv:** [2606.06976v1](https://arxiv.org/abs/2606.06976v1) · 2026-06-05 · cs.AI
**Authors:** Yijin Zhou, Linqian Zeng, Xiaoya Lu, Wenyuan Xie et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language model (LLM)-based agents often make suboptimal tool-use decisions, including unsupported tool invocation and hallucinated direct responses, which may accumulate errors throughout multi-step interactions. Existing approaches mainly improve these behaviors through inference-time correction or coarse-grained reward signals based on decision outcomes and structured checklists, leaving the uncertainty characteristics of agent decisions underexplored. We observe that decision-oriented reinforcement learning tends to weaken the uncertainty separation between correct and incorrect actions, resulting in overconfident mistakes and weaker exploration signals. Therefore, we propose TRUST, which incorporates uncertainty quantification into reward design as a repulsive force for maintaining uncertainty separation, and labels lightweight key-turn annotations for unified post-training of multi-turn trajectories. Experimental results across diverse tool-use benchmarks show that TRUST consistently enhances both decision quality and agent performance while maintaining more reliable uncertainty estimates during optimization.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.06976v1)
