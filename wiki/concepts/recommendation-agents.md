---
type: concept
tags: [agents, recommendation, personalization]
created: 2026-06-21
updated: 2026-06-22
census_count: 278
kind: domain
---

# Recommendation & personalization agents

*LLM agents applied to recommender systems — conversational recommendation, preference reasoning, agentic user simulation, and personalization.*

## What it is
Agents that sit on top of (or replace parts of) recommender systems: holding a dialogue to elicit preferences, reasoning over user history, and — increasingly — *simulating* users to generate evaluation signal. The largest application cluster surfaced when the census widened into cs.IR.

## Why it matters
A big, commercially-loaded vertical that was almost invisible under the old cs.AI/CL/LG scope — a concrete example of why the [[2026-06-22-okf-adoption-assessment|category widening]] mattered. Two things to watch: agentic *personalization* (the agent as a persistent preference model) and user-simulation as a cheap eval substrate.

## What the evidence shows
**2025 foundations.** Tellingly, one of the most-cited agentic results here is a **security** one: **CheatAgent** shows an LLM agent can attack an LLM-empowered recommender system, using prompt tuning to iteratively craft perturbations from victim feedback (→ [[2025-04-13-arxiv-2504-13192v2-cheatagent-attacking-llm-empowered-recommender-systems-via-llm]]). That the frontier result is an attack is itself a signal: agentic recommenders inherit the agentic *attack surface* ([[agent-security]]).
- _Honest note: deep-ingested coverage is thin relative to the ~278-paper census cluster — most of this vertical sits in the browsable layer, and agentic-specific (vs classical-ML) RecSys work is still early._

## Includes (sub-themes folded here)
Folds in: **personalization & user-simulation** agents (~153 papers) and conversational recommendation.

## Relationships
- uses [[agent-memory]], [[tool-use]], [[agentic-rag]]
- inherits risk from [[agent-security]]
- a form of [[agentic-ai]]
- on-device personalization: [[on-device-agents]]

## Key 2025 papers (citation-ranked)
- **56** · [[2025-04-13-arxiv-2504-13192v2-cheatagent-attacking-llm-empowered-recommender-systems-via-llm|CheatAgent: Attacking LLM-Empowered Recommender Systems via LLM Agent]]
