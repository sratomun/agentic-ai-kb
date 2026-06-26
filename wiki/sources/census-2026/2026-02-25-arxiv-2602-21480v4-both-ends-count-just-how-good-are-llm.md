---
type: source
source_type: arxiv
title: "Both Ends Count! Just How Good are LLM Agents at 'Text-to-Big SQL'?"
authors: Germán T. Eizaguirre, Lars Tissen, Marc Sánchez-Artigas
url: https://arxiv.org/abs/2602.21480v4
date: 2026-02-25
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.DB
tags: [data-query-agents, agent-evaluation, arxiv, auto-ingested]
---

# Both Ends Count! Just How Good are LLM Agents at "Text-to-Big SQL"?

**arXiv:** [2602.21480v4](https://arxiv.org/abs/2602.21480v4) · 2026-02-25 · cs.DB
**Authors:** Germán T. Eizaguirre, Lars Tissen, Marc Sánchez-Artigas

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Text-to-SQL and Big Data are both extensively benchmarked fields, yet there is limited research that evaluates them jointly. In the real world, Text-to-SQL systems are often embedded with Big Data workflows, such as large-scale data processing or interactive data analytics. We refer to this as ``Text-to-Big SQL''. However, existing text-to-SQL benchmarks remain narrowly scoped and overlook the cost and performance implications that arise at scale. For instance, translation errors that are minor on small datasets lead to substantial cost and latency overheads as data scales, a relevant issue completely ignored by text-to-SQL metrics. In this paper, we overcome this overlooked challenge by introducing novel and representative metrics for evaluating Text-to-Big SQL. Our study focuses on production-level LLM agents, a database-agnostic system adaptable to diverse user needs. Via an extensive evaluation of frontier models, we show that text-to-SQL metrics are insufficient for Big Data. In contrast, our proposed text-to-Big SQL metrics accurately reflect execution efficiency, cost, and the impact of data scale. For example, GPT-4o compensates for roughly 7% lower accuracy than the top-performing later-generation models with up to a 12.16x speedup, while GPT-5.2 is more than twice as cost-effective as Gemini 3 Pro at large input scales.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]] · [[gemini]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.21480v4)
