---
type: source
source_type: arxiv
title: "Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic Multimodal Models"
authors: Shilin Yan, Jintao Tong, Hongwei Xue, Xiaojun Tang et al.
url: https://arxiv.org/abs/2604.08545v1
date: 2026-04-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.CV
tags: [agentic-rl, tool-use, arxiv, auto-ingested]
---

# Act Wisely: Cultivating Meta-Cognitive Tool Use in Agentic Multimodal Models

**arXiv:** [2604.08545v1](https://arxiv.org/abs/2604.08545v1) · 2026-04-09 · cs.CV
**Authors:** Shilin Yan, Jintao Tong, Hongwei Xue, Xiaojun Tang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The advent of agentic multimodal models has empowered systems to actively interact with external environments. However, current agents suffer from a profound meta-cognitive deficit: they struggle to arbitrate between leveraging internal knowledge and querying external utilities. Consequently, they frequently fall prey to blind tool invocation, resorting to reflexive tool execution even when queries are resolvable from the raw visual context. This pathological behavior precipitates severe latency bottlenecks and injects extraneous noise that derails sound reasoning. Existing reinforcement learning protocols attempt to mitigate this via a scalarized reward that penalizes tool usage. Yet, this coupled formulation creates an irreconcilable optimization dilemma: an aggressive penalty suppresses essential tool use, whereas a mild penalty is entirely subsumed by the variance of the accuracy reward during advantage normalization, rendering it impotent against tool overuse. To transcend this bottleneck, we propose HDPO, a framework that reframes tool efficiency from a competing scalar objective to a strictly conditional one. By eschewing reward scalarization, HDPO maintains two orthogonal optimization channels: an accuracy channel that maximizes task correctness, and an efficiency channel that enforces execution economy exclusively within accurate trajectories via conditional advantage estimation. This decoupled architecture naturally induces a cognitive curriculum-compelling the agent to first master task resolution before refining its self-reliance. Extensive evaluations demonstrate that our resulting model, Metis, reduces tool invocations by orders of magnitude while simultaneously elevating reasoning accuracy.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.08545v1)
