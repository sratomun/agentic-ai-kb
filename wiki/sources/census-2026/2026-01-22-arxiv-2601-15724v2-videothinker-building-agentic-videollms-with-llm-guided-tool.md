---
type: source
source_type: arxiv
title: "VideoThinker: Building Agentic VideoLLMs with LLM-Guided Tool Reasoning"
authors: Chenglin Li, Qianglong Chen, Feng Han, Yikun Wang et al.
url: https://arxiv.org/abs/2601.15724v2
date: 2026-01-22
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CV
tags: [tool-use, agent-evaluation, arxiv, auto-ingested]
---

# VideoThinker: Building Agentic VideoLLMs with LLM-Guided Tool Reasoning

**arXiv:** [2601.15724v2](https://arxiv.org/abs/2601.15724v2) · 2026-01-22 · cs.CV
**Authors:** Chenglin Li, Qianglong Chen, Feng Han, Yikun Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Long-form video understanding remains a fundamental challenge for current Video Large Language Models. Most existing models rely on static reasoning over uniformly sampled frames, which weakens temporal localization and leads to substantial information loss in long videos. Agentic tools such as temporal retrieval, spatial zoom, and temporal zoom offer a natural way to overcome these limitations by enabling adaptive exploration of key moments. However, constructing agentic video understanding data requires models that already possess strong long-form video comprehension, creating a circular dependency. We address this challenge with VideoThinker, an agentic Video Large Language Model trained entirely on synthetic tool interaction trajectories. Our key idea is to convert videos into rich captions and employ a powerful agentic language model to generate multi-step tool use sequences in caption space. These trajectories are subsequently grounded back to video by replacing captions with the corresponding frames, yielding a large-scale interleaved video and tool reasoning dataset without requiring any long-form understanding from the underlying model. Training on this synthetic agentic dataset equips VideoThinker with dynamic reasoning capabilities, adaptive temporal exploration, and multi-step tool use. Remarkably, VideoThinker significantly outperforms both caption-only language model agents and strong video model baselines across long-video benchmarks, demonstrating the effectiveness of tool augmented synthetic data and adaptive retrieval and zoom reasoning for long-form video understanding.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.15724v2)
