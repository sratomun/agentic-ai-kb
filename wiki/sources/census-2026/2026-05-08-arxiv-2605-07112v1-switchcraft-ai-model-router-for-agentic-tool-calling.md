---
type: source
source_type: arxiv
title: "Switchcraft: AI Model Router for Agentic Tool Calling"
authors: Sharad Agarwal, Pooria Namyar, Alec Wolman, Rahul Ambavat et al.
url: https://arxiv.org/abs/2605.07112v1
date: 2026-05-08
ingested: 2026-06-21
depth: abstract
auto: true
score: 22
primary: cs.AI
tags: [tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Switchcraft: AI Model Router for Agentic Tool Calling

**arXiv:** [2605.07112v1](https://arxiv.org/abs/2605.07112v1) · 2026-05-08 · cs.AI
**Authors:** Sharad Agarwal, Pooria Namyar, Alec Wolman, Rahul Ambavat et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic AI systems that invoke external tools are powerful but costly, leading developers to default to large models and overspend inference budgets. Model routing can mitigate this, but existing routers are designed for chat completion rather than tool use. We present Switchcraft, the first (to the best of our knowledge) model router optimized for agentic tool calling. Switchcraft operates inline, selecting the lowest-cost model subject to correctness. We construct an evaluation framework on five function-calling benchmarks and train a DistilBERT-based classifier, deployed under a latency budget. Switchcraft achieves 82.9% accuracy -- matching or exceeding the best individual model -- while reducing inference cost by 84%, saving over $3,600 per million queries. We find that larger models do not consistently outperform smaller ones on tool-use tasks, and that nominally cheaper models can incur higher total cost due to token-intensive reasoning. Our work enables cost-aware agentic AI deployment without sacrificing correctness.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.07112v1)
