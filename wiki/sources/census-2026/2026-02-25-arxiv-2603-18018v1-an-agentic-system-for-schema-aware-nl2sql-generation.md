---
type: source
source_type: arxiv
title: "An Agentic System for Schema Aware NL2SQL Generation"
authors: David Onyango, Naseef Mansoor
url: https://arxiv.org/abs/2603.18018v1
date: 2026-02-25
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.CL
tags: [data-query-agents, coding-agents, agent-evaluation, arxiv, auto-ingested]
---

# An Agentic System for Schema Aware NL2SQL Generation

**arXiv:** [2603.18018v1](https://arxiv.org/abs/2603.18018v1) · 2026-02-25 · cs.CL
**Authors:** David Onyango, Naseef Mansoor

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The natural language to SQL (NL2SQL) task plays a pivotal role in democratizing data access by enabling non-expert users to interact with relational databases through intuitive language. While recent frameworks have enhanced translation accuracy via task specialization, their reliance on Large Language Models (LLMs) raises significant concerns regarding computational overhead, data privacy, and real-world deployability in resource-constrained environments. To address these challenges, we propose a schema based agentic system that strategically employs Small Language Models (SLMs) as primary agents, complemented by a selective LLM fallback mechanism. The LLM is invoked only upon detection of errors in SLM-generated output, the proposed system significantly minimizes computational expenditure. Experimental results on the BIRD benchmark demonstrate that our system achieves an execution accuracy of 47.78% and a validation efficiency score of 51.05%, achieving over 90% cost reduction compared to LLM-centric baselines as approximately 67% of queries are resolved using local SLMs. The system achieves an average cost per query of 0.0085 compared to 0.094 for LLM-only systems, achieving near-zero operational costs for locally executed queries. [Github repository: https://github.com/mindslab25/CESMA.]

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[coding-agents|Coding agents]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[bird-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.18018v1)
