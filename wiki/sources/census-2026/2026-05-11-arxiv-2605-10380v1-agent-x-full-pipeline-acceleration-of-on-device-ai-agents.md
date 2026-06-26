---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Agent-X: Full Pipeline Acceleration of On-device AI Agents"
authors: Jinha Chung et al.
url: https://arxiv.org/abs/2605.10380v1
date: 2026-05-11
score: 7
primary: cs.AI
tags: [arxiv, auto-ingested, small-language-models, coding-agents]
---

# Agent-X: Full Pipeline Acceleration of On-device AI Agents

**arXiv:** [2605.10380v1](https://arxiv.org/abs/2605.10380v1) · 2026-05-11 · cs.AI
**Authors:** Jinha Chung et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM-based agents deliver state-of-the-art performance across tasks but incur high end-to-end latency on edge devices. We introduce Agent-X, a software-only, accuracy-preserving framework that accelerates both the prefill and decode stages of on-device agent workloads. Agent-X's two key components rewrite prompts to leverage prefix caching tailored to agent-specific input-token patterns and enable LLM-free speculative decoding for fast token generation with minimal overhead. On representative agentic workloads, Agent-X achieves a 1.61x end-to-end speedup in real systems with no accuracy loss and can be seamlessly integrated into existing on-device AI agents. To the best of our knowledge, ours is the first to systematically characterize and eliminate latency bottlenecks in on-device agents.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[coding-agents]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.10380v1)
