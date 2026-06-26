---
type: source
source_type: arxiv
title: "Toward Scalable Verifiable Reward: Proxy State-Based Evaluation for Multi-turn Tool-Calling LLM Agents"
authors: Yun-Shiuan Chuang, Chaitanya Kulkarni, Alec Chiu, Avinash Thangali et al.
url: https://arxiv.org/abs/2602.16246v3
date: 2026-02-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [agent-reliability, agentic-rl, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Toward Scalable Verifiable Reward: Proxy State-Based Evaluation for Multi-turn Tool-Calling LLM Agents

**arXiv:** [2602.16246v3](https://arxiv.org/abs/2602.16246v3) · 2026-02-18 · cs.AI
**Authors:** Yun-Shiuan Chuang, Chaitanya Kulkarni, Alec Chiu, Avinash Thangali et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Interactive large language model (LLM) agents operating via multi-turn dialogue and multi-step tool calling are increasingly used in production. Benchmarks for these agents must both reliably compare models and yield on-policy training data. Prior agentic benchmarks, such as tau-bench, tau^2-bench, and AppWorld, rely on fully deterministic backends, which are costly to build and iterate. We propose Proxy State-Based Evaluation, an LLM-driven simulation framework that preserves final state-based evaluation without a deterministic database. Specifically, a scenario specifies the user goal, user/system facts, expected final state, and expected agent behavior, and an LLM state tracker infers a structured proxy state from the full interaction trace. LLM judges then verify goal completion and detect tool/user hallucinations against scenario constraints. Empirically, our benchmark produces stable, model-differentiating rankings across model families and inference-time reasoning efforts, and its on-/off-policy rollouts provide supervision that transfers to unseen scenarios. Careful scenario specification yields near-zero simulator hallucination rates, as supported by ablation studies. The framework also supports sensitivity analyses over user personas. Human-LLM judge agreement exceeds 90%, indicating reliable automated evaluation. Overall, proxy state-based evaluation offers a practical, scalable alternative to deterministic agentic benchmarks for industrial LLM agents.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[appworld]] · [[tau-bench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.16246v3)
