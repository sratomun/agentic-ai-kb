---
type: source
source_type: arxiv
title: "RUBICON: Agentic AI for Messy Enterprise Data"
authors: Fabian Wenz, Felix Treutwein, Kai Arenja, Çagatay Demiralp et al.
url: https://arxiv.org/abs/2604.21413v2
date: 2026-04-23
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.DB
tags: [data-query-agents, agent-reliability, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# RUBICON: Agentic AI for Messy Enterprise Data

**arXiv:** [2604.21413v2](https://arxiv.org/abs/2604.21413v2) · 2026-04-23 · cs.DB
**Authors:** Fabian Wenz, Felix Treutwein, Kai Arenja, Çagatay Demiralp et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Enterprise data exists in many forms, such as tables, text, maps, e-mail, and CAD models, that are access-controlled and hidden behind bespoke interfaces. Current agentic AI systems delegate the entire query workflow to a frontier LLM: a single model interprets the request, selects sources or tools, integrates retrieved evidence, judges completeness, and generates an answer, with few constraints, limited use of schemas, and text as the primary representation throughout. We argue that this is an ineffective abstraction for enterprise data. Reliable agentic AI should instead require structure: a constrained query interface over each source and a table-centric integration layer driven by a query processor. We introduce RUBICON, a system that embodies this vision. RUBICON is based on two observations. First, text-to-SQL fails on real enterprise data and must be dramatically subsetted to achieve reliable results. Second, data integration across disparate corporate datasets is best performed using tables as the core abstraction rather than text-centric LLM pipelines. We evaluate RUBICON on two benchmarks: our enterprise-focused RUBICON-Bench, against agentic baselines, and SemBench, against LOTUS and Palimpzest. On RUBICON-Bench, where queries require coordination across heterogeneous enterprise sources, RUBICON achieves 100% end-to-end accuracy, while all agentic baselines, including single- and multi-agent ReAct systems, produce no correct answers. On SemBench, RUBICON surpasses both LOTUS and Palimpzest: it achieves 14.7% higher accuracy, reduces latency by 62.64%, and lowers token cost by 98.64%, demonstrating that a table-centric architecture better matches enterprise data while yielding significant efficiency gains.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.21413v2)
