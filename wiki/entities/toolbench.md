---
type: entity
entity_type: benchmark
tags: [agents, benchmark]
created: 2026-06-21
updated: 2026-06-22
census_count: 27
---

# ToolBench

*A large-scale tool-use benchmark built on massive real-world APIs — used for training and evaluating agents that must select, call, and chain real APIs at scale.*

## What it is
ToolBench provides a massive set of real API tools (16,000+ from RapidAPI) paired with instruction-following tasks requiring multi-step tool chains. Appears in ~27 of the 2026 H1 census papers as a standard for training and evaluating API-calling agents at scale.

## Why it matters
API-calling at scale is the bread-and-butter of enterprise agents — ToolBench performance reveals whether an agent generalizes tool selection to long-tail or poorly-documented APIs, which is the norm in real enterprise system landscapes.

## Relationships
- evaluates [[tool-use]]
