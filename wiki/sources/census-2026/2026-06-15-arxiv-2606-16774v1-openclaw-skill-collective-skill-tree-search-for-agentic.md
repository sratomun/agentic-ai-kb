---
type: source
source_type: arxiv
title: "OpenClaw-Skill: Collective Skill Tree Search for Agentic Large Language Models"
authors: Tianyi Lin, Chuanyu Sun, Jingyi Zhang, Changxu Wei et al.
url: https://arxiv.org/abs/2606.16774v1
date: 2026-06-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 22
primary: cs.AI
tags: [agentic-rl, agent-skills, agent-memory, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# OpenClaw-Skill: Collective Skill Tree Search for Agentic Large Language Models

**arXiv:** [2606.16774v1](https://arxiv.org/abs/2606.16774v1) · 2026-06-15 · cs.AI
**Authors:** Tianyi Lin, Chuanyu Sun, Jingyi Zhang, Changxu Wei et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Equipping Large Language Model (LLM) agents with effective skills is crucial for solving complex tasks in real-world systems like OpenClaw. In this work, we aim to develop a framework that automatically constructs such reusable skills to enhance LLMs in tool use, multi-step reasoning, and dynamic environment interaction. To this end, we propose Collective Skill Tree Search (CSTS), a novel tree-search-based skill construction framework that constructs structured, diverse and generalizable tree of skills. The core idea of CSTS is to leverage collective intelligence to jointly search, identify and compose effective skills via two iterative phases: Collective Skill Node Generation (CSN-Gen) and Collective Skill Node Assessment (CSN-Assess). CSN-Gen exploits collective knowledge from multiple models to explore diverse candidate skills for each subtask, enabling comprehensive skill exploration. CSN-Assess employs multiple models as judges to evaluate and select skill nodes with two scoring mechanisms: (1) collective quality scoring that aggregates independent evaluations to produce a robust estimate of skill effectiveness, and (2) collective transferability scoring that explicitly verifies whether a skill generalizes well across different models. With CSTS, we construct a set of comprehensive tree of skills along with skill-augmented training data, enabling models to effectively learn and utilize skills. Besides, we introduce Collective Skill Reinforcement Learning, which actively selects multiple relevant skills from the tree to broaden solution-space exploration, avoid being trapped by a single skill and its resulting homogeneous or suboptimal solutions. As a result, our trained model, OpenClaw-Skill, exhibits outstanding agentic capabilities in long-horizon planning, tool use and generalization over challenging benchmarks.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.16774v1)
