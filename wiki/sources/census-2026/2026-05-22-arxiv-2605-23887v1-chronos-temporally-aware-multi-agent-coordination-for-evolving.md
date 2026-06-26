---
type: source
source_type: arxiv
title: "CHRONOS: Temporally-Aware Multi-Agent Coordination for Evolving Data Marketplaces"
authors: Joydeep Chandra
url: https://arxiv.org/abs/2605.23887v1
date: 2026-05-22
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.DB
tags: [agent-economies, knowledge-graph, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# CHRONOS: Temporally-Aware Multi-Agent Coordination for Evolving Data Marketplaces

**arXiv:** [2605.23887v1](https://arxiv.org/abs/2605.23887v1) · 2026-05-22 · cs.DB
**Authors:** Joydeep Chandra

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Temporal knowledge-graph data marketplaces face three coupled failures in static designs: stale hybrid index shortcuts reduce recall as edges evolve, stationary Shapley pricing misattributes value after distribution shifts, and uncoordinated agents over-consume a shared differential-privacy budget. We present CHRONOS, a three-layer architecture providing a unified treatment of these challenges with explicit public and private separation. Layer one applies neural-ODE temporal decay to shortcut edges, providing a per-query expected recall-loss bound of Big-O of Pq lambda delta t, with a monotone-envelope guarantee reducing bound looseness to 1.8 to 3.2 times observed loss. Layer two conditions Shapley valuation on detected changepoints and provides finite-sample error guarantees under noise. Layer three uses EXP3-IX to achieve Big-O of the square root of T log T regret while enforcing epsilon and delta differential privacy via moments accounting. CHRONOS releases a privatized affinity matrix per epoch using the Gaussian mechanism; all retrieval and ranking are post-processing, incurring no extra privacy cost. We provide multi-epoch settlement, scalability analysis for 500 sellers, and comparisons against accelerated baselines. Across four benchmarks, CHRONOS shows 0.937 recall at ten, 2.74 queries per second, 161 ms latency, and total epsilon of 4.25 at delta of 10 to the power of negative 6 under zCDP composition. These results indicate a competitive operating point. A limitation is that at this privacy level, released valuations remain noise-dominated; utility derives primarily from public index routing and adaptive scheduling driven by low-sensitivity statistics.

## Graph
- **Concepts:** [[agent-economies|Agent economies]] · [[knowledge-graph|Knowledge graphs]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.23887v1)
