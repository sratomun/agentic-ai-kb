---
type: source
source_type: arxiv
title: "SAGE: Multi-Agent Self-Evolution for LLM Reasoning"
authors: Yulin Peng, Xinxin Zhu, Chenxing Wei, Nianbo Zeng et al.
url: https://arxiv.org/abs/2603.15255v2
date: 2026-03-16
ingested: 2026-06-21
depth: full-text
tags: [self-evolving-agents, multi-agent-systems, agentic-rl, arxiv]
---

# SAGE: Multi-Agent Self-Evolution for LLM Reasoning

**Why it matters:** Four co-evolving agents (Challenger/Planner/Solver/Critic) from one backbone, with the Critic preventing curriculum drift — a cleaner answer to self-play instability in long-horizon reasoning.

## Takeaways
- SAGE: Challenger generates harder tasks, Planner makes structured plans, Solver executes, Critic filters questions+plans to prevent curriculum drift — all from a shared LLM with a small seed set.
- Explicit planning + quality control address the stability gap in self-play RLVR.
- Qwen-2.5-7B: +8.9% LiveCodeBench, +10.7% OlympiadBench; consistent across scales.

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-rl|Agentic RL]]
- **Raw:** `raw/arxiv/2603.15255v2.md` · `raw/arxiv/2603.15255v2.fulltext.md`
