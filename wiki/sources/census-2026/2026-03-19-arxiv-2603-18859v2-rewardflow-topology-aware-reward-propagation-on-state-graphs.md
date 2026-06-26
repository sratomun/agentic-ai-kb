---
type: source
source_type: arxiv
title: "RewardFlow: Topology-Aware Reward Propagation on State Graphs for Agentic RL with Large Language Models"
authors: Xiao Feng, Bo Han, Zhanke Zhou, Jiaqi Fan et al.
url: https://arxiv.org/abs/2603.18859v2
date: 2026-03-19
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [agent-reliability, agentic-rl, agent-evaluation, arxiv, auto-ingested]
---

# RewardFlow: Topology-Aware Reward Propagation on State Graphs for Agentic RL with Large Language Models

**arXiv:** [2603.18859v2](https://arxiv.org/abs/2603.18859v2) · 2026-03-19 · cs.AI
**Authors:** Xiao Feng, Bo Han, Zhanke Zhou, Jiaqi Fan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Reinforcement learning (RL) shows promise for enhancing LLM agentic reasoning, yet sparse terminal rewards hinder fine-grained optimization. Process reward modeling offers an alternative but incurs high computational costs, reward hacking risks, and annotation bottlenecks. We introduce RewardFlow, a lightweight method for estimating state-level rewards in agentic reasoning. By constructing state graphs that capture the intrinsic topological structure of trajectories, RewardFlow performs topology-aware propagation to estimate each state's contribution to success, yielding principled, annotation-free dense rewards. Used for RL optimization, RewardFlow substantially outperforms prior baselines across four agentic benchmarks: +6.2% average success rate on text-based tasks, +29.7% on visual reasoning over the strongest baseline across three model scales, and +10% accuracy on DeepResearch, with superior robustness and training efficiency. The implementation of RewardFlow is publicly available at https://github.com/tmlr-group/RewardFlow.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.18859v2)
