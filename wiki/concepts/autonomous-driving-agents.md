---
type: concept
tags: [agents, autonomous-driving, embodied]
created: 2026-06-21
updated: 2026-06-22
census_count: 131
kind: domain
---

# Autonomous-driving agents

*LLM/VLM agents for driving — perception-to-planning, decision agents, and generative traffic/scenario simulation.*

## What it is
A specialization of [[embodied-agents]] for the driving domain: language/vision models that reason about scenes and make driving decisions, plus the generative [[world-models]] used to manufacture and stress-test scenarios safely.

## Why it matters
A high-stakes embodied vertical with the heaviest [[agent-reliability]] and safety demands of any on the radar — and a useful pressure-test of agent decision-making where errors are physical. It shares the planning + [[multi-agent-systems]] stack with the rest of the field, so its safety-critical techniques (especially simulation-for-evaluation) flow back outward.

## What the evidence shows
**2025 foundations.** The most-cited line of work is **simulation, not the driver itself**: GAIA-2 is a domain-specialized generative world model that produces controllable, multi-view driving scenarios — reducing dependence on costly real-world data and giving safe, repeatable evaluation environments (→ [[2025-03-26-arxiv-2503-20523v1-gaia-2-a-controllable-multi-view-generative-world]]; the cross-cutting hub is [[world-models]]).
- _Honest note: thin deep coverage relative to its census size; the browsable census layer has the long tail of driving-decision and traffic-scenario papers._

## Relationships
- specialization of [[embodied-agents]]
- planning via [[world-models]]
- uses [[multi-agent-systems]], [[agent-reliability]]
- a form of [[agentic-ai]]

## Key 2025 papers (citation-ranked)
- **143** · [[2025-03-26-arxiv-2503-20523v1-gaia-2-a-controllable-multi-view-generative-world|GAIA-2: A Controllable Multi-View Generative World Model for Autonomous Driving]]
