---
type: source
source_type: arxiv
title: "RoboPhD: Self-Improving Text-to-SQL Through Autonomous Agent Evolution"
authors: Andrew Borthwick, Stephen Ash
url: https://arxiv.org/abs/2601.01126v2
date: 2026-01-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.CL
tags: [data-query-agents, self-evolving-agents, multi-agent-systems, arxiv, auto-ingested]
---

# RoboPhD: Self-Improving Text-to-SQL Through Autonomous Agent Evolution

**arXiv:** [2601.01126v2](https://arxiv.org/abs/2601.01126v2) · 2026-01-03 · cs.CL
**Authors:** Andrew Borthwick, Stephen Ash

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We present RoboPhD, a system where AI agents autonomously conduct research to improve Text-to-SQL performance. RoboPhD implements a closed-loop evolution cycle with two coordinated components: a SQL Generation agent composed of a database analysis script and SQL generation instructions, and an Evolution agent that designs new versions based on performance feedback. Central to the framework is an ELO-based selection mechanism enabling survival-of-the-fittest dynamics while handling non-transitivity in performance. Starting from a naive 70-line baseline, RoboPhD evolves agents through iterative cross-pollination, discovering effective techniques without any external guidance on the Text-to-SQL domain. Our best agent, evolved to 1500 lines over 18 iterations, autonomously discovered strategies such as size-adaptive database analysis that adjusts depth based on schema complexity and SQL generation patterns for column selection, evidence interpretation, and aggregation. Evolution provides the largest gains on cheaper models: while we improve by 2.3 points over a strong Claude Opus 4.5 naive baseline, we show an improvement of 8.9 points over the weaker Claude Haiku model. This enables 'skip a tier' deployment: evolved Haiku exceeds naive Sonnet accuracy, and evolved Sonnet exceeds naive Opus, both at lower cost. The full system achieves 73.67% accuracy on the BIRD test set, demonstrating that AI can autonomously build a strong agentic system with only a trivial human-provided starting point.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[self-evolving-agents|Self-evolving agents]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[bird-benchmark]] · [[claude]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.01126v2)
