---
type: source
source_type: arxiv
title: "TRACER: Trajectory Risk Aggregation for Critical Episodes in Agentic Reasoning"
authors: Sina Tayebati, Divake Kumar, Nastaran Darabi, Davide Ettori et al.
url: https://arxiv.org/abs/2602.11409v1
date: 2026-02-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# TRACER: Trajectory Risk Aggregation for Critical Episodes in Agentic Reasoning

**arXiv:** [2602.11409v1](https://arxiv.org/abs/2602.11409v1) · 2026-02-11 · cs.AI
**Authors:** Sina Tayebati, Divake Kumar, Nastaran Darabi, Davide Ettori et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Estimating uncertainty for AI agents in real-world multi-turn tool-using interaction with humans is difficult because failures are often triggered by sparse critical episodes (e.g., looping, incoherent tool use, or user-agent miscoordination) even when local generation appears confident. Existing uncertainty proxies focus on single-shot text generation and therefore miss these trajectory-level breakdown signals. We introduce TRACER, a trajectory-level uncertainty metric for dual-control Tool-Agent-User interaction. TRACER combines content-aware surprisal with situational-awareness signals, semantic and lexical repetition, and tool-grounded coherence gaps, and aggregates them using a tail-focused risk functional with a MAX-composite step risk to surface decisive anomalies. We evaluate TRACER on $τ^2$-bench by predicting task failure and selective task execution. To this end, TRACER improves AUROC by up to 37.1% and AUARC by up to 55% over baselines, enabling earlier and more accurate detection of uncertainty in complex conversational tool-use settings. Our code and benchmark are available at https://github.com/sinatayebati/agent-tracer.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.11409v1)
