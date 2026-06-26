---
type: source
source_type: arxiv
title: "CreativityBench: Evaluating Agent Creative Reasoning via Affordance-Based Tool Repurposing"
authors: Cheng Qian, Hyeonjeong Ha, Jiayu Liu, Jeonghwan Kim et al.
url: https://arxiv.org/abs/2605.02910v2
date: 2026-04-06
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-reliability, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# CreativityBench: Evaluating Agent Creative Reasoning via Affordance-Based Tool Repurposing

**arXiv:** [2605.02910v2](https://arxiv.org/abs/2605.02910v2) · 2026-04-06 · cs.AI
**Authors:** Cheng Qian, Hyeonjeong Ha, Jiayu Liu, Jeonghwan Kim et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in large language models have led to strong performance on reasoning and environment-interaction tasks, yet their ability for creative problem-solving remains underexplored. We study this capability through the lens of creative tool use, where a model repurposes available objects by reasoning about their affordances and attributes rather than relying on canonical usage. As a first step, we introduce CreativityBench, a benchmark for evaluating affordance-based creativity in LLMs. To this end, we build a large-scale affordance knowledge base (KB) with 4K entities and 150K+ affordance annotations, explicitly linking objects, parts, attributes, and actionable uses. Building on this KB, we generate 14K grounded tasks that require identifying non-obvious yet physically plausible solutions under constraints. Evaluations across 10 state-of-the-art LLMs, including closed and open-source models, show that models can often select a plausible object, but fail to identify the correct parts, their affordances, and the underlying physical mechanism needed to solve the task, leading to a significant drop in performance. Furthermore, improvements from model scaling quickly saturate, strong general reasoning does not reliably translate to creative affordance discovery, and common inference-time strategies such as Chain-of-Thought yield limited gains. These results suggest that creative tool use remains a major challenge for current models, and that CreativityBench provides a useful testbed for studying this missing dimension of intelligence, with potential implications for planning and reasoning modules in future agents.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.02910v2)
