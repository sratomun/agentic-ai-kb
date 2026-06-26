---
type: source
source_type: arxiv
title: "Large-Scale Optimization Model Auto-Formulation: Harnessing LLM Flexibility via Structured Workflow"
authors: Kuo Liang, Yuhang Lu, Jianming Mao, Shuyi Sun et al.
url: https://arxiv.org/abs/2601.09635v3
date: 2026-01-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Large-Scale Optimization Model Auto-Formulation: Harnessing LLM Flexibility via Structured Workflow

**arXiv:** [2601.09635v3](https://arxiv.org/abs/2601.09635v3) · 2026-01-14 · cs.AI
**Authors:** Kuo Liang, Yuhang Lu, Jianming Mao, Shuyi Sun et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large-scale optimization is a key backbone of modern business decision-making. However, building these models is often labor-intensive and time-consuming. We address this by proposing LEAN-LLM-OPT, a LightwEight AgeNtic workflow construction framework for LLM-assisted large-scale OPTimization auto-formulation. LEAN-LLM-OPT takes as input a problem description together with associated datasets and orchestrates a team of LLM agents to produce an optimization formulation. Specifically, upon receiving a query, two upstream LLM agents dynamically construct a workflow that specifies, step-by-step, how optimization models for similar problems can be formulated. A downstream LLM agent then follows this workflow to generate the final output. The agentic workflow leverages common modeling practices to structure the modeling process into a sequence of sub-tasks, offloading mechanical data-handling operations to auxiliary tools. This reduces the LLM's burden in planning and data handling, allowing us to exploit its flexibility to address unstructured components. Extensive simulations show that LEAN-LLM-OPT, instantiated with GPT-4.1 and the open source gpt-oss-20B, achieves strong performance on large-scale optimization modeling tasks and is competitive with state-of-the-art approaches. In addition, in a Singapore Airlines choice-based revenue management use case, LEAN-LLM-OPT demonstrates practical value by achieving leading performance across a range of scenarios. Along the way, we introduce Large-Scale-OR and Air-NRM, the first comprehensive benchmarks for large-scale optimization auto-formulation. The code and data of this work is available at https://github.com/CoraLiang01/lean-llm-opt.

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.09635v3)
