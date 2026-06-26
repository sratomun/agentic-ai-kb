---
type: source
source_type: arxiv
title: "Reason-to-Transmit: Deliberative Adaptive Communication for Cooperative Perception"
authors: Aayam Bansal, Ishaan Gangwani
url: https://arxiv.org/abs/2603.20308v1
date: 2026-03-19
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.MA
tags: [agent-reliability, multi-agent-systems, arxiv, auto-ingested]
---

# Reason-to-Transmit: Deliberative Adaptive Communication for Cooperative Perception

**arXiv:** [2603.20308v1](https://arxiv.org/abs/2603.20308v1) · 2026-03-19 · cs.MA
**Authors:** Aayam Bansal, Ishaan Gangwani

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Cooperative perception among autonomous agents overcomes the limitations of single-agent sensing, but bandwidth constraints in vehicle-to-everything (V2X) networks require efficient communication policies. Existing approaches rely on reactive mechanisms, such as confidence maps, learned gating, or sparse masks, to decide what to transmit, without reasoning about why a message benefits the receiver. We introduce Reason-to-Transmit (R2T), a framework that equips each agent with a lightweight transformer-based module that reasons over local scene context, estimated neighbor information gaps, and bandwidth budget to make per-region transmission decisions. Trained end-to-end with a bandwidth-aware objective, R2T is evaluated against nine baselines in a multi-agent bird's-eye-view perception environment. Any communication improves performance by about 58% AP over no communication. At low bandwidth, all selective methods perform similarly, but R2T shows clear gains under high occlusion, where information asymmetry is greatest, approaching oracle performance. All methods degrade gracefully under packet drops up to 50%, showing robustness to communication failures. These results indicate that while fusion design dominates performance, deliberative communication provides additional gains in challenging scenarios. R2T introduces a reasoning-based approach to communication, enabling more efficient and context-aware information sharing in cooperative perception.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[bird-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.20308v1)
