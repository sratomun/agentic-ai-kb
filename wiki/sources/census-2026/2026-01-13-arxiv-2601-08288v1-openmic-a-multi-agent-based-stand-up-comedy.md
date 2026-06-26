---
type: source
source_type: arxiv
title: "OpenMic: A Multi-Agent-Based Stand-Up Comedy Generation System"
authors: Yuyang Wu, Hanzhong Cao, Jianhao Chen, Yufei Li
url: https://arxiv.org/abs/2601.08288v1
date: 2026-01-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [agentic-rag, multi-agent-systems, arxiv, auto-ingested]
---

# OpenMic: A Multi-Agent-Based Stand-Up Comedy Generation System

**arXiv:** [2601.08288v1](https://arxiv.org/abs/2601.08288v1) · 2026-01-13 · cs.AI
**Authors:** Yuyang Wu, Hanzhong Cao, Jianhao Chen, Yufei Li

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Chinese stand-up comedy generation goes beyond plain text generation, requiring culturally grounded humor, precise timing, stage-performance cues, and implicit multi-step reasoning. Moreover, commonly used Chinese humor datasets are often better suited for humor understanding and evaluation than for long-form stand-up generation, making direct supervision misaligned with the target task. To address these challenges, we present OpenMic, an end-to-end multi-agent system built on AutoGen that transforms a user-provided life topic into a 3-5 minute Chinese stand-up performance and further produces a narrated comedy video. OpenMic orchestrates multiple specialized agents in a multi-round iterative loop-planning to jointly optimize humor, timing, and performability. To mitigate the dataset-task mismatch, we augment generation with retrieval-augmented generation (RAG) for material grounding and idea expansion, and we fine-tune a dedicated JokeWriter to better internalize stand-up-specific setup-punchline structures and long-range callbacks.

## Graph
- **Concepts:** [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[autogen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.08288v1)
