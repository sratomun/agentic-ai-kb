---
type: source
source_type: arxiv
title: "D-MEM: Dopamine-Gated Agentic Memory via Reward Prediction Error Routing"
authors: Yuru Song, Qi Xin
url: https://arxiv.org/abs/2603.14597v1
date: 2026-03-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 13
primary: q-bio.NC
tags: [knowledge-graph, agentic-rl, agent-security, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# D-MEM: Dopamine-Gated Agentic Memory via Reward Prediction Error Routing

**arXiv:** [2603.14597v1](https://arxiv.org/abs/2603.14597v1) · 2026-03-15 · q-bio.NC
**Authors:** Yuru Song, Qi Xin

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Autonomous LLM agents require structured long-term memory, yet current "append-and-evolve" systems like A-MEM face O(N^2) write-latency and excessive token costs. We introduce D-MEM (Dopamine-Gated Agentic Memory), a biologically inspired architecture that decouples short-term interaction from cognitive restructuring via a Fast/Slow routing system based on Reward Prediction Error (RPE). A lightweight Critic Router evaluates stimuli for Surprise and Utility. Routine, low-RPE inputs are bypassed or cached in an O(1) fast-access buffer. Conversely, high-RPE inputs, such as factual contradictions or preference shifts, trigger a "dopamine" signal, activating the O(N) memory evolution pipeline to reshape the agent's knowledge graph. To evaluate performance under realistic conditions, we introduce the LoCoMo-Noise benchmark, which injects controlled conversational noise into long-term sessions. Evaluations demonstrate that D-MEM reduces token consumption by over 80%, eliminates O(N^2) bottlenecks, and outperforms baselines in multi-hop reasoning and adversarial resilience. By selectively gating cognitive restructuring, D-MEM provides a scalable, cost-efficient foundation for lifelong agentic memory.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.14597v1)
