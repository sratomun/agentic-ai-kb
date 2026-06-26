---
type: source
source_type: arxiv
title: "Engineering Reasoning and Instruction (ERI) Benchmark: A Large Taxonomy-driven Dataset for Foundation Models and Agents"
authors: MZ Naser, Ahmad Bani Awwad, Zoie McCreery, Radwa Eissa et al.
url: https://arxiv.org/abs/2603.02239v1
date: 2026-02-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-protocols, agentic-rag, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Engineering Reasoning and Instruction (ERI) Benchmark: A Large Taxonomy-driven Dataset for Foundation Models and Agents

**arXiv:** [2603.02239v1](https://arxiv.org/abs/2603.02239v1) · 2026-02-16 · cs.AI
**Authors:** MZ Naser, Ahmad Bani Awwad, Zoie McCreery, Radwa Eissa et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The Engineering Reasoning and Instruction (ERI) benchmark is a taxonomy-driven instruction dataset designed to train and evaluate engineering-capable large language models (LLMs) and agents. This dataset spans nine engineering fields (namely: civil, mechanical, electrical, chemical, environmental, aerospace, materials, fire, and industrial engineering) and 55 subdomains, and is crossed with seven intent types (i.e., definition, explanation, calculation, comparison, design/synthesis, troubleshooting, and code-related) and three difficulty tiers (undergraduate, graduate, and professional), yielding 57,750 records with field/subdomain/type/difficulty metadata and solution formatting. We examined ERI via seven LLMs and report a statistically significant three-tier performance structure, with frontier models (GPT-5, Claude Sonnet 4, DeepSeek V3.1) achieving mean scores above 4.30 on a five-point scale, while mid-tier and smaller models exhibited progressively higher failure rates and steeper performance degradation on graduate-level questions. To address circularity concerns inherent in LLM benchmarks, we developed a convergent validation protocol that leverages cross-provider independence, multi-judge averaging, and frontier-model agreement analysis to empirically bound hallucination risk to 1.7%. ERI is released with taxonomy specifications, validation scripts, and an evaluation harness to enable reproducible comparisons and regression testing for instruction tuning, routing, retrieval-augmented evaluation, and agentic tool-use workflows in engineering settings.

## Graph
- **Concepts:** [[agent-protocols|Agent protocols]] · [[agentic-rag|Agentic RAG]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[claude]] · [[gpt-5]] · [[deepseek]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.02239v1)
