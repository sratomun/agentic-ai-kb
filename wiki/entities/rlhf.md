---
type: entity
entity_type: method
tags: [agents, method]
created: 2026-06-22
updated: 2026-06-22
---

# RLHF

*Reinforcement Learning from Human Feedback — the foundational alignment method that preceded verifiable-reward agentic RL.*

## What it is
RLHF trains a reward model from human preference data (A is better than B) and optimizes an LLM policy against that reward using RL (typically PPO). It is the alignment method used for GPT-3.5/4, early Claude models, and most production LLMs through 2024.

## Why it matters
RLHF established that human preference signals can align LLMs — but also introduced reward hacking and scalability limits that RLVR and Constitutional AI are designed to fix. Understanding RLHF is understanding the design space that current agent training techniques are evolving away from.

## Relationships
- alignment method feeding [[agentic-rl]]
- compare [[rlvr]], [[grpo]], [[dpo]]
- part of [[post-training]]; uses [[reward-modeling]]
