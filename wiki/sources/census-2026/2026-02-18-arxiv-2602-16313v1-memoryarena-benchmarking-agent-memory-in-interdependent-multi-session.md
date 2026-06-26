---
type: source
source_type: arxiv
title: "MemoryArena: Benchmarking Agent Memory in Interdependent Multi-Session Agentic Tasks"
authors: Zexue He, Yu Wang, Churan Zhi, Yuanzhe Hu et al.
url: https://arxiv.org/abs/2602.16313v1
date: 2026-02-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CL
tags: [computer-use-agents, embodied-agents, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# MemoryArena: Benchmarking Agent Memory in Interdependent Multi-Session Agentic Tasks

**arXiv:** [2602.16313v1](https://arxiv.org/abs/2602.16313v1) · 2026-02-18 · cs.CL
**Authors:** Zexue He, Yu Wang, Churan Zhi, Yuanzhe Hu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Existing evaluations of agents with memory typically assess memorization and action in isolation. One class of benchmarks evaluates memorization by testing recall of past conversations or text but fails to capture how memory is used to guide future decisions. Another class focuses on agents acting in single-session tasks without the need for long-term memory. However, in realistic settings, memorization and action are tightly coupled: agents acquire memory while interacting with the environment, and subsequently rely on that memory to solve future tasks. To capture this setting, we introduce MemoryArena, a unified evaluation gym for benchmarking agent memory in multi-session Memory-Agent-Environment loops. The benchmark consists of human-crafted agentic tasks with explicitly interdependent subtasks, where agents must learn from earlier actions and feedback by distilling experiences into memory, and subsequently use that memory to guide later actions to solve the overall task. MemoryArena supports evaluation across web navigation, preference-constrained planning, progressive information search, and sequential formal reasoning, and reveals that agents with near-saturated performance on existing long-context memory benchmarks like LoCoMo perform poorly in our agentic setting, exposing a gap in current evaluations for agents with memory.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.16313v1)
