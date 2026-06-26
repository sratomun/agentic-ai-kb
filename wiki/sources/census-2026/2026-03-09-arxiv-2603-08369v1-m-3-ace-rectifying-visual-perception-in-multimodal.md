---
type: source
source_type: arxiv
title: "M$^3$-ACE: Rectifying Visual Perception in Multimodal Math Reasoning via Multi-Agentic Context Engineering"
authors: Peijin Xie, Zhen Xu, Bingquan Liu, Baoxun Wang
url: https://arxiv.org/abs/2603.08369v1
date: 2026-03-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-reliability, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# M$^3$-ACE: Rectifying Visual Perception in Multimodal Math Reasoning via Multi-Agentic Context Engineering

**arXiv:** [2603.08369v1](https://arxiv.org/abs/2603.08369v1) · 2026-03-09 · cs.AI
**Authors:** Peijin Xie, Zhen Xu, Bingquan Liu, Baoxun Wang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multimodal large language models have recently shown promising progress in visual mathematical reasoning. However, their performance is often limited by a critical yet underexplored bottleneck: inaccurate visual perception. Through systematic analysis, we find that the most failures originate from incorrect or incomplete visual evidence extraction rather than deficiencies in reasoning capability. Moreover, models tend to remain overly confident in their initial perceptions, making standard strategies such as prompt engineering, multi-round self-reflection, or posterior guidance insufficient to reliably correct errors. To address this limitation, we propose M3-ACE, a multi-agentic context engineering framework designed to rectify visual perception in multimodal math reasoning. Instead of directly aggregating final answers, our approach decouples perception and reasoning by dynamically maintaining a shared context centered on visual evidence lists. Multiple agents collaboratively contribute complementary observations, enabling the system to expose inconsistencies and recover missing perceptual information. To support stable multi-turn collaboration, we further introduce two lightweight tools: a Summary Tool that organizes evidence from different agents into consistent, complementary, and conflicting components, and a Refine Tool that filters unreliable samples and guides iterative correction. Extensive experiments demonstrate that M3-ACE substantially improves visual mathematical reasoning performance across multiple benchmarks. Our method establishes new state-of-the-art results 89.1 on the MathVision benchmark and achieves consistent improvements on other related datasets, including MathVista and MathVerse. These results highlight the importance of perception-centric multi-agent collaboration for advancing multimodal reasoning systems.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.08369v1)
