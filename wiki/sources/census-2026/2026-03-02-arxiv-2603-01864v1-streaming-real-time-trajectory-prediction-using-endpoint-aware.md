---
type: source
source_type: arxiv
title: "Streaming Real-Time Trajectory Prediction Using Endpoint-Aware Modeling"
authors: Alexander Prutsch, David Schinagl, Horst Possegger
url: https://arxiv.org/abs/2603.01864v1
date: 2026-03-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 10
primary: cs.CV
tags: [autonomous-driving-agents, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Streaming Real-Time Trajectory Prediction Using Endpoint-Aware Modeling

**arXiv:** [2603.01864v1](https://arxiv.org/abs/2603.01864v1) · 2026-03-02 · cs.CV
**Authors:** Alexander Prutsch, David Schinagl, Horst Possegger

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Future trajectories of neighboring traffic agents have a significant influence on the path planning and decision-making of autonomous vehicles. While trajectory forecasting is a well-studied field, research mainly focuses on snapshot-based prediction, where each scenario is treated independently of its global temporal context. However, real-world autonomous driving systems need to operate in a continuous setting, requiring real-time processing of data streams with low latency and consistent predictions over successive timesteps. We leverage this continuous setting to propose a lightweight yet highly accurate streaming-based trajectory forecasting approach. We integrate valuable information from previous predictions with a novel endpoint-aware modeling scheme. Our temporal context propagation uses the trajectory endpoints of the previous forecasts as anchors to extract targeted scenario context encodings. Our approach efficiently guides its scene encoder to extract highly relevant context information without needing refinement iterations or segment-wise decoding. Our experiments highlight that our approach effectively relays information across consecutive timesteps. Unlike methods using multi-stage refinement processing, our approach significantly reduces inference latency, making it well-suited for real-world deployment. We achieve state-of-the-art streaming trajectory prediction results on the Argoverse~2 multi-agent and single-agent benchmarks, while requiring substantially fewer resources.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.01864v1)
