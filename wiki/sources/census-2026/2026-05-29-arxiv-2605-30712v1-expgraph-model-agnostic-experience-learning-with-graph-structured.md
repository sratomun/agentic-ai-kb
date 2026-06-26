---
type: source
source_type: arxiv
title: "ExpGraph: Model-Agnostic Experience Learning with Graph-Structured Memory for LLM Agents"
authors: Tao Feng, Chongrui Ye, Tianyang Luo, Jingjun Xu et al.
url: https://arxiv.org/abs/2605.30712v1
date: 2026-05-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.CL
tags: [coding-agents, self-evolving-agents, agentic-rl, agent-skills, agent-memory, arxiv, auto-ingested]
---

# ExpGraph: Model-Agnostic Experience Learning with Graph-Structured Memory for LLM Agents

**arXiv:** [2605.30712v1](https://arxiv.org/abs/2605.30712v1) · 2026-05-29 · cs.CL
**Authors:** Tao Feng, Chongrui Ye, Tianyang Luo, Jingjun Xu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language model (LLM) agents have shown strong capabilities in reasoning, tool use, and multi-step interaction, but they often solve tasks from scratch and fail to reuse successful strategies or failure lessons from prior experience. Fine-tuning on collected experience can improve reuse, but it is inflexible when stronger or more suitable executors emerge. We propose ExpGraph, a model-agnostic experience learning framework that enables frozen and replaceable LLM executors to improve through external experience reuse without parameter updates. ExpGraph summarizes historical trajectories into reusable skills and failure lessons, organizes them as nodes in a self-evolving experience graph, and retrieves useful experiences through graph diffusion and utility-aware ranking. A lightweight retrieval copilot is trained with reinforcement learning using feedback that compares executor performance with and without retrieved experiences, while the graph is updated online from downstream task outcomes. We evaluate ExpGraph on ExpSuite, covering question answering, mathematical reasoning, code generation, and multi-step agentic environments including ALFWorld and AppWorld. ExpGraph improves over the strongest baseline by 12.2% and 4.7% on static tasks with smaller and larger executors, and by 21.4% and 12.7% in agentic environments, while reducing average interaction steps by 12.7% and 21.6%. Ablations show that graph-structured experience, utility-aware ranking, and adaptive retrieval jointly enable effective experience reuse across diverse tasks and executor models.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]]
- **Entities:** [[alfworld]] · [[appworld]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.30712v1)
