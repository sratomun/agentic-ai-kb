---
type: source
source_type: arxiv
title: "Hybrid Self-evolving Structured Memory for GUI Agents"
authors: Sibo Zhu, Wenyi Wu, Kun Zhou, Stephen Wang et al.
url: https://arxiv.org/abs/2603.10291v1
date: 2026-03-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.AI
tags: [computer-use-agents, knowledge-graph, self-evolving-agents, agent-memory, arxiv, auto-ingested]
---

# Hybrid Self-evolving Structured Memory for GUI Agents

**arXiv:** [2603.10291v1](https://arxiv.org/abs/2603.10291v1) · 2026-03-11 · cs.AI
**Authors:** Sibo Zhu, Wenyi Wu, Kun Zhou, Stephen Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The remarkable progress of vision-language models (VLMs) has enabled GUI agents to interact with computers in a human-like manner. Yet real-world computer-use tasks remain difficult due to long-horizon workflows, diverse interfaces, and frequent intermediate errors. Prior work equips agents with external memory built from large collections of trajectories, but relies on flat retrieval over discrete summaries or continuous embeddings, falling short of the structured organization and self-evolving characteristics of human memory. Inspired by the brain, we propose Hybrid Self-evolving Structured Memory (HyMEM), a graph-based memory that couples discrete high-level symbolic nodes with continuous trajectory embeddings. HyMEM maintains a graph structure to support multi-hop retrieval, self-evolution via node update operations, and on-the-fly working-memory refreshing during inference. Extensive experiments show that HyMEM consistently improves open-source GUI agents, enabling 7B/8B backbones to match or surpass strong closed-source models; notably, it boosts Qwen2.5-VL-7B by +22.5% and outperforms Gemini2.5-Pro-Vision and GPT-4o.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[knowledge-graph|Knowledge graphs]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-memory|Agent memory]]
- **Entities:** [[gpt-5]] · [[qwen]] · [[gemini]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.10291v1)
