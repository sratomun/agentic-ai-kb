---
type: source
source_type: arxiv
title: "SeeUPO: Sequence-Level Agentic-RL with Convergence Guarantees"
authors: Tianyi Hu, Qingxu Fu, Yanxi Chen, Zhaoyang Liu et al.
url: https://arxiv.org/abs/2602.06554v1
date: 2026-02-06
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.AI
tags: [agentic-rl, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# SeeUPO: Sequence-Level Agentic-RL with Convergence Guarantees

**arXiv:** [2602.06554v1](https://arxiv.org/abs/2602.06554v1) · 2026-02-06 · cs.AI
**Authors:** Tianyi Hu, Qingxu Fu, Yanxi Chen, Zhaoyang Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Reinforcement learning (RL) has emerged as the predominant paradigm for training large language model (LLM)-based AI agents. However, existing backbone RL algorithms lack verified convergence guarantees in agentic scenarios, especially in multi-turn settings, which can lead to training instability and failure to converge to optimal policies. In this paper, we systematically analyze how different combinations of policy update mechanisms and advantage estimation methods affect convergence properties in single/multi-turn scenarios. We find that REINFORCE with Group Relative Advantage Estimation (GRAE) can converge to the globally optimal under undiscounted conditions, but the combination of PPO & GRAE breaks PPO's original monotonic improvement property. Furthermore, we demonstrate that mainstream backbone RL algorithms cannot simultaneously achieve both critic-free and convergence guarantees in multi-turn scenarios. To address this, we propose SeeUPO (Sequence-level Sequential Update Policy Optimization), a critic-free approach with convergence guarantees for multi-turn interactions. SeeUPO models multi-turn interaction as sequentially executed multi-agent bandit problems. Through turn-by-turn sequential policy updates in reverse execution order, it ensures monotonic improvement and convergence to global optimal solution via backward induction. Experiments on AppWorld and BFCL v4 demonstrate SeeUPO's substantial improvements over existing backbone algorithms: relative gains of 43.3%-54.6% on Qwen3-14B and 24.1%-41.9% on Qwen2.5-14B (averaged across benchmarks), along with superior training stability.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[qwen]] · [[ppo]] · [[bfcl]] · [[appworld]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.06554v1)
