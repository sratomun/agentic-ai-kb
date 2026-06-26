---
type: source
source_type: arxiv
title: "Agentic Search in the Wild: Intents and Trajectory Dynamics from 14M+ Real Search Requests"
authors: Jingjie Ning, João Coelho, Yibo Kong et al.
url: https://arxiv.org/abs/2601.17617v3
date: 2026-01-24
depth: abstract
auto: true
score: 10
primary: cs.IR
tags: [intent-understanding, deep-research-agents, arxiv, auto-ingested]
---

# Agentic Search in the Wild: Intents and Trajectory Dynamics from 14M+ Real Search Requests

**arXiv:** [2601.17617v3](https://arxiv.org/abs/2601.17617v3) · 2026-01-24 · cs.IR
**Authors:** Jingjie Ning, João Coelho, Yibo Kong et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived. Part of the intent-understanding corpus (2026-06-23).

## Abstract
LLM-powered search agents are increasingly being used for multi-step information seeking tasks, yet the IR community lacks empirical understanding of how agentic search sessions unfold and how retrieved evidence is reflected in later queries. This paper presents a large-scale log analysis of agentic search based on 14.44M search requests (3.97M sessions) collected from DeepResearchGym, i.e., an open-source search API accessed by external agentic clients. We sessionize the logs, assign session-level intents and step-wise query-reformulation labels using LLM-based annotation, and propose Context-driven Term Adoption Rate (CTAR) to quantify whether newly introduced query terms are lexically traceable to previously retrieved evidence. Our analyses reveal distinctive behavioral patterns. First, over 90\% of multi-turn sessions contain at most ten steps, and 89\% of inter-step intervals fall under one minute. Second, behavior varies by intent. Fact-seeking sessions exhibit high repetition that increases over time, while sessions requiring reasoning sustain broader exploration. Third, query reformulations are often traceable to retrieved evidence across steps. On average, 54\% of newly introduced query terms appear in the accumulated evidence context, with additional traceability to earlier steps beyond the most recent retrieval. These findings provide candidate signals for repetition-aware stopping, intent-adaptive retrieval budgeting, and explicit cross-step context tracking. We released the anonymized logs, making them available at a public HuggingFace~\chref{https://huggingface.co/datasets/cx-cmu/deepresearchgym-agentic-search-logs}{repository}.

## Graph
- **Concepts:** [[intent-understanding|Intent understanding]] · [[deep-research-agents|Deep research agents]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.17617v3)
