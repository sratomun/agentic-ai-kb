---
type: source
source_type: arxiv
title: "Complete Cyclic Subtask Graphs for Tool-Using LLM Agents: Flexibility, Cost, and Bottlenecks in Multi-Agent Workflows"
authors: Luay Gharzeddine, Samer Saab
url: https://arxiv.org/abs/2604.22820v1
date: 2026-04-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.MA
tags: [finance-agents, agent-reliability, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Complete Cyclic Subtask Graphs for Tool-Using LLM Agents: Flexibility, Cost, and Bottlenecks in Multi-Agent Workflows

**arXiv:** [2604.22820v1](https://arxiv.org/abs/2604.22820v1) · 2026-04-17 · cs.MA
**Authors:** Luay Gharzeddine, Samer Saab

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Long-horizon tool-using tasks sometimes benefit from revisiting earlier subtasks for recovery and exploration, but added multi-agent workflow flexibility can also introduce coordination overhead and substantial inference cost. We study complete cyclic subtask graphs, a deliberately maximally flexible multi-agent architecture in which executable subtask nodes are fully connected and a unified state-analysis-and-routing agent selects transitions using natural-language criteria. This makes unrestricted revisitation explicit and directly analyzable at the subtask level. We evaluate task-specific (Spec-Cyc) and benchmark-generic (Gen-Cyc) graphs on TextCraft, ALFWorld, and Finance-Agent, with ablations over planner/executor/router strength, tool exposure (generalist vs specialized), $n$-shot successful trajectory summaries, and fault-injected random subtask perturbations. The benchmarks expose three distinct regimes. ALFWorld highlights a setting where explicit revisitation supports recovery and exploration; TextCraft, a largely prerequisite-chain domain, often favors the efficiency of simpler forward execution; and Finance-Agent remains bottlenecked by retrieval, grounding, and evidence synthesis more than by workflow flexibility alone. Shared-win token comparisons further show that the added flexibility can be substantially more expensive than a single ReAct agent. Overall, we use complete cyclic subtask graphs as a maximally flexible experimental lens for measuring when multi-agent revisitation helps, when it mainly adds coordination cost, and when external task bottlenecks dominate.

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[alfworld]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.22820v1)
