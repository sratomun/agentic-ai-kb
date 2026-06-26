---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Polaris: A Gödel Agent Framework for Small Language Models through Experience-Abstracted Policy Repair"
authors: Aditya Kakade et al.
url: https://arxiv.org/abs/2603.23129v2
date: 2026-03-24
score: 8
primary: cs.LG
tags: [arxiv, auto-ingested, small-language-models, llm-as-judge, distillation, reasoning-models]
---

# Polaris: A Gödel Agent Framework for Small Language Models through Experience-Abstracted Policy Repair

**arXiv:** [2603.23129v2](https://arxiv.org/abs/2603.23129v2) · 2026-03-24 · cs.LG
**Authors:** Aditya Kakade et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Gödel agent realize recursive self-improvement: an agent inspects its own policy and traces and then modifies that policy in a tested loop. We introduce Polaris, a Gödel agent for compact models that performs policy repair via experience abstraction, turning failures into policy updates through a structured cycle of analysis, strategy formation, abstraction, and minimal code pat ch repair with conservative checks. Unlike response level self correction or parameter tuning, Polaris makes policy level changes with small, auditable patches that persist in the policy and are reused on unseen instances within each benchmark. As part of the loop, the agent engages in meta reasoning: it explains its errors, proposes concrete revisions to its own policy, and then updates the policy. To enable cumulative policy refinement, we introduce experience abstraction, which distills failures into compact, reusable strategies that transfer to unseen instances. On MGSM, DROP, GPQA, and LitBench (covering arithmetic reasoning, compositional inference, graduate-level problem solving, and creative writing evaluation), a 7-billion-parameter model equipped with Polaris achieves consistent gains over the base policy and competitive baselines.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[llm-as-judge]] · [[distillation]] · [[reasoning-models]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.23129v2)
