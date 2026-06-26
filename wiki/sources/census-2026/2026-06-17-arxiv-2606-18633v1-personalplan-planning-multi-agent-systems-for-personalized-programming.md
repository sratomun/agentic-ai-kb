---
type: source
source_type: arxiv
title: "PersonalPlan: Planning Multi-Agent Systems for Personalized Programming Learning"
authors: Zhiyuan Wen, Jiannong Cao, Peng Gao, Haochen Shi et al.
url: https://arxiv.org/abs/2606.18633v1
date: 2026-06-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.MA
tags: [agentic-rl, multi-agent-systems, arxiv, auto-ingested]
---

# PersonalPlan: Planning Multi-Agent Systems for Personalized Programming Learning

**arXiv:** [2606.18633v1](https://arxiv.org/abs/2606.18633v1) · 2026-06-17 · cs.MA
**Authors:** Zhiyuan Wen, Jiannong Cao, Peng Gao, Haochen Shi et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Effective programming education requires personalized instruction adapted to diverse learner backgrounds. However, while LLM-based multi-agent systems (MAS) excel at complex planning, existing planners often lack profile-grounding and pedagogical scaffolding, thereby undermining personalized programming learning. To fill in the gap, we first introduce \textbf{MAP-PPL} (\textbf{M}ulti-\textbf{A}gent \textbf{P}lans for \textbf{P}ersonalized \textbf{P}rogramming \textbf{L}earning), a profile-conditioned multi-agent planning dataset with 3{,}043 query--profile--plan instances from 1{,}730 Stack Overflow question groups and 2{,}738 learner profiles. Each plan specifies agents, subtasks, executable steps, and prerequisite dependencies. Then, we propose \textbf{PersonalPlan}, a two-stage MAS planner that first performs hierarchical SFT with separate LoRA adapters for profile-aware task decomposition and step dependency planning, then applies a Reward-Adaptive GRPO to encourage the model to generate executable, personalized, and pedagogically scaffolded plans. Extensive experiments on MAP-PPL comparing PersonalPlan against frontier LLMs, generic MAS frameworks, and agentic planners demonstrate its superiority. With only 8B and 32B variants, PersonalPlan achieves state-of-the-art plan executability, personalization, and pedagogical quality, effectively orchestrating MAS for agent-student interactions.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.18633v1)
