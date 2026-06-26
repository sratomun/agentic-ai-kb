---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Bridging the Reasoning Gap in Vietnamese with Small Language Models via Test-Time Scaling"
authors: Bui The Trung et al.
url: https://arxiv.org/abs/2604.17794v1
date: 2026-04-20
score: 9
primary: cs.CL
tags: [arxiv, auto-ingested, small-language-models, llm-as-judge, post-training, reasoning-models]
---

# Bridging the Reasoning Gap in Vietnamese with Small Language Models via Test-Time Scaling

**arXiv:** [2604.17794v1](https://arxiv.org/abs/2604.17794v1) · 2026-04-20 · cs.CL
**Authors:** Bui The Trung et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The democratization of ubiquitous AI hinges on deploying sophisticated reasoning capabilities on resource-constrained devices. However, Small Language Models (SLMs) often face a "reasoning gap", particularly in non-English languages like Vietnamese, where they struggle to maintain coherent chains of thought. This paper investigates Test-Time Scaling strategies for the Qwen3-1.7B architecture within the context of Vietnamese Elementary Mathematics. We introduce Vi-S1K, a high-fidelity reasoning dataset localized via a Gemini 2.5 Flash-Lite powered pipeline, and Vi-Elementary-Bench, a dual-resource benchmark for rigorous evaluation. Using an LLM-as-a-Judge protocol, we reveal that the base model possesses robust latent knowledge (Accuracy: 4.05/5.00) but suffers from a severe "formatting gap" in communication. Supervised Fine-Tuning (SFT) acts as a critical "reasoning unlocker", yielding a 77% improvement in Explanation Quality and bridging the gap between raw calculation and pedagogical coherence. Furthermore, our analysis of prompting strategies uncovers a significant trade-off: structured frameworks like ReAct impose a "cognitive tax" on the 1.7B parameter capacity, degrading performance relative to pure Chain-of-Thought (CoT) combined with Self-Consistency. These findings establish a deployment hierarchy for SLMs, demonstrating that SFT combined with simplified test-time scaling is superior to complex agentic workflows for edge-based reasoning.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[llm-as-judge]] · [[post-training]] · [[reasoning-models]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.17794v1)
