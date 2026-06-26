---
type: source
source_type: arxiv
title: "Faramesh: A Protocol-Agnostic Execution Control Plane for Autonomous Agent Systems"
authors: Amjad Fatmi
url: https://arxiv.org/abs/2601.17744v1
date: 2026-01-25
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-reliability, agent-protocols, multi-agent-systems, governance-gap, arxiv, auto-ingested]
---

# Faramesh: A Protocol-Agnostic Execution Control Plane for Autonomous Agent Systems

**arXiv:** [2601.17744v1](https://arxiv.org/abs/2601.17744v1) · 2026-01-25 · cs.AI
**Authors:** Amjad Fatmi

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Autonomous agent systems increasingly trigger real-world side effects: deploying infrastructure, modifying databases, moving money, and executing workflows. Yet most agent stacks provide no mandatory execution checkpoint where organizations can deterministically permit, deny, or defer an action before it changes reality. This paper introduces Faramesh, a protocol-agnostic execution control plane that enforces execution-time authorization for agent-driven actions via a non-bypassable Action Authorization Boundary (AAB). Faramesh canonicalizes agent intent into a Canonical Action Representation (CAR), evaluates actions deterministically against policy and state, and issues a decision artifact (PERMIT/DEFER/DENY) that executors must validate prior to execution. The system is designed to be framework- and model-agnostic, supports multi-agent and multi-tenant deployments, and remains independent of transport protocols (e.g., MCP). Faramesh further provides decision-centric, append-only provenance logging keyed by canonical action hashes, enabling auditability, verification, and deterministic replay without re-running agent reasoning. We show how these primitives yield enforceable, predictable governance for autonomous execution while avoiding hidden coupling to orchestration layers or observability-only approaches.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]] · [[governance-gap|Governance gap]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.17744v1)
