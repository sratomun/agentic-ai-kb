---
type: source
source_type: arxiv
title: "When Does Memory Help Multi-Trajectory Inference for Tool-Use LLM Agents?"
authors: Xinzhe Li, Yaguang Tao
url: https://arxiv.org/abs/2605.28224v1
date: 2026-05-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 14
primary: cs.AI
tags: [knowledge-graph, agent-memory, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# When Does Memory Help Multi-Trajectory Inference for Tool-Use LLM Agents?

**arXiv:** [2605.28224v1](https://arxiv.org/abs/2605.28224v1) · 2026-05-27 · cs.AI
**Authors:** Xinzhe Li, Yaguang Tao

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-trajectory inference for tool-use LLM agents - generating multiple reasoning attempts and selecting among them - benefits from transferring knowledge across attempts so that later ones avoid the pitfalls of earlier ones. Existing cross-trajectory memory methods (trajectory-level reflection, atomic fact extraction, raw observation injection) are each evaluated under a single inference strategy on a single task, making it unclear whether reported gains reflect properties of the memory abstraction or of the inference method. We propose a unified framework that decomposes memory along two axes -- the scope of transfer (within an expansion vs. across trajectories) and the abstraction of the transferred content -- and evaluate four methods under three inference strategies (best-of-N, beam search, MCTS) on four tool-use benchmarks spanning SQL, knowledge-graph, and CLI environments, in a verifier-free setting that matches the deployment regime of practical agents. The experiment matrix identifies the inference method as a confound: the same memory method produces statistically distinct results under different inference strategies on the same examples. Reflection reaches significance only under MCTS (not under best-of-N); within-expansion injection (conditioning each candidate on prior siblings' outcomes) helps only diversity-starved beam search; and atomic fact extraction is accuracy-neutral but shortens trajectories by 19-26% on tasks with reusable environmental structure.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.28224v1)
