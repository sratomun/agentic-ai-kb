---
type: source
source_type: arxiv
title: "From Correctness to Preference: A Framework for Personalized Agentic Reinforcement Learning"
authors: Ranxu zhang, zeyang li, Jiacheng Huang, Rui Zhang et al.
url: https://arxiv.org/abs/2605.23382v1
date: 2026-05-22
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.CL
tags: [knowledge-graph, agentic-rl, agent-skills, agent-memory, tool-use, arxiv, auto-ingested]
---

# From Correctness to Preference: A Framework for Personalized Agentic Reinforcement Learning

**arXiv:** [2605.23382v1](https://arxiv.org/abs/2605.23382v1) · 2026-05-22 · cs.CL
**Authors:** Ranxu zhang, zeyang li, Jiacheng Huang, Rui Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic reinforcement learning (Agentic RL) has achieved strong progress in tasks with clear success signals. However, many real-world agent applications require user-conditioned behavior: the same query may call for different planning strategies and tool-use decisions across users. This setting raises key challenges: generic rewards cannot capture heterogeneous user preferences, observed behaviors are entangled with conformity effects, and flat memories cannot support personalized skill retrieval. To this end, we propose a unified personalized Agentic RL framework that embeds personalization into training-time optimization. At its core is \emph{Personalized Anchor Reward-Decoupled Policy Optimization} (\textbf{PARPO}), which decouples generic task-quality rewards from personalized preference rewards and uses user-specific anchors to stabilize learning under heterogeneous reward scales. We further introduce a two-stage preference-disentangled reward model and \emph{Preference-Aligned Skill Evolution Graph Memory} (\textbf{PSGM}) for personalized supervision and preference-aligned skill retrieval. Together, they form a closed loop of preference identification, policy optimization, and structured skill accumulation. Experiments on ETAPP, ETAPP-Hard, and SJAgent show that our framework consistently outperforms strong memory and RL baselines. Code and data are included in the supplementary materials.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.23382v1)
