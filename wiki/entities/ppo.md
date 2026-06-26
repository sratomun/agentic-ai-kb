---
type: entity
entity_type: method
tags: [agents, method]
created: 2026-06-21
updated: 2026-06-22
census_count: 118
---

# PPO

*Proximal Policy Optimization — the classic RL algorithm, still a strong baseline for agent training in 2025–26.*

## What it is
PPO (Proximal Policy Optimization) is a policy-gradient RL algorithm that constrains policy updates to avoid large changes. It remains the dominant RL baseline for LLM training on planning and multi-agent tasks, mentioned in ~118 of 2026 H1 census papers.

## Why it matters
PPO is the incumbent against which every new RL training algorithm (GRPO, DPO, RLVR) is compared. When a new agentic RL paper claims an improvement, knowing PPO's performance is the baseline check — and in some multi-agent settings it still wins.

## Relationships
- used in [[agentic-rl]]
- compare [[grpo]], [[dpo]]
- part of [[post-training]]; optimizes a [[reward-modeling|reward model]]

## Cited by (2025 deep notes)
- **127** · [[2025-08-27-arxiv-2508-19828v5-memory-r1-enhancing-large-language-model-agents-to|Memory-R1: Enhancing Large Language Model Agents to Manage and Utilize Memori...]]
- **112** · [[2025-04-12-arxiv-2504-09037v4-a-survey-of-frontiers-in-llm-reasoning-inference|A Survey of Frontiers in LLM Reasoning: Inference Scaling, Learning to Reason...]]
- **68** · [[2025-01-04-arxiv-2501-03262v9-reinforce-stabilizing-critic-free-policy-optimization-with-global|REINFORCE++: Stabilizing Critic-Free Policy Optimization with Global Advantag...]]
- **62** · [[2025-04-21-arxiv-2504-14870v2-acting-less-is-reasoning-more-teaching-model-to|Acting Less is Reasoning More! Teaching Model to Act Efficiently]]
