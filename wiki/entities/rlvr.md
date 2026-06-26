---
type: entity
entity_type: method
tags: [agents, method]
created: 2026-06-22
updated: 2026-06-22
---

# RLVR

*RL with Verifiable Rewards — the dominant agentic RL paradigm of 2025–26, training on checkable correctness signals.*

## What it is
RLVR (RL with Verifiable Rewards) replaces the learned reward model of RLHF with a deterministic correctness check — the answer is either right or wrong — making reward hacking structurally harder and training more stable. It is the recipe behind DeepSeek R1, GRPO, and most 2025–26 reasoning-model training.

## Why it matters
RLVR is the key insight unlocking reliable agent training at scale: by grounding rewards in verifiable outcomes (math, code, tool calls), training avoids the proxy-gaming that plagued RLHF. Any team training task-specific agents should understand RLVR as the current best practice.

## Relationships
- core of [[agentic-rl]]
- powers [[self-evolving-agents]]
- compare [[rlhf]]
- part of [[post-training]]; replaces [[reward-modeling]] with verifiable rewards
