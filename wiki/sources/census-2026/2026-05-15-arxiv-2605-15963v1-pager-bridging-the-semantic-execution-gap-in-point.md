---
type: source
source_type: arxiv
title: "PAGER: Bridging the Semantic-Execution Gap in Point-Precise Geometric GUI Control"
authors: Jingxuan Wei, Xi Bai, Shan Liu, Caijun Jia et al.
url: https://arxiv.org/abs/2605.15963v1
date: 2026-05-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.AI
tags: [computer-use-agents, knowledge-graph, agent-reliability, agentic-rl, multi-agent-systems, arxiv, auto-ingested]
---

# PAGER: Bridging the Semantic-Execution Gap in Point-Precise Geometric GUI Control

**arXiv:** [2605.15963v1](https://arxiv.org/abs/2605.15963v1) · 2026-05-15 · cs.AI
**Authors:** Jingxuan Wei, Xi Bai, Shan Liu, Caijun Jia et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large vision-language models have significantly advanced GUI agents, enabling executable interaction across web, mobile, and desktop interfaces. Yet these gains largely rely on a forgiving region-tolerant paradigm, where many nearby pixels inside the same component remain valid. Precise geometric construction breaks this assumption: actions must land on points in continuous canvas space rather than tolerant regions. Because geometric primitives carry ontological dependencies, a local coordinate error can induce cascading topological failures that distort downstream objects and invalidate the final construction. We identify this regime as precision-sensitive GUI tasks, requiring point-level accuracy, geometry-aware verification, and robustness to dependency-driven error propagation. To benchmark it, we introduce PAGE Bench, with 4,906 problems and over 224K process-supervised, pixel-level GUI actions. We further propose PAGER, a topology-aware agent that decomposes construction into dependency-structured planning and pixel-level execution. Pixel-grounded supervised tuning establishes executable action grammar, while precision-aligned reinforcement learning mitigates rollout-induced exposure bias through state-conditioned geometric feedback. Experiments reveal a pronounced Semantic-Execution Gap: general multimodal models can exceed 88% action type accuracy yet remain below 6% task success. PAGER closes this gap, delivering 4.1x higher task success than the strongest evaluated general baseline and raising step success rate from below 9% for GUI-specialized agents to over 62%, establishing a new state of the art for point-precise GUI control.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.15963v1)
