---
type: source
source_type: arxiv
title: "MemFlow: Intent-Driven Memory Orchestration for Small Language Model Agents"
authors: Jiayi Chen, Yingcong Li, Guiling Wang
url: https://arxiv.org/abs/2605.03312v1
date: 2026-05-05
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.MA
tags: [agent-reliability, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# MemFlow: Intent-Driven Memory Orchestration for Small Language Model Agents

**arXiv:** [2605.03312v1](https://arxiv.org/abs/2605.03312v1) · 2026-05-05 · cs.MA
**Authors:** Jiayi Chen, Yingcong Li, Guiling Wang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Modern language agents must operate over long-horizon, multi-turn histories, yet deploying such agents with Small Language Models (SLMs) remains fundamentally difficult. Full-context prompting causes context overflow, flat retrieval exposes the model to noisy evidence, and open-ended agentic loops are unreliable under limited reasoning capacity. We argue that a substantial portion of SLM memory failure arises from mismatched memory operations: different query types demand categorically different retrieval strategies, evidence transformations, and context budgets that SLMs cannot reliably self-orchestrate through open-ended reasoning. We introduce MemFlow, a training-free memory orchestration framework that externalizes memory planning from the SLM. A Router Agent classifies each query by intent and dispatches it to the Memory Agent, which executes one of three specialized tiers (Profile Lookup, Targeted Retrieval, or Deep Reasoning) and assembles the resulting evidence under a dynamic, tier-aware token budget. An Answer Agent then generates a response from this compact context, and a Validator Agent optionally retries with a heavier memory tier when the response is not supported by the provided evidence. This route-then-compile design avoids tool-selection hallucination and reasoning loops while keeping the answer context compact. Evaluated on a frozen Qwen3-1.7B backbone across long-horizon memory benchmarks - LongMemEval, LoCoMo, and LongBench - MemFlow improves accuracy by nearly 2x over full-context SLM baselines. These results suggest that structured intent routing and deterministic evidence preparation can make limited-capacity models substantially more effective in resource-constrained long-horizon agents.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.03312v1)
