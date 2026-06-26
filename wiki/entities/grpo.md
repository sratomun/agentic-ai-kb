---
type: entity
entity_type: method
tags: [method, agents, reinforcement-learning, training, credit-assignment]
created: 2026-06-21
updated: 2026-06-22
---
# GRPO

*Group Relative Policy Optimization — the RL algorithm at the core of the DeepSeek R1 recipe and most 2025–26 agentic RL training.*

## What it is
GRPO (Group Relative Policy Optimization) is an RL algorithm that computes advantages relative to a group of sampled responses rather than a baseline value function, eliminating the need for a separate critic model. It is the algorithm in the DeepSeek R1 training recipe.

## Why it matters
GRPO made high-quality reasoning-model training accessible without a separate reward model or critic — dramatically lowering the cost of RL fine-tuning. Any team building task-specific agents via RL is likely using GRPO or a variant.

## Relationships
- used by [[2026-06-18-arxiv-2606-20002v1-long-lifecycle-agents-cross-domain]]
- relates to [[agent-memory]]
- part of [[post-training]]; optimizes a [[reward-modeling|reward model]]

## Cited by (2025 deep notes)
- **280** · [[2025-04-16-arxiv-2504-13958v1-toolrl-reward-is-all-tool-learning-needs|ToolRL: Reward is All Tool Learning Needs]]
- **268** · [[2025-05-16-arxiv-2505-10978v3-group-in-group-policy-optimization-for-llm-agent|Group-in-Group Policy Optimization for LLM Agent Training]]
- **218** · [[2025-04-14-arxiv-2504-10458v4-gui-r1-a-generalist-r1-style-vision-language|GUI-R1 : A Generalist R1-Style Vision-Language Action Model For GUI Agents]]
- **127** · [[2025-08-27-arxiv-2508-19828v5-memory-r1-enhancing-large-language-model-agents-to|Memory-R1: Enhancing Large Language Model Agents to Manage and Utilize Memori...]]
- **122** · [[2025-03-27-arxiv-2503-21620v5-ui-r1-enhancing-efficient-action-prediction-of-gui|UI-R1: Enhancing Efficient Action Prediction of GUI Agents by Reinforcement L...]]
- **112** · [[2025-04-12-arxiv-2504-09037v4-a-survey-of-frontiers-in-llm-reasoning-inference|A Survey of Frontiers in LLM Reasoning: Inference Scaling, Learning to Reason...]]
- **77** · [[2025-09-16-arxiv-2509-13313v3-resum-unlocking-long-horizon-search-intelligence-via-context|ReSum: Unlocking Long-Horizon Search Intelligence via Context Summarization]]
- **68** · [[2025-01-04-arxiv-2501-03262v9-reinforce-stabilizing-critic-free-policy-optimization-with-global|REINFORCE++: Stabilizing Critic-Free Policy Optimization with Global Advantag...]]
