---
type: source
source_type: arxiv
title: "Towards Scalable Lightweight GUI Agents via Multi-role Orchestration"
authors: Ziwei Wang, Junjie Zheng, Leyang Yang, Sheng Zhou et al.
url: https://arxiv.org/abs/2604.13488v1
date: 2026-04-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [computer-use-agents, agentic-rl, agent-skills, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# Towards Scalable Lightweight GUI Agents via Multi-role Orchestration

**arXiv:** [2604.13488v1](https://arxiv.org/abs/2604.13488v1) · 2026-04-15 · cs.AI
**Authors:** Ziwei Wang, Junjie Zheng, Leyang Yang, Sheng Zhou et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Autonomous Graphical User Interface (GUI) agents powered by Multimodal Large Language Models (MLLMs) enable digital automation on end-user devices. While scaling both parameters and data has yielded substantial gains, advanced methods still suffer from prohibitive deployment costs on resource-constrained devices. When facing complex in-the-wild scenarios, lightweight GUI agents are bottlenecked by limited capacity and poor task scalability under end-to-end episodic learning, impeding adaptation to multi-agent systems (MAS), while training multiple skill-specific experts remains costly. Can we strike an effective trade-off in this cost-scalability dilemma, enabling lightweight MLLMs to participate in realistic GUI workflows? To address these challenges, we propose the LAMO framework, which endows a lightweight MLLM with GUI-specific knowledge and task scalability, allowing multi-role orchestration to expand its capability boundary for GUI automation. LAMO combines role-oriented data synthesis with a two-stage training recipe: (i) supervised fine-tuning with Perplexity-Weighted Cross-Entropy optimization for knowledge distillation and visual perception enhancement, and (ii) reinforcement learning for role-oriented cooperative exploration. With LAMO, we develop a task-scalable native GUI agent, LAMO-3B, supporting monolithic execution and MAS-style orchestration. When paired with advanced planners as a plug-and-play policy executor, LAMO-3B can continuously benefit from planner advances, enabling a higher performance ceiling. Extensive static and online evaluations validate the effectiveness of our design.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agentic-rl|Agentic RL]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.13488v1)
