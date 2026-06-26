---
type: source
source_type: arxiv
title: "LongVidSearch: An Agentic Benchmark for Multi-hop Evidence Retrieval Planning in Long Videos"
authors: Rongyi Yu, Chenyuan Duan, Wentao Zhang
url: https://arxiv.org/abs/2603.14468v1
date: 2026-03-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.CV
tags: [tool-use, agent-evaluation, arxiv, auto-ingested]
---

# LongVidSearch: An Agentic Benchmark for Multi-hop Evidence Retrieval Planning in Long Videos

**arXiv:** [2603.14468v1](https://arxiv.org/abs/2603.14468v1) · 2026-03-15 · cs.CV
**Authors:** Rongyi Yu, Chenyuan Duan, Wentao Zhang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Long video question answering (Long-Video QA) increasingly relies on agentic tool use to retrieve evidence from long videos. In realistic settings, this process often requires multi-hop retrieval, where agents must iteratively gather multiple discontinuous evidence clips. However, existing long-video benchmarks are largely static: they rarely enforce strict multi-hop retrieval and typically lack a standardized evidence-access interface, making it difficult to separate failures in retrieval planning from those in answer generation. To address this gap, we introduce LongVidSearch, a benchmark for evaluating agentic multi-hop evidence retrieval planning in long videos under standardized access constraints. LongVidSearch enforces retrieval necessity: a Hop-k question requires exactly k necessary evidence clips, and removing any single clip renders the question unsolvable. The benchmark contains 3,000 questions over 447 long videos (average length 26 minutes), covering four reasoning categories: State Mutation, Causal Inference, Global Summary, and Visual Tracking, with 2-hop, 3-hop, and 4-hop evidence requirements. To ensure fair and controlled evaluation, all agents interact with LongVidSearch through a unified tool interface, which fixes the retrieval backend and isolates the agent's ability to formulate queries and plan iterative retrieval. In addition to answer accuracy, we measure tool-call cost to analyze the accuracy-efficiency trade-off under identical access conditions. We evaluate VideoAgent-style QA agents with multiple backbone LLMs using three-judge majority voting. GPT-5 achieves the highest accuracy (42.43), outperforming Gemini 3 Pro (30.97) and GPT-4o (19.20), yet remaining below 50 %, highlighting the difficulty of multi-hop retrieval planning. With gold evidence clips, performance becomes near-perfect, confirming retrieval planning as the primary bottleneck.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]] · [[gemini]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.14468v1)
