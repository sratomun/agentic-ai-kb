---
type: source
source_type: arxiv
title: "EngiAI: A Multi-Agent Framework and Benchmark Suite for LLM-Driven Engineering Design"
authors: Gioele Molinari, Florian Felten, Soheyl Massoudi, Mark Fuge
url: https://arxiv.org/abs/2605.19743v2
date: 2026-05-19
ingested: 2026-06-21
depth: abstract
auto: true
score: 22
primary: cs.AI
tags: [agentic-rag, agent-memory, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# EngiAI: A Multi-Agent Framework and Benchmark Suite for LLM-Driven Engineering Design

**arXiv:** [2605.19743v2](https://arxiv.org/abs/2605.19743v2) · 2026-05-19 · cs.AI
**Authors:** Gioele Molinari, Florian Felten, Soheyl Massoudi, Mark Fuge

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Model (LLM) agents are increasingly applied to engineering design tasks, yet existing evaluation frameworks do not adequately address multi-agent systems that combine simulation, retrieval, and manufacturing preparation. We introduce a benchmark suite with three evaluation dimensions: (1) a workflow benchmark with seven prompt styles targeting distinct cognitive demands-including direct tool use, semantic disambiguation, conditional branching, and working-memory tasks; (2) a Retrieval-Augmented Generation (RAG) benchmark with gated scoring isolating retrieval contributions to parameter selection; and (3) an High Performance Computing (HPC) benchmark evaluating end-to-end ML training orchestration on a SLURM cluster. Alongside the benchmark we present EngiAI, a Multi-Agent System (MAS) reference implementation built on LangGraph that operationalizes the benchmark by coordinating seven specialized agents through a supervisor architecture, unifying topology optimization, document retrieval, HPC job orchestration, and 3D printer control. Across four LLM backends and two EngiBench problems, proprietary models achieve 96-97% average task completion on Beams2D, while open-source 4B-parameter models reach 55-78%, with clear generational improvement. Conditional branching proves most challenging, with task completion dropping to 20-53% for the conditional style on Photonics2D. RAG gating confirms near-perfect retrieval-augmented scores (about 1.0) versus near-zero without retrieval, validating the evaluation design. On HPC orchestration, one model completes all pipeline steps in 100% of runs while another drops to 50%, revealing that multi-step instruction following degrades over long-running workflows.

## Graph
- **Concepts:** [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[langgraph]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.19743v2)
