---
type: entity
entity_type: method
tags: [agents, method]
created: 2026-06-21
updated: 2026-06-22
census_count: 30
---

# DPO

*Direct Preference Optimization — a preference-based alignment method that bypasses an explicit reward model.*

## What it is
DPO optimizes LLMs directly from human preference data without training a separate reward model, treating the policy itself as the implicit reward signal. Appears in ~30 of the 2026 H1 census papers as an alignment baseline in agent post-training pipelines.

## Why it matters
DPO is the lightweight alternative to PPO for teams that want preference alignment without the complexity of a reward model — a relevant tradeoff for enterprise fine-tuning of tool-calling and safety-aligned agents.

## Relationships
- used in [[agentic-rl]]
- compare [[grpo]], [[ppo]]
- part of [[post-training]]; bypasses an explicit [[reward-modeling|reward model]]
