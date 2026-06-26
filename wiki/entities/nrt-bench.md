---
type: entity
entity_type: benchmark
tags: [benchmark, agents, security, red-teaming, safety-critical, evaluation]
created: 2026-06-21
updated: 2026-06-22
---

# NRT-Bench

*A multi-turn red-teaming benchmark for LLM agents in safety-critical control rooms — harm is an objective signal (a critical safety function lost), not LLM-judged text.*

## What it is
NRT-Bench instantiates a simulated nuclear power plant control room with a five-role operator team (each backed by a configurable LLM) governing six Critical Safety Functions (CSFs). Adversaries inject messages over four ingress channels in bounded multi-turn sessions with per-turn feedback for adaptive escalation; a run terminates the moment any CSF is lost. Across four frontier models, adaptive attacks lost a CSF in 8.7–12.1% of sessions, with failures nearly disjoint across models.

## Why it matters
The objective harm signal (CSF lost = run over) removes LLM-as-judge subjectivity — making NRT-Bench the highest-fidelity published safety benchmark for high-stakes agentic deployments. The near-disjoint failure patterns across models suggest ensembles could significantly reduce risk.

## Relationships
- introduced by [[2026-06-18-arxiv-2606-20408v1-llm-agent-safety-red-teaming]]
- evaluates [[agent-security]]

## Cited by
<!-- Auto-maintained by the kg-curator skill: the highest-cited source notes that reference this node. -->
- [[2026-06-18-arxiv-2606-20408v1-llm-agent-safety-red-teaming]]
