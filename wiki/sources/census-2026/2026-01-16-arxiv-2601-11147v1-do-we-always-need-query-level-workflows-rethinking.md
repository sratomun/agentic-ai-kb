---
type: source
source_type: arxiv
title: "Do We Always Need Query-Level Workflows? Rethinking Agentic Workflow Generation for Multi-Agent Systems"
authors: Zixu Wang, Bingbing Xu, Yige Yuan, Huawei Shen et al.
url: https://arxiv.org/abs/2601.11147v1
date: 2026-01-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-reliability, agentic-rl, multi-agent-systems, arxiv, auto-ingested]
---

# Do We Always Need Query-Level Workflows? Rethinking Agentic Workflow Generation for Multi-Agent Systems

**arXiv:** [2601.11147v1](https://arxiv.org/abs/2601.11147v1) · 2026-01-16 · cs.AI
**Authors:** Zixu Wang, Bingbing Xu, Yige Yuan, Huawei Shen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-Agent Systems (MAS) built on large language models typically solve complex tasks by coordinating multiple agents through workflows. Existing approaches generates workflows either at task level or query level, but their relative costs and benefits remain unclear. After rethinking and empirical analyses, we show that query-level workflow generation is not always necessary, since a small set of top-K best task-level workflows together already covers equivalent or even more queries. We further find that exhaustive execution-based task-level evaluation is both extremely token-costly and frequently unreliable. Inspired by the idea of self-evolution and generative reward modeling, we propose a low-cost task-level generation framework \textbf{SCALE}, which means \underline{\textbf{S}}elf prediction of the optimizer with few shot \underline{\textbf{CAL}}ibration for \underline{\textbf{E}}valuation instead of full validation execution. Extensive experiments demonstrate that \textbf{SCALE} maintains competitive performance, with an average degradation of just 0.61\% compared to existing approach across multiple datasets, while cutting overall token usage by up to 83\%.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.11147v1)
