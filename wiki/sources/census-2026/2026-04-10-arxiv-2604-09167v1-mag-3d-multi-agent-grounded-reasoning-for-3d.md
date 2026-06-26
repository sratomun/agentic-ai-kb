---
type: source
source_type: arxiv
title: "MAG-3D: Multi-Agent Grounded Reasoning for 3D Understanding"
authors: Henry Zheng, Chenyue Fang, Rui Huang, Siyuan Wei et al.
url: https://arxiv.org/abs/2604.09167v1
date: 2026-04-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 23
primary: cs.CV
tags: [coding-agents, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# MAG-3D: Multi-Agent Grounded Reasoning for 3D Understanding

**arXiv:** [2604.09167v1](https://arxiv.org/abs/2604.09167v1) · 2026-04-10 · cs.CV
**Authors:** Henry Zheng, Chenyue Fang, Rui Huang, Siyuan Wei et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Vision-language models (VLMs) have achieved strong performance in multimodal understanding and reasoning, yet grounded reasoning in 3D scenes remains underexplored. Effective 3D reasoning hinges on accurate grounding: to answer open-ended queries, a model must first identify query-relevant objects and regions in a complex scene, and then reason about their spatial and geometric relationships. Recent approaches have demonstrated strong potential for grounded 3D reasoning. However, they often rely on in-domain tuning or hand-crafted reasoning pipelines, which limit their flexibility and zero-shot generalization to novel environments. In this work, we present MAG-3D, a training-free multi-agent framework for grounded 3D reasoning with off-the-shelf VLMs. Instead of relying on task-specific training or fixed reasoning procedures, MAG-3D dynamically coordinates expert agents to address the key challenges of 3D reasoning. Specifically, we propose a planning agent that decomposes the task and orchestrates the overall reasoning process, a grounding agent that performs free-form 3D grounding and relevant frame retrieval from extensive 3D scene observations, and a coding agent that conducts flexible geometric reasoning and explicit verification through executable programs. This multi-agent collaborative design enables flexible training-free 3D grounded reasoning across diverse scenes and achieves state-of-the-art performance on challenging benchmarks.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.09167v1)
