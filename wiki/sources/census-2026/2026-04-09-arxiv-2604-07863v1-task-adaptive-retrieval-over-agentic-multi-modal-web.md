---
type: source
source_type: arxiv
title: "Task-Adaptive Retrieval over Agentic Multi-Modal Web Histories via Learned Graph Memory"
authors: Saman Forouzandeh, Kamal Berahmand, Mahdi Jalili
url: https://arxiv.org/abs/2604.07863v1
date: 2026-04-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.IR
tags: [knowledge-graph, agent-memory, arxiv, auto-ingested]
---

# Task-Adaptive Retrieval over Agentic Multi-Modal Web Histories via Learned Graph Memory

**arXiv:** [2604.07863v1](https://arxiv.org/abs/2604.07863v1) · 2026-04-09 · cs.IR
**Authors:** Saman Forouzandeh, Kamal Berahmand, Mahdi Jalili

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Retrieving relevant observations from long multi-modal web interaction histories is challenging because relevance depends on the evolving task state, modality (screenshots, HTML text, structured signals), and temporal distance. Prior approaches typically rely on static similarity thresholds or fixed-capacity buffers, which fail to adapt relevance to the current task context. We propose \textbf{ACGM}, a learned graph-memory retriever that constructs \emph{task-adaptive} relevance graphs over agent histories using policy-gradient optimization from downstream task success. ACGM captures heterogeneous temporal dynamics with modality-specific decay (visual decays $4.3\times$ faster than text: $λ_v{=}0.47$ vs.\ $λ_x{=}0.11$) and learns sparse connectivity (3.2 edges/node), enabling efficient $O(\log T)$ retrieval. Across WebShop, VisualWebArena, and Mind2Web, ACGM improves retrieval quality to \textbf{82.7 nDCG@10} (+9.3 over GPT-4o, $p{<}0.001$) and \textbf{89.2\% Precision@10} (+7.7), outperforming 19 strong dense, re-ranking, multi-modal, and graph-based baselines. Code to reproduce our results is available at{\color{blue}\href{https://github.com/S-Forouzandeh/ACGM-Agentic-Web}{Saman Forouzandeh}}.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]]
- **Entities:** [[gpt-5]] · [[webarena]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.07863v1)
