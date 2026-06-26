---
type: source
source_type: arxiv
title: "Characterization of Multi-Model Agentic AI Systems on General Tasks via Trace-Driven Simulation"
authors: Donghwan Kim, Prakhar Singh, Younghoon Min, Jongryool Kim et al.
url: https://arxiv.org/abs/2606.01725v1
date: 2026-06-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Characterization of Multi-Model Agentic AI Systems on General Tasks via Trace-Driven Simulation

**arXiv:** [2606.01725v1](https://arxiv.org/abs/2606.01725v1) · 2026-06-01 · cs.AI
**Authors:** Donghwan Kim, Prakhar Singh, Younghoon Min, Jongryool Kim et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic AI completes tasks through iterative planning, tool use, and reasoning based on observed outcomes. Despite its popularity, its system-level behavior remains poorly understood, particularly for complex datasets and agent architectures-owing to highly non-deterministic execution, prohibitive evaluation costs, and limited visibility into proprietary models. This paper presents GAIATrace, the first token-level trace dataset of two state-of-the-art agentic systems (MiroThinker and OWL) running GAIA, a benchmark composed of a heterogeneous mix of general-purpose tasks. Unlike prior trace datasets, GAIATrace captures full reasoning tokens, task-level structures, and activities of every major participating LLMs, enabling in-depth systems research. Complementing the dataset, we present Vidur-Agent, a trace-driven simulator that can replay GAIATrace to perform reproducible, low-cost system evaluation across diverse simulated environments. Using both artifacts, we characterize how modern agentic systems handle general tasks and how various system design choices shape their behavior, yielding several unique findings.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gaia-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.01725v1)
