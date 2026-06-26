---
type: entity
entity_type: benchmark
tags: [agents, benchmark]
created: 2026-06-21
updated: 2026-06-22
---

# MCP-TDP Security Benchmark

*A 32-scenario sandbox benchmark for Tool Description Poisoning attacks on MCP agents — leading models show near-100% attack success in high-risk scenarios.*

## What it is
A high-fidelity benchmark of 32 real-world test cases across 6 risk categories, purpose-built to measure how susceptible MCP-connected agents are to [[tool-description-poisoning|Tool Description Poisoning]] attacks. Scenarios use real-world-grounded attack payloads embedded in tool descriptions.

## Why it matters
Near-100% attack success against leading models in high-risk scenarios means this isn't a theoretical risk — any enterprise deploying MCP-connected agents is exposed today, with no reliable prompt-based defense available.

## Relationships
- evaluates [[agent-security]]
- targets [[mcp]]
- measures [[tool-description-poisoning]]

## Cited by
<!-- Auto-maintained by the kg-curator skill: the highest-cited source notes that reference this node. -->
- [[2026-05-22-arxiv-2605-24069v1-mcp-poisoning-tool-description-attacks]]
