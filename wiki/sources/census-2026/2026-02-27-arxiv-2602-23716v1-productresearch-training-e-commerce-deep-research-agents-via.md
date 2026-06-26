---
type: source
source_type: arxiv
title: "ProductResearch: Training E-Commerce Deep Research Agents via Multi-Agent Synthetic Trajectory Distillation"
authors: Jiangyuan Wang, Kejun Xiao, Huaipeng Zhao, Tao Luo et al.
url: https://arxiv.org/abs/2602.23716v1
date: 2026-02-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [science-agents, agent-memory, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# ProductResearch: Training E-Commerce Deep Research Agents via Multi-Agent Synthetic Trajectory Distillation

**arXiv:** [2602.23716v1](https://arxiv.org/abs/2602.23716v1) · 2026-02-27 · cs.AI
**Authors:** Jiangyuan Wang, Kejun Xiao, Huaipeng Zhao, Tao Luo et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Model (LLM)-based agents show promise for e-commerce conversational shopping, yet existing implementations lack the interaction depth and contextual breadth required for complex product research. Meanwhile, the Deep Research paradigm, despite advancing information synthesis in web search, suffers from domain gaps when transferred to e-commerce. We propose ProductResearch, a multi-agent framework that synthesizes high-fidelity, long-horizon tool-use trajectories for training robust e-commerce shopping agents. The framework employs a User Agent to infer nuanced shopping intents from behavioral histories, and a Supervisor Agent that orchestrates iterative collaboration with a Research Agent to generate synthetic trajectories culminating in comprehensive, insightful product research reports. These trajectories are rigorously filtered and distilled through a reflective internalization process that consolidates multi-agent supervisory interactions into coherent single-role training examples, enabling effective fine-tuning of LLM agents for complex shopping inquiries. Extensive experiments show that a compact MoE model fine-tuned on our synthetic data achieves substantial improvements over its base model in response comprehensiveness, research depth, and user-perceived utility, approaching the performance of frontier proprietary deep research systems and establishing multi-agent synthetic trajectory training as an effective and scalable paradigm for enhancing LLM-based shopping assistance.

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.23716v1)
