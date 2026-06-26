---
type: entity
entity_type: method
tags: [agents, method]
created: 2026-06-21
updated: 2026-06-22
---

# DART (Disentangled Action–Reasoning Tuning)

*An Agentic-RL training method that decouples reasoning and tool-use into separate LoRA modules to prevent gradient interference.*

## What it is
DART separates parameter updates for reasoning and tool-use into independent low-rank adaptation modules after demonstrating that joint optimization induces misaligned gradients. It outperforms joint-optimization baselines and approaches a 2-agent upper bound (specialized reasoning agent + specialized tool-use agent).

## Why it matters
DART identifies a fundamental training conflict in tool-using agents — the same parameters can't be optimized for both cognitive tasks simultaneously. Any team fine-tuning agents for enterprise tool-calling workflows should account for this interference before assuming joint training will converge well.

## Relationships
- method in [[agentic-rl]]
- addresses [[tool-use]]

## Cited by
<!-- Auto-maintained by the kg-curator skill: the highest-cited source notes that reference this node. -->
- [[2026-02-01-arxiv-2602-00994v2-reasoning-vs-tooluse-interference-dart]]
