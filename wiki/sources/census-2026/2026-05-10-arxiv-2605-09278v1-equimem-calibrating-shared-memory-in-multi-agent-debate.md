---
type: source
source_type: arxiv
title: "EquiMem: Calibrating Shared Memory in Multi-Agent Debate via Game-Theoretic Equilibrium"
authors: Yuqiao Meng, Sakshi Sunil Narvekar, Luoxi Tang, Rupali Rajendra Vaje et al.
url: https://arxiv.org/abs/2605.09278v1
date: 2026-05-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.AI
tags: [knowledge-graph, agent-security, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# EquiMem: Calibrating Shared Memory in Multi-Agent Debate via Game-Theoretic Equilibrium

**arXiv:** [2605.09278v1](https://arxiv.org/abs/2605.09278v1) · 2026-05-10 · cs.AI
**Authors:** Yuqiao Meng, Sakshi Sunil Narvekar, Luoxi Tang, Rupali Rajendra Vaje et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-agent debate (MAD) systems increasingly rely on shared memory to support long-horizon reasoning, but this convenience opens a critical vulnerability: a single corrupted entry can contaminate the downstream memory-augmented reasoning, and debate alone fails to filter such errors. Existing safeguards filter entries via heuristics or LLM-based validation, yet they rely on AI judgments that share the same failure modes and overlook the cross-agent dynamics of MAD. We address this gap by formulating memory updating in MAD as a zero-trust memory game, in which no agent is assumed honest and the game's equilibrium serves as an indicator of optimal memory trust. Guided by this equilibrium, we propose EquiMem, an inference-time calibration mechanism that quantifies each update algorithmically against the shared memory state, using agents' existing retrieval queries and traversal paths as evidence rather than soliciting any LLM judgment. EquiMem instantiates calibration for both embedding- and graph-based memory, and across diverse benchmarks, MAD frameworks, and memory architectures, it consistently outperforms existing safeguards, remains robust under adversarial agents, and incurs negligible inference overhead.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.09278v1)
