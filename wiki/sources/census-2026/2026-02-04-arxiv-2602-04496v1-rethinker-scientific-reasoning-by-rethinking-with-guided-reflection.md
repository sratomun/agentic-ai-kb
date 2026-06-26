---
type: source
source_type: arxiv
title: "ReThinker: Scientific Reasoning by Rethinking with Guided Reflection and Confidence Control"
authors: Zhentao Tang, Yuqi Cui, Shixiong Kai, Wenqian Zhao et al.
url: https://arxiv.org/abs/2602.04496v1
date: 2026-02-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# ReThinker: Scientific Reasoning by Rethinking with Guided Reflection and Confidence Control

**arXiv:** [2602.04496v1](https://arxiv.org/abs/2602.04496v1) · 2026-02-04 · cs.AI
**Authors:** Zhentao Tang, Yuqi Cui, Shixiong Kai, Wenqian Zhao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Expert-level scientific reasoning remains challenging for large language models, particularly on benchmarks such as Humanity's Last Exam (HLE), where rigid tool pipelines, brittle multi-agent coordination, and inefficient test-time scaling often limit performance. We introduce ReThinker, a confidence-aware agentic framework that orchestrates retrieval, tool use, and multi-agent reasoning through a stage-wise Solver-Critic-Selector architecture. Rather than following a fixed pipeline, ReThinker dynamically allocates computation based on model confidence, enabling adaptive tool invocation, guided multi-dimensional reflection, and robust confidence-weighted selection. To support scalable training without human annotation, we further propose a reverse data synthesis pipeline and an adaptive trajectory recycling strategy that transform successful reasoning traces into high-quality supervision. Experiments on HLE, GAIA, and XBench demonstrate that ReThinker consistently outperforms state-of-the-art foundation models with tools and existing deep research systems, achieving state-of-the-art results on expert-level reasoning tasks.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gaia-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.04496v1)
