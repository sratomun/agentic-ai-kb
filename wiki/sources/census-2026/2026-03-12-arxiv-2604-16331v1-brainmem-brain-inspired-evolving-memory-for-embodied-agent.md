---
type: source
source_type: arxiv
title: "BrainMem: Brain-Inspired Evolving Memory for Embodied Agent Task Planning"
authors: Xiaoyu Ma, Lianyu Hu, Wenbing Tang, Zixuan Hu et al.
url: https://arxiv.org/abs/2604.16331v1
date: 2026-03-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 7
primary: cs.RO
tags: [embodied-agents, knowledge-graph, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# BrainMem: Brain-Inspired Evolving Memory for Embodied Agent Task Planning

**arXiv:** [2604.16331v1](https://arxiv.org/abs/2604.16331v1) · 2026-03-12 · cs.RO
**Authors:** Xiaoyu Ma, Lianyu Hu, Wenbing Tang, Zixuan Hu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Embodied task planning requires agents to execute long-horizon, goal-directed actions in complex 3D environments, where success depends on both immediate perception and accumulated experience across tasks. However, most existing LLM-based planners are stateless and reactive, operating without persistent memory and therefore repeating errors and struggling with spatial or temporal dependencies. We propose BrainMem(Brain-Inspired Evolving Memory), a training-free hierarchical memory system that equips embodied agents with working, episodic, and semantic memory inspired by human cognition. BrainMem continuously transforms interaction histories into structured knowledge graphs and distilled symbolic guidelines, enabling planners to retrieve, reason over, and adapt behaviors from past experience without any model fine-tuning or additional training. This plug-and-play design integrates seamlessly with arbitrary multi-modal LLMs and greatly reduces reliance on task-specific prompt engineering. Extensive experiments on four representative benchmarks, including EB-ALFRED, EB-Navigation, EB-Manipulation, and EB-Habitat, demonstrate that BrainMem significantly enhances task success rates across diverse models and difficulty subsets, with the largest gains observed on long-horizon and spatially complex tasks. These results highlight evolving memory as a promising and scalable mechanism for generalizable embodied intelligence.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.16331v1)
