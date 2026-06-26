---
type: source
source_type: arxiv
title: "Do More Agents Help? Controlled and Protocol-Aligned Evaluation of LLM Agent Workflows"
authors: Yuhang Fu, Ruishan Fang, Jiaqi Shao, Huiyu Zheng et al.
url: https://arxiv.org/abs/2606.05670v1
date: 2026-06-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-protocols, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Do More Agents Help? Controlled and Protocol-Aligned Evaluation of LLM Agent Workflows

**arXiv:** [2606.05670v1](https://arxiv.org/abs/2606.05670v1) · 2026-06-04 · cs.AI
**Authors:** Yuhang Fu, Ruishan Fang, Jiaqi Shao, Huiyu Zheng et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Does adding more agents help an LLM workflow once compared systems share the same benchmark loader, tool access, answer contract, usage accounting, and trajectory logging? We introduce BenchAgent, an evaluation framework that places single-agent, fixed multi-agent (MAS), and evolving MAS workflows under one normalized execution and logging protocol. BenchAgent evaluates these substrate-internal workflows across ten reasoning, coding, and tool-use benchmarks with GPT-4.1, and separately reports a Protocol-Aligned External (PAE) GAIA study of a runtime-generated workflow. Under SI conditions, at most one of six tested MAS exceeds the matched single-agent anchor on benchmark-balanced average accuracy: EvoAgent lies within the Wilson one-run guidance, while the remaining five trail by 2.56-11.29 points and occupy more expensive accuracy-cost trade-offs. On the PAE GAIA snapshot, a Claude-Code-style runtime workflow reaches 66.72% overall and 69.23% on Level 3, more than 20 points above the strongest non-Claude baseline, Jarvis, a fixed MAS.

## Graph
- **Concepts:** [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[claude]] · [[gaia-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.05670v1)
