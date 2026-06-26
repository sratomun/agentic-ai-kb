---
type: entity
entity_type: framework
tags: [agents, framework, evaluation]
created: 2026-06-22
updated: 2026-06-22
---

# Inspect AI

*Open-source LLM/agent evaluation framework from the UK AI Safety Institute, used by frontier labs to run standardized agent evals.*

## What it is
A Python framework for building and running evaluations of LLMs and agents — datasets, solvers, scorers, and tool-using agent harnesses — created by the UK AI Safety Institute (AISI). It has become a de-facto shared substrate for agent evaluation across several frontier labs and safety orgs.

## Why it matters
It's the concrete tooling under the "evals are the bottleneck" argument — the thing practitioners reach for when they stop hand-rolling measurement. On the radar it's a graph connector between the [[agent-evaluation]] research layer and the practitioner [[hamel-husain]] perspective layer, and a signal that agent-eval infrastructure is consolidating rather than fragmenting.

## Relationships
- tooling for [[agent-evaluation]]; used to validate [[llm-as-judge]] setups
- championed by [[hamel-husain]] → [[2025-06-23-blog-husain-inspect-ai]]
- relates to [[debate-evals-vs-frameworks]]

## Cited by
<!-- Auto-maintained by the kg-curator skill: the highest-cited source notes that reference this node. -->
- [[2025-06-23-blog-husain-inspect-ai]]
