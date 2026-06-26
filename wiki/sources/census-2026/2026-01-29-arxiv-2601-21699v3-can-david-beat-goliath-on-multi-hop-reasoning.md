---
type: source
source_type: arxiv
title: "Can David Beat Goliath? On Multi-Hop Reasoning with Resource-Constrained Agents"
authors: Hojae Han, Heeyun Jung, Jongyoon Kim, Seung-won Hwang
url: https://arxiv.org/abs/2601.21699v3
date: 2026-01-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CL
tags: [agentic-rl, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Can David Beat Goliath? On Multi-Hop Reasoning with Resource-Constrained Agents

**arXiv:** [2601.21699v3](https://arxiv.org/abs/2601.21699v3) · 2026-01-29 · cs.CL
**Authors:** Hojae Han, Heeyun Jung, Jongyoon Kim, Seung-won Hwang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-turn reasoning agents solve complex questions by decomposing them into intermediate retrieval or tool-use steps, for accumulating supporting evidence across turns. Meanwhile, with reinforcement learning (RL), training these agents rely on many on-policy rollouts and large training batches. Under realistic resource constraints that make dense exploration infeasible, each RL batch contains only few useful reasoning paths from the current policy. Existing approaches do not fully address this bottleneck: SFT-based initialization can overfit when annotated trajectories are scarce, retrieval-level rewards can assign credit to individual retrieved documents without directly optimizing coverage of the full evidence set, and expansion can waste rollouts from poorly chosen prefixes. We introduce David-GRPO, which improves small-batch learning by using information from both outside and inside the current policy: (i) expert bootstrapping injects a few off-policy expert trajectories into RL updates, and (ii) evidence-guided exploration turns on-policy partial successes into evidence-coverage scores and additional continuations. On agents up to 1.5B parameters trained on four RTX 3090 GPUs, David-GRPO improves over prior RL baselines under the same low-budget setting on six multi-hop QA benchmarks. The gains come with a behavioral shift: unlike prior low-budget RL baselines that often skip retrieval or stop after shallow search, David-GRPO learns to increase retrieval depth and evidence coverage.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.21699v3)
