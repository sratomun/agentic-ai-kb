---
type: source
source_type: arxiv
title: "Human-Inspired Memory Architecture for LLM Agents"
authors: Doga Kerestecioglu, Alexei Robsky, Clemens Vasters, Anshul Sharma et al.
url: https://arxiv.org/abs/2605.08538v1
date: 2026-05-08
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.AI
tags: [knowledge-graph, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# Human-Inspired Memory Architecture for LLM Agents

**arXiv:** [2605.08538v1](https://arxiv.org/abs/2605.08538v1) · 2026-05-08 · cs.AI
**Authors:** Doga Kerestecioglu, Alexei Robsky, Clemens Vasters, Anshul Sharma et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Current LLM agents lack principled mechanisms for managing persistent memory across long interaction horizons. We present a biologically-grounded memory architecture comprising six cognitive mechanisms: (1) sleep-phase consolidation, (2) interference-based forgetting, (3) engram maturation, (4) reconsolidation upon retrieval, (5) entity knowledge graphs, and (6) hybrid multi-cue retrieval. Each mechanism addresses a specific failure mode of naive memory accumulation. We introduce a synthetic calibration methodology that derives all pipeline thresholds without benchmark data exposure, eliminating a common source of evaluation leakage. We evaluate on two benchmarks. First, a VSCode issue-tracking dataset (13K issues, 120K events) where deduplication-based consolidation achieves 97.2% retention precision with 58% store reduction (+21.8 pp over baseline). Second, the LongMemEval personal-chat benchmark where we conduct the first streaming M-tier evaluation (475 sessions, ~540K unique turns). At a 200K-token context budget, our pipeline matches raw retrieval accuracy (70.1% vs. 71.2%, overlapping 95% CI) while exposing a tunable accuracy/store-size operating curve. At S-tier scale (50 sessions), dedup-based consolidation yields a +13.3 pp improvement in preference recall.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.08538v1)
