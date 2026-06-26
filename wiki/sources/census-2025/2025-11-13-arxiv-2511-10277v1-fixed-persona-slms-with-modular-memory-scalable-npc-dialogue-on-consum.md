---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Fixed-Persona SLMs with Modular Memory: Scalable NPC Dialogue on Consumer Hardware"
authors: Martin Braas et al.
url: https://arxiv.org/abs/2511.10277v1
date: 2025-11-13
score: 3
primary: cs.AI
tags: [arxiv, auto-ingested, small-language-models, agent-memory, llm-as-judge, post-training]
---

# Fixed-Persona SLMs with Modular Memory: Scalable NPC Dialogue on Consumer Hardware

**arXiv:** [2511.10277v1](https://arxiv.org/abs/2511.10277v1) · 2025-11-13 · cs.AI
**Authors:** Martin Braas et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) have demonstrated remarkable capabilities in generating human-like text, yet their applicability to dialogue systems in computer games remains limited. This limitation arises from their substantial hardware requirements, latency constraints, and the necessity to maintain clearly defined knowledge boundaries within a game setting. In this paper, we propose a modular NPC dialogue system that leverages Small Language Models (SLMs), fine-tuned to encode specific NPC personas and integrated with runtime-swappable memory modules. These memory modules preserve character-specific conversational context and world knowledge, enabling expressive interactions and long-term memory without retraining or model reloading during gameplay. We comprehensively evaluate our system using three open-source SLMs: DistilGPT-2, TinyLlama-1.1B-Chat, and Mistral-7B-Instruct, trained on synthetic persona-aligned data and benchmarked on consumer-grade hardware. While our approach is motivated by applications in gaming, its modular design and persona-driven memory architecture hold significant potential for broader adoption in domains requiring expressive, scalable, and memory-rich conversational agents, such as virtual assistants, customer support bots, or interactive educational systems.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[agent-memory]] · [[llm-as-judge]] · [[post-training]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2511.10277v1)
