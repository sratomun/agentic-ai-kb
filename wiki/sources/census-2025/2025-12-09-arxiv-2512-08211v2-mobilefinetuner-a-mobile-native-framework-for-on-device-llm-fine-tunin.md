---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "MobileFineTuner: A Mobile-Native Framework for On-Device LLM Fine-Tuning in Real-World Embedded AI Applications"
authors: Jiaxiang Geng et al.
url: https://arxiv.org/abs/2512.08211v2
date: 2025-12-09
score: 0
primary: cs.LG
tags: [arxiv, auto-ingested, small-language-models, agent-memory, llm-as-judge, post-training, clinical-agents]
---

# MobileFineTuner: A Mobile-Native Framework for On-Device LLM Fine-Tuning in Real-World Embedded AI Applications

**arXiv:** [2512.08211v2](https://arxiv.org/abs/2512.08211v2) · 2025-12-09 · cs.LG
**Authors:** Jiaxiang Geng et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models (LLMs) are moving from cloud-centric services toward on-device embedded AI, where models interact with private, longitudinal signals sensed from users and their physical environments. Mobile phones are a natural platform for such applications because they are continuously carried by users, connected to wearable sensors, and deeply integrated with daily mobile applications. However, practical LLM fine-tuning on commodity phones remains difficult. Existing fine-tuning frameworks are largely Python-based and server-oriented, making them hard to deploy inside mobile applications. We present MobileFineTuner, a mobile-native open-source framework for end-to-end LLM fine-tuning on commodity mobile phones. MobileFineTuner is implemented in C++ and provides a reusable training stack. To make fine-tuning feasible under mobile resource constraints, MobileFineTuner integrates a resource-aware training runtime with memory-efficient attention, activation checkpointing, gradient accumulation, parameter sharding, and energy-aware scheduling. We evaluate MobileFineTuner on real mobile phones using GPT-2, Gemma 3, and Qwen2.5 models across multiple fine-tuning tasks. The results show that MobileFineTuner reproduces standard Full-FT and LoRA fine-tuning behavior, substantially reduces memory pressure and improves executability on memory-constrained phones. We further demonstrate MobileFineTuner through a private campus health-agent application, where a local LLM is fine-tuned on user-specific wearable-sensing records to provide more personalized responses while keeping raw records on the phone. These results establish MobileFineTuner as a practical toolkit for studying and building on-device LLM fine-tuning applications in embedded AI and sensing systems.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[agent-memory]] · [[llm-as-judge]] · [[post-training]] · [[clinical-agents]]
- **Entities:** [[gemma]] · [[qwen]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2512.08211v2)
