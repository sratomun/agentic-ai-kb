---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "FOCAL: Filtered On-device Continuous Activity Logging for Efficient Personal Desktop Summarization"
authors: Haoran Yin et al.
url: https://arxiv.org/abs/2604.19541v1
date: 2026-04-21
score: 5
primary: cs.MA
tags: [arxiv, auto-ingested, small-language-models, agent-memory, reasoning-models, multi-agent-systems]
---

# FOCAL: Filtered On-device Continuous Activity Logging for Efficient Personal Desktop Summarization

**arXiv:** [2604.19541v1](https://arxiv.org/abs/2604.19541v1) · 2026-04-21 · cs.MA
**Authors:** Haoran Yin et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Desktop interaction streams provide a continuous, privacy-sensitive record of interleaved user tasks. Transforming these streams into task-organized personal logs on-device faces two main challenges: exhaustive Vision-Language Model (VLM) processing strains local resources, and global stream processing causes cross-task context pollution. We present FOCAL (Filtered On-device Continuous Activity Logging), a privacy-first multi-agent system utilizing a unified filter-plan-log architecture. It cascades a lightweight Filter Agent for noise suppression, a text-only Brain Agent for task attribution, a Record Agent for selective visual reasoning, and a task-isolated Memory Agent for context-coherent summarization. Experiments on DesktopBench (comprising 2,572 screenshots across 420 complex sessions) show FOCAL reduces total token consumption by 60.4% and VLM call count by 72.3% versus a baseline, while boosting Key Information Recall (KIR) from 0.38 to 0.61. Crucially, under $A{\to}B{\to}A$ task interruptions, FOCAL maintains Task Acc 0.81 and KIR 0.80, whereas the baseline collapses to Task Acc 0.03. FOCAL pioneers the efficient, on-device summarization of instruction-free desktop streams into multi-perspective personal logs.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[agent-memory]] · [[reasoning-models]] · [[multi-agent-systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.19541v1)
