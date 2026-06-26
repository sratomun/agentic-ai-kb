---
type: source
source_type: arxiv
title: "Reinforcement Learning for LLM-based Multi-Agent Systems through Orchestration Traces"
authors: Chenchen Zhang
url: https://arxiv.org/abs/2605.02801v1
date: 2026-05-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.CL
tags: [agentic-rl, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# Reinforcement Learning for LLM-based Multi-Agent Systems through Orchestration Traces

**arXiv:** [2605.02801v1](https://arxiv.org/abs/2605.02801v1) · 2026-05-04 · cs.CL
**Authors:** Chenchen Zhang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As large language model (LLM) agents evolve from isolated tool users into coordinated teams, reinforcement learning (RL) must optimize not only individual actions but also how work is spawned, delegated, communicated, aggregated, and stopped. This paper studies RL for LLM-based multi-agent systems through orchestration traces: temporal interaction graphs whose events include sub-agent spawning, delegation, communication, tool use, return, aggregation, and stopping decisions. Using this lens, we identify three technical axes. First, reward design spans eight families, including orchestration rewards for parallelism speedup, split correctness, and aggregation quality. Second, reward and credit signals attach to eight credit- or signal-bearing units from token to team; explicit counterfactual message-level credit remains especially sparse in our curated pool. Third, orchestration learning decomposes into five sub-decisions: when to spawn, whom to delegate to, how to communicate, how to aggregate, and when to stop. In our curated pool as of May 4, 2026, we found no explicit RL training method for the stopping decision. We connect academic methods to public industrial evidence from Kimi Agent Swarm, OpenAI Codex, and Anthropic Claude Code. The resulting scale gap is a gap between publicly reported deployment envelopes and open academic evaluation regimes, not independent verification of industrial training traces. We release the artifact at https://github.com/xxzcc/awesome-llm-mas-rl, including an 84-entry tagged paper pool, a 32-record exclusion log, scripted corpus statistics, and a minimal JSON schema for replayable orchestration traces.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[claude]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.02801v1)
