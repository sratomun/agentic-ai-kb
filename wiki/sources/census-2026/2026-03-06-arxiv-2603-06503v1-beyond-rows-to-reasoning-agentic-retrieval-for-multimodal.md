---
type: source
source_type: arxiv
title: "Beyond Rows to Reasoning: Agentic Retrieval for Multimodal Spreadsheet Understanding and Editing"
authors: Anmol Gulati, Sahil Sen, Waqar Sarguroh, Kevin Paul
url: https://arxiv.org/abs/2603.06503v1
date: 2026-03-06
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.CL
tags: [agent-reliability, agentic-rag, tool-use, agent-evaluation, governance-gap, arxiv, auto-ingested]
---

# Beyond Rows to Reasoning: Agentic Retrieval for Multimodal Spreadsheet Understanding and Editing

**arXiv:** [2603.06503v1](https://arxiv.org/abs/2603.06503v1) · 2026-03-06 · cs.CL
**Authors:** Anmol Gulati, Sahil Sen, Waqar Sarguroh, Kevin Paul

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in multimodal Retrieval-Augmented Generation (RAG) enable Large Language Models (LLMs) to analyze enterprise spreadsheet workbooks containing millions of cells, cross-sheet dependencies, and embedded visual artifacts. However, state-of-the-art approaches exclude critical context through single-pass retrieval, lose data resolution through compression, and exceed LLM context windows through naive full-context injection, preventing reliable multi-step reasoning over complex enterprise workbooks. We introduce Beyond Rows to Reasoning (BRTR), a multimodal agentic framework for spreadsheet understanding that replaces single-pass retrieval with an iterative tool-calling loop, supporting end-to-end Excel workflows from complex analysis to structured editing. Supported by over 200 hours of expert human evaluation, BRTR achieves state-of-the-art performance across three frontier spreadsheet understanding benchmarks, surpassing prior methods by 25 percentage points on FRTR-Bench, 7 points on SpreadsheetLLM, and 32 points on FINCH. We evaluate five multimodal embedding models, identifying NVIDIA NeMo Retriever 1B as the top performer for mixed tabular and visual data, and vary nine LLMs. Ablation experiments confirm that the planner, retrieval, and iterative reasoning each contribute substantially, and cost analysis shows GPT-5.2 achieves the best efficiency-accuracy trade-off. Throughout all evaluations, BRTR maintains full auditability through explicit tool-call traces.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rag|Agentic RAG]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]]
- **Entities:** [[gpt-5]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.06503v1)
