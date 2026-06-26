---
type: source
source_type: arxiv
title: "Meta-Agent: From Task Descriptions to Verified Multi-Agent Systems"
authors: Andy Xu, Yu-Wing Tai
url: https://arxiv.org/abs/2605.25233v1
date: 2026-05-24
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [coding-agents, agent-reliability, multi-agent-systems, arxiv, auto-ingested]
---

# Meta-Agent: From Task Descriptions to Verified Multi-Agent Systems

**arXiv:** [2605.25233v1](https://arxiv.org/abs/2605.25233v1) · 2026-05-24 · cs.AI
**Authors:** Andy Xu, Yu-Wing Tai

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
AI agents are increasingly used to solve complex, multi-step tasks, but existing multi-agent frameworks remain brittle as workflows grow in scale and depth. Small errors at intermediate stages can propagate through agent interactions, while insufficient grounding and weak verification mechanisms further limit reliability. We present Meta-Agent, a two-phase framework that automatically constructs and executes specialized multi-agent systems from natural-language task descriptions. In the construction phase, a task planner decomposes a problem into a directed acyclic graph of agent specifications with explicit input/output contracts and verification criteria. A web search module grounds each specification with external evidence, and a code generation module produces system prompts and tool configurations. A construction-time verification stage then validates generated artifacts and triggers targeted regeneration when failures are detected. In the execution phase, a coordinator dispatches subtasks across the agent graph while execution-time verification gates intermediate outputs. We further introduce a three-level error attribution mechanism that distinguishes local, upstream, and structural failures, enabling targeted recovery strategies ranging from localized retries to partial re-execution and re-decomposition. We evaluate Meta-Agent across coding, contextual learning, and open-ended reasoning tasks. Experiments against strong multi-agent baselines and ablation studies demonstrate consistent improvements in task success rate, error recovery, and workflow stability. The results highlight the importance of tightly integrating planning, grounding, and verification for building reliable multi-agent systems.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.25233v1)
