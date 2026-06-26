---
type: source
source_type: arxiv
title: "Paper Circle: An Open-source Multi-agent Research Discovery and Analysis Framework"
authors: Komal Kumar, Aman Chadha, Salman Khan, Fahad Shahbaz Khan et al.
url: https://arxiv.org/abs/2604.06170v1
date: 2026-04-07
ingested: 2026-06-21
depth: abstract
auto: true
score: 15
primary: cs.CL
tags: [knowledge-graph, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Paper Circle: An Open-source Multi-agent Research Discovery and Analysis Framework

**arXiv:** [2604.06170v1](https://arxiv.org/abs/2604.06170v1) · 2026-04-07 · cs.CL
**Authors:** Komal Kumar, Aman Chadha, Salman Khan, Fahad Shahbaz Khan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The rapid growth of scientific literature has made it increasingly difficult for researchers to efficiently discover, evaluate, and synthesize relevant work. Recent advances in multi-agent large language models (LLMs) have demonstrated strong potential for understanding user intent and are being trained to utilize various tools. In this paper, we introduce Paper Circle, a multi-agent research discovery and analysis system designed to reduce the effort required to find, assess, organize, and understand academic literature. The system comprises two complementary pipelines: (1) a Discovery Pipeline that integrates offline and online retrieval from multiple sources, multi-criteria scoring, diversity-aware ranking, and structured outputs; and (2) an Analysis Pipeline that transforms individual papers into structured knowledge graphs with typed nodes such as concepts, methods, experiments, and figures, enabling graph-aware question answering and coverage verification. Both pipelines are implemented within a coder LLM-based multi-agent orchestration framework and produce fully reproducible, synchronized outputs including JSON, CSV, BibTeX, Markdown, and HTML at each agent step. This paper describes the system architecture, agent roles, retrieval and scoring methods, knowledge graph schema, and evaluation interfaces that together form the Paper Circle research workflow. We benchmark Paper Circle on both paper retrieval and paper review generation, reporting hit rate, MRR, and Recall at K. Results show consistent improvements with stronger agent models. We have publicly released the website at https://papercircle.vercel.app/ and the code at https://github.com/MAXNORM8650/papercircle.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.06170v1)
