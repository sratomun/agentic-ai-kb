---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Small Language Model Agents Enable Efficient and High-Quality Knowledge Mining"
authors: Sipeng Zhang et al.
url: https://arxiv.org/abs/2510.01427v3
date: 2025-10-01
score: 12
primary: cs.AI
tags: [arxiv, auto-ingested, small-language-models, llm-as-judge, reasoning-models]
---

# Small Language Model Agents Enable Efficient and High-Quality Knowledge Mining

**arXiv:** [2510.01427v3](https://arxiv.org/abs/2510.01427v3) · 2025-10-01 · cs.AI
**Authors:** Sipeng Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
At the core of Deep Research is knowledge mining, the task of extracting structured information from massive unstructured text in response to user instructions. Large language models (LLMs) excel at interpreting such instructions but are prohibitively expensive to deploy at scale, while traditional pipelines of classifiers and extractors remain efficient yet brittle and unable to generalize to new tasks. We introduce Falconer, a collaborative framework that combines the agentic reasoning of LLMs with lightweight proxy models for scalable knowledge mining. In Falconer, LLMs act as planners, decomposing user instructions into executable pipelines, and as annotators, generating supervision to train small proxies. The framework unifies classification and extraction into two atomic operations, get label and get span, enabling a single instruction-following model to replace multiple task-specific components. To evaluate the consistency between proxy models incubated by Falconer and annotations provided by humans and large models, we construct new benchmarks covering both planning and end-to-end execution. Experiments show that Falconer closely matches state-of-the-art LLMs in instruction-following accuracy while reducing inference cost by up to 90% and accelerating large-scale knowledge mining by more than 20x, offering an efficient and scalable foundation for Deep Research.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[llm-as-judge]] · [[reasoning-models]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2510.01427v3)
