---
type: source
source_type: arxiv
title: "KLDrive: Fine-Grained 3D Scene Reasoning for Autonomous Driving based on Knowledge Graph"
authors: Ye Tian, Jingyi Zhang, Zihao Wang, Xiaoyuan Ren et al.
url: https://arxiv.org/abs/2603.21029v1
date: 2026-03-22
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.AI
tags: [autonomous-driving-agents, knowledge-graph, agent-reliability, agent-evaluation, arxiv, auto-ingested]
---

# KLDrive: Fine-Grained 3D Scene Reasoning for Autonomous Driving based on Knowledge Graph

**arXiv:** [2603.21029v1](https://arxiv.org/abs/2603.21029v1) · 2026-03-22 · cs.AI
**Authors:** Ye Tian, Jingyi Zhang, Zihao Wang, Xiaoyuan Ren et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Autonomous driving requires reliable reasoning over fine-grained 3D scene facts. Fine-grained question answering over multi-modal driving observations provides a natural way to evaluate this capability, yet existing perception pipelines and driving-oriented large language model (LLM) methods still suffer from unreliable scene facts, hallucinations, opaque reasoning, and heavy reliance on task-specific training. We present KLDrive, the first knowledge-graph-augmented LLM reasoning framework for fine-grained question answering in autonomous driving. KLDrive addresses this problem through designing two tightly coupled components: an energy-based scene fact construction module that consolidates multi-source evidence into a reliable scene knowledge graph, and an LLM agent that performs fact-grounded reasoning over a constrained action space under explicit structural constraints. By combining structured prompting with few-shot in-context exemplars, the framework adapts to diverse reasoning tasks without heavy task-specific fine-tuning. Experiments on two large-scale autonomous-driving QA benchmarks show that KLDrive outperforms prior state-of-the-art methods, achieving the best overall accuracy of 65.04% on NuScenes-QA and the best SPICE score of 42.45 on GVQA. On counting, the most challenging factual reasoning task, it improves over the strongest baseline by 46.01 percentage points, demonstrating substantially reduced hallucinations and the benefit of coupling reliable scene fact construction with explicit reasoning.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.21029v1)
