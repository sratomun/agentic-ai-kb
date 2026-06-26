---
type: source
source_type: arxiv
title: "Self-Compression of Chain-of-Thought via Multi-Agent Reinforcement Learning"
authors: Yiqun Chen, Jinyuan Feng, Wei Yang, Meizhi Zhong et al.
url: https://arxiv.org/abs/2601.21919v1
date: 2026-01-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.AI
tags: [agentic-rl, multi-agent-systems, arxiv, auto-ingested]
---

# Self-Compression of Chain-of-Thought via Multi-Agent Reinforcement Learning

**arXiv:** [2601.21919v1](https://arxiv.org/abs/2601.21919v1) · 2026-01-29 · cs.AI
**Authors:** Yiqun Chen, Jinyuan Feng, Wei Yang, Meizhi Zhong et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The inference overhead induced by redundant reasoning undermines the interactive experience and severely bottlenecks the deployment of Large Reasoning Models. Existing reinforcement learning (RL)-based solutions tackle this problem by coupling a length penalty with outcome-based rewards. This simplistic reward weighting struggles to reconcile brevity with accuracy, as enforcing brevity may compromise critical reasoning logic. In this work, we address this limitation by proposing a multi-agent RL framework that selectively penalizes redundant chunks, while preserving essential reasoning logic. Our framework, Self-Compression via MARL (SCMA), instantiates redundancy detection and evaluation through two specialized agents: \textbf{a Segmentation Agent} for decomposing the reasoning process into logical chunks, and \textbf{a Scoring Agent} for quantifying the significance of each chunk. The Segmentation and Scoring agents collaboratively define an importance-weighted length penalty during training, incentivizing \textbf{a Reasoning Agent} to prioritize essential logic without introducing inference overhead during deployment. Empirical evaluations across model scales demonstrate that SCMA reduces response length by 11.1\% to 39.0\% while boosting accuracy by 4.33\% to 10.02\%. Furthermore, ablation studies and qualitative analysis validate that the synergistic optimization within the MARL framework fosters emergent behaviors, yielding more powerful LRMs compared to vanilla RL paradigms.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.21919v1)
