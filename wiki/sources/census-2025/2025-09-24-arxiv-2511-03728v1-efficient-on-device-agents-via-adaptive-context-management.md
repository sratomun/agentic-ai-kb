---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Efficient On-Device Agents via Adaptive Context Management"
authors: Sanidhya Vijayvargiya et al.
url: https://arxiv.org/abs/2511.03728v1
date: 2025-09-24
score: 3
primary: cs.AI
tags: [arxiv, auto-ingested, small-language-models, tool-use, agent-memory, llm-as-judge, distillation]
---

# Efficient On-Device Agents via Adaptive Context Management

**arXiv:** [2511.03728v1](https://arxiv.org/abs/2511.03728v1) · 2025-09-24 · cs.AI
**Authors:** Sanidhya Vijayvargiya et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
On-device AI agents offer the potential for personalized, low-latency assistance, but their deployment is fundamentally constrained by limited memory capacity, which restricts usable context. This reduced practical context window creates a trade-off between supporting rich, stateful interactions with complex tool capabilities and maintaining on-device feasibility. We break this trade-off with a framework for context-efficient on-device agents, driven by three synergistic optimizations (1) a dynamic memory system using specialized LoRA adapters to distill conversational history into a compressed, and structured Context State Object; (2) a minimalist serialization format for tool schemas to minimize token overhead per tool; and (3) a just-in-time schema-passing mechanism that loads full tool definitions only upon tool selection. We instantiate this framework by adapting a 3B parameter SLM to context-efficient trajectories and rigorously evaluate it against a conventional baseline on complex user tasks. Our agent matches, or exceeds, the performance of a conventional baseline while dramatically compressing context, achieving more than a 6-fold reduction in initial system prompt context and a 10- to 25-fold reduction in context growth rate based on the interaction verbosity, demonstrating that strategic context management is key to unlocking capable and persistent on-device AI.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[tool-use]] · [[agent-memory]] · [[llm-as-judge]] · [[distillation]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2511.03728v1)
