---
type: source
source_type: arxiv
title: "Adaptive Orchestration: Scalable Self-Evolving Multi-Agent Systems"
authors: Sathish Sampath, Anuradha Baskaran
url: https://arxiv.org/abs/2601.09742v1
date: 2026-01-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.MA
tags: [self-evolving-agents, multi-agent-systems, arxiv, auto-ingested]
---

# Adaptive Orchestration: Scalable Self-Evolving Multi-Agent Systems

**arXiv:** [2601.09742v1](https://arxiv.org/abs/2601.09742v1) · 2026-01-10 · cs.MA
**Authors:** Sathish Sampath, Anuradha Baskaran

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As Large Language Models (LLMs) are increasingly deployed as autonomous agents, they face a critical scalability bottleneck known as the "Generalization-Specialization Dilemma." Monolithic agents equipped with extensive toolkits suffer from context pollution and attention decay, leading to hallucinations. Conversely, static multi-agent swarms introduce significant latency and resource overhead. This paper introduces a Self-Evolving Concierge System, a novel architecture utilizing a Dynamic Mixture of Experts (DMoE) approach. Unlike recent self-improving agents that rewrite their own codebase, our system preserves stability by dynamically restructuring its runtime environment: "hiring" specialized sub-agents based on real-time conversation analysis. We introduce an asynchronous "Meta-Cognition Engine" that detects capability gaps, a Least Recently Used (LRU) eviction policy for resource constraints, and a novel "Surgical History Pruning" mechanism to mitigate refusal bias. Experimental results demonstrate that this architecture maintains high task success rates while minimizing token consumption compared to static agent swarms.

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.09742v1)
