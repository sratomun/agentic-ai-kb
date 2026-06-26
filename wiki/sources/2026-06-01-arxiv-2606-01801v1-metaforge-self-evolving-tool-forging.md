---
type: source
source_type: arxiv
title: "MetaForge: A Self-Evolving Multimodal Agent that Retrieves, Adapts, and Forges Tools On Demand"
authors: Shouang Wei, Houcheng Min, Xinpeng Dong, Xin Lin et al.
url: https://arxiv.org/abs/2606.01801v1
date: 2026-06-01
ingested: 2026-06-21
depth: full-text
tags: [self-evolving-agents, agent-skills, tool-use, arxiv]
---

# MetaForge: A Self-Evolving Multimodal Agent that Retrieves, Adapts, and Forges Tools On Demand

**Why it matters:** Multimodal agent that learns when to call tools and forges new ones on demand — a judge→retrieve→adapt→forge→recycle loop with an explicit invocation-cost penalty. The 'forge + recycle' move is the notable bit.

## Takeaways
- MetaForge factorizes behavior into Decide / Retrieve / Adapt / Forge, recycling forged skills back into the tool library for reuse.
- Unified orchestration policy chooses among answering directly, reusing tools, or forging new ones; jointly RL-optimizes invocation necessity, retrieval, execution, and forged-skill reusability with a cost penalty for redundant calls.
- Beats 16 baselines across 12 benchmarks — a paradigm shift from static tool inventories to on-demand self-evolution.

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agent-skills|Agent skills]] · [[tool-use|Tool use]]
- **Raw:** `raw/arxiv/2606.01801v1.md` · `raw/arxiv/2606.01801v1.fulltext.md`
