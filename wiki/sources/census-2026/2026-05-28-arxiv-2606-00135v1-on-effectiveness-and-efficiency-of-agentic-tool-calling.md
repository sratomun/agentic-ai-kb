---
type: source
source_type: arxiv
title: "On Effectiveness and Efficiency of Agentic Tool-calling and RL Training"
authors: Tong Liu, Cheng Qian, Matej Cief, Yuan He et al.
url: https://arxiv.org/abs/2606.00135v1
date: 2026-05-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.LG
tags: [agent-reliability, agentic-rl, agent-skills, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# On Effectiveness and Efficiency of Agentic Tool-calling and RL Training

**arXiv:** [2606.00135v1](https://arxiv.org/abs/2606.00135v1) · 2026-05-28 · cs.LG
**Authors:** Tong Liu, Cheng Qian, Matej Cief, Yuan He et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Tool-calling is a central component of modern large language model (LLM) agents, equipping them with skills beyond their parametric knowledge. This paper studies tool-calling along two complementary axes: effectiveness, i.e., how this capability is measured, and efficiency, i.e., how it is learned. On effectiveness, we systematically analyze tool-calling evaluation pipelines and show that results can be highly sensitive to seemingly minor, often undocumented implementation choices including the random seed, system prompt, multi-turn template construction, and how prior interaction/reasoning history is carried forward. These choices can lead to substantial differences in reported performance, especially in multi-turn settings where without rigorous standardization, leaderboard rankings are unreliable. On efficiency, we examine standard reinforcement learning (RL) for tool-calling and identify two sources of computational waste: (i) during rollouts, many prompts produce no learning signal, and (ii) during policy updates, optimization incurs high computational cost. Guided by these findings, we introduce two techniques that accelerate RL-based tool-calling training, achieving substantial wall-clock speedup without degrading performance.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-skills|Agent skills]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.00135v1)
