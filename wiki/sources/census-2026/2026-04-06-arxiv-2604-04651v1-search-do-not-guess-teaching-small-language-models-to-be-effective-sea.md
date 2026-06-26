---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Search, Do not Guess: Teaching Small Language Models to Be Effective Search Agents"
authors: Yizhou Liu et al.
url: https://arxiv.org/abs/2604.04651v1
date: 2026-04-06
score: 9
primary: cs.AI
tags: [arxiv, auto-ingested, small-language-models, llm-as-judge, distillation, post-training, reasoning-models]
---

# Search, Do not Guess: Teaching Small Language Models to Be Effective Search Agents

**arXiv:** [2604.04651v1](https://arxiv.org/abs/2604.04651v1) · 2026-04-06 · cs.AI
**Authors:** Yizhou Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agents equipped with search tools have emerged as effective solutions for knowledge-intensive tasks. While Large Language Models (LLMs) exhibit strong reasoning capabilities, their high computational cost limits practical deployment for search agents. Consequently, recent work has focused on distilling agentic behaviors from LLMs into Small Language Models (SLMs). Through comprehensive evaluation on complex multi-hop reasoning tasks, we find that despite possessing less parametric knowledge, SLMs invoke search tools less frequently and are more prone to hallucinations. To address this issue, we propose \policy, a lightweight fine-tuning approach that explicitly trains SLMs to reliably retrieve and generate answers grounded in retrieved evidence. Compared to agent distillation from LLMs, our approach improves performance by 17.3 scores on Bamboogle and 15.3 scores on HotpotQA, achieving LLM-level results across benchmarks. Our further analysis reveals that adaptive search strategies in SLMs often degrade performance, highlighting the necessity of consistent search behavior for reliable reasoning.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[llm-as-judge]] · [[distillation]] · [[post-training]] · [[reasoning-models]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.04651v1)
