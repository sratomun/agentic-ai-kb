---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Meta-Tool: Efficient Few-Shot Tool Adaptation for Small Language Models"
authors: Sachin Kumar
url: https://arxiv.org/abs/2604.20148v1
date: 2026-04-22
score: 7
primary: cs.CL
tags: [arxiv, auto-ingested, small-language-models, tool-use, llm-as-judge, post-training, coding-agents]
---

# Meta-Tool: Efficient Few-Shot Tool Adaptation for Small Language Models

**arXiv:** [2604.20148v1](https://arxiv.org/abs/2604.20148v1) · 2026-04-22 · cs.CL
**Authors:** Sachin Kumar

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Can small language models achieve strong tool-use performance without complex adaptation mechanisms? This paper investigates this question through Meta-Tool, a controlled empirical study comparing hypernetwork-based LoRA adaptation against carefully designed few-shot prompting. Using a Llama-3.2-3B-Instruct backbone, we evaluate four adaptation mechanisms--few-shot prompting, documentation encoding, hypernetwork-generated LoRA weights, and value-guided beam search--across four diverse benchmarks: Gorilla APIBench, Spider 2.0, WebArena, and InterCode. Our central finding is a well-supported negative result: despite generating non-trivial weight matrices, the 227.8M-parameter hypernetwork provides no measurable improvement over few-shot prompting alone. Comprehensive ablation studies reveal that few-shot examples contribute +21.5% to performance and documentation contributes +5.0%, while the hypernetwork adds 0%. A 3B model with well-designed prompts achieves 79.7% of GPT-5's average performance at $10 \times$ lower latency. Error analysis across 722 failure cases spanning all shot counts (0--5) shows that at the 5-shot configuration (106 failures), failure modes are task-dependent: schema-heavy tasks (Spider 2.0, WebArena) show near-zero format errors with remaining failures semantic, while format errors dominate on Gorilla (100%) and InterCode (70%). These findings redirect practitioners toward prompt engineering and example curation rather than complex adaptation architectures.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[tool-use]] · [[llm-as-judge]] · [[post-training]] · [[coding-agents]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.20148v1)
