---
type: source
source_type: arxiv
title: "Table-as-Search: Formulate Long-Horizon Agentic Information Seeking as Table Completion"
authors: Tian Lan, Felix Henry, Bin Zhu, Qianghuai Jia et al.
url: https://arxiv.org/abs/2602.06724v1
date: 2026-02-06
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.CL
tags: [agent-reliability, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Table-as-Search: Formulate Long-Horizon Agentic Information Seeking as Table Completion

**arXiv:** [2602.06724v1](https://arxiv.org/abs/2602.06724v1) · 2026-02-06 · cs.CL
**Authors:** Tian Lan, Felix Henry, Bin Zhu, Qianghuai Jia et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Current Information Seeking (InfoSeeking) agents struggle to maintain focus and coherence during long-horizon exploration, as tracking search states, including planning procedure and massive search results, within one plain-text context is inherently fragile. To address this, we introduce \textbf{Table-as-Search (TaS)}, a structured planning framework that reformulates the InfoSeeking task as a Table Completion task. TaS maps each query into a structured table schema maintained in an external database, where rows represent search candidates and columns denote constraints or required information. This table precisely manages the search states: filled cells strictly record the history and search results, while empty cells serve as an explicit search plan. Crucially, TaS unifies three distinct InfoSeeking tasks: Deep Search, Wide Search, and the challenging DeepWide Search. Extensive experiments demonstrate that TaS significantly outperforms numerous state-of-the-art baselines across three kinds of benchmarks, including multi-agent framework and commercial systems. Furthermore, our analysis validates the TaS's superior robustness in long-horizon InfoSeeking, alongside its efficiency, scalability and flexibility. Code and datasets are publicly released at https://github.com/AIDC-AI/Marco-Search-Agent.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.06724v1)
