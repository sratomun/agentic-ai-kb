---
type: entity
entity_type: method
tags: [agents, method]
created: 2026-06-21
updated: 2026-06-22
---

# RUBAS (Rubric-Based RL for Agent Safety)

*A safety-alignment method applying fine-grained rubric rewards across four agent-behavior dimensions — replacing binary refusal signals with a structured quality signal.*

## What it is
RUBAS assigns granular rubric rewards over whole agent trajectories across four dimensions: tool-use safety, argument safety, response safety, and helpfulness. It replaces the coarse refusal label used in standard safety alignment with multi-dimensional quality scoring, significantly improving fine-grained safety metrics.

## Why it matters
Binary refusal training produces brittle safety behavior — an agent that either acts or refuses, with no gradient on *how well* it refused. RUBAS's multi-dimensional rubric is closer to what enterprise QA actually needs: auditable, nuanced standards for what constitutes a safe agent trajectory.

## Relationships
- method in [[agentic-rl]]
- advances [[agent-security]]

## Cited by
<!-- Auto-maintained by the kg-curator skill: the highest-cited source notes that reference this node. -->
- [[2026-06-02-arxiv-2606-04051v1-rubas-rubric-based-rl-agent-safety]]
