---
type: source
source_type: arxiv
title: "State-Grounded Multi-Agent Synthetic Data Generation for Tool-Augmented LLMs"
authors: Rahul Khedar, Eshita, Sneha Teja Sree Reddy Thondapu, Mayank Malhotra et al.
url: https://arxiv.org/abs/2606.16307v1
date: 2026-06-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# State-Grounded Multi-Agent Synthetic Data Generation for Tool-Augmented LLMs

**arXiv:** [2606.16307v1](https://arxiv.org/abs/2606.16307v1) · 2026-06-15 · cs.AI
**Authors:** Rahul Khedar, Eshita, Sneha Teja Sree Reddy Thondapu, Mayank Malhotra et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Training tool-augmented LLM agents requires large corpora of multi-turn, tool-grounded conversational data that is expensive to annotate, privacy-constrained in production settings, and largely absent from public datasets. We present StateGen, a synthetic data generation platform that produces scored, reasoning-trace-rich training conversations by orchestrating a four-role LLM loop: a persona-conditioned user simulator, an agent under test, a state-grounded tool simulator, and a multi-axis LLM judge. The key architectural contribution is an authoritative state manager that maintains a structured world-state object across turns, enforcing a backend-is-truth invariant that eliminates the dominant class of tool-call hallucinations by construction. StateGen extends naturally to hierarchical multi-agent settings by declaring sub-agents as tools, all sharing a single state object. We report results on 64,698 evaluated conversations across three production corpora: tool-call hallucination scores reach 9.66/10, the system supports persona-driven variation via a 23-dimensional trait vector, and a cleanly separated train and golden evaluation set split confirms the data is not memorization bait (per-criterion gap analysis). Comparison with eight external systems shows that no single publicly available platform combines multi-turn generation, state-grounded tool simulation, hierarchical multi-agent support, and built-in judge scoring.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.16307v1)
