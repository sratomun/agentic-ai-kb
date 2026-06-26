---
type: entity
entity_type: method
tags: [agents, method]
created: 2026-06-21
updated: 2026-06-22
---

# EAPO (Efficient Agentic Policy Optimization)

*An Agentic-RL framework teaching agents when not to act — tool-call restraint via tool-free trajectories and difficulty-aware reward shaping.*

## What it is
EAPO injects tool-free trajectories into RL training and applies difficulty-aware reward shaping to penalize unnecessary tool calls. It cuts tool invocations 18–25% vs GRPO without accuracy loss, while improving overall accuracy.

## Why it matters
Tool overuse is a real cost and latency problem in production agentic workflows — each unnecessary call adds latency, cost, and failure surface. EAPO shows restraint is learnable at training time rather than requiring post-hoc filtering, a practical lever for high-volume enterprise deployments.

## Relationships
- method in [[agentic-rl]]
- addresses [[tool-use]]
- compares to [[grpo]]

## Cited by
<!-- Auto-maintained by the kg-curator skill: the highest-cited source notes that reference this node. -->
- [[2026-06-01-arxiv-2606-02132v2-eapo-learning-when-not-to-act]]
