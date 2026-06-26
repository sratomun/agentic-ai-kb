---
type: source
source_type: arxiv
title: "Can Agents Price a Reaction? Evaluating LLMs on Chemical Cost Reasoning"
authors: Yuyang Wu, Yue Huang, Shuaike Shen, Xujian Wang et al.
url: https://arxiv.org/abs/2605.07251v1
date: 2026-05-08
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [clinical-agents, science-agents, agent-reliability, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Can Agents Price a Reaction? Evaluating LLMs on Chemical Cost Reasoning

**arXiv:** [2605.07251v1](https://arxiv.org/abs/2605.07251v1) · 2026-05-08 · cs.AI
**Authors:** Yuyang Wu, Yue Huang, Shuaike Shen, Xujian Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) have become increasingly capable as tool-using agents, with benchmarks spanning diverse general agentic tasks. Yet rigorous evaluation of scientific tool use remains limited. In chemistry, recent agents can plan syntheses and invoke domain-specific tools, but evaluations often rely on curated demonstrations, expert assessment, or LLM-as-judge scoring rather than exact, judge-free ground truth. We address this gap with chemical procurement cost estimation, a practical task in which an agent must ground chemical identities, retrieve supplier quotes, select valid purchasable packs, normalize quantities, and compute cost from a reaction description. We introduce ChemCost, a benchmark of 1,427 evaluable reactions grounded to a frozen pricing snapshot covering 2,261 chemicals and 230,775 supplier quotes, supporting scalar scoring and stage-level diagnosis of grounding, retrieval, procurement, and arithmetic failures. To evaluate robustness, we further construct controlled noise-injected views that perturb chemical aliases, quantity expressions, missing fields, and input formatting. Experiments with frontier, open-weight, and chemistry-specialized LLM agents show that tool access is necessary but insufficient for solving the task. The strongest agents reach only 50.6% accuracy within 25% relative error on clean inputs and degrade substantially with realistic noise. Stage-level analysis further shows that failures arise from brittle parsing, ineffective evidence integration, invalid pack selection, and non-convergent tool use.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[science-agents|Science agents]] · [[agent-reliability|Agent reliability]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.07251v1)
