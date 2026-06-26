---
type: source
source_type: arxiv
title: "RLAR: An Agentic Reward System for Multi-task Reinforcement Learning on Large Language Models"
authors: Andrew Zhuoer Feng, Cunxiang Wang, Bosi Wen, Yidong Wang et al.
url: https://arxiv.org/abs/2603.00724v1
date: 2026-02-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 22
primary: cs.CL
tags: [coding-agents, self-evolving-agents, agentic-rl, multi-agent-systems, arxiv, auto-ingested]
---

# RLAR: An Agentic Reward System for Multi-task Reinforcement Learning on Large Language Models

**arXiv:** [2603.00724v1](https://arxiv.org/abs/2603.00724v1) · 2026-02-28 · cs.CL
**Authors:** Andrew Zhuoer Feng, Cunxiang Wang, Bosi Wen, Yidong Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language model alignment via reinforcement learning depends critically on reward function quality. However, static, domain-specific reward models are often costly to train and exhibit poor generalization in out-of-distribution scenarios encountered during RL iterations. We present RLAR (Reinforcement Learning from Agent Rewards), an agent-driven framework that dynamically assigns tailored reward functions to individual queries. Specifically, RLAR transforms reward acquisition into a dynamic tool synthesis and invocation task. It leverages LLM agents to autonomously retrieve optimal reward models from the Internet and synthesize programmatic verifiers through code generation. This allows the reward system to self-evolve with the shifting data distributions during training. Experimental results demonstrate that RLAR yields consistent performance gains ranging from 10 to 60 across mathematics, coding, translation, and dialogue tasks. On RewardBench-V2, RLAR significantly outperforms static baselines and approaches the performance upper bound, demonstrating superior generalization through dynamic reward orchestration. The data and code are available on this link: https://github.com/ZhuoerFeng/RLAR.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.00724v1)
