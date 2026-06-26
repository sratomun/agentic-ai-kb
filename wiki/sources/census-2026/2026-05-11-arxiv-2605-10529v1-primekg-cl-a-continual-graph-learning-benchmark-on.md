---
type: source
source_type: arxiv
title: "PrimeKG-CL: A Continual Graph Learning Benchmark on Evolving Biomedical Knowledge Graphs"
authors: Yousef A. Radwan, Yao Li, Qing Qing, Ziqi Xu et al.
url: https://arxiv.org/abs/2605.10529v1
date: 2026-05-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 3
primary: cs.AI
tags: [clinical-agents, knowledge-graph, agentic-rag, agent-evaluation, arxiv, auto-ingested]
---

# PrimeKG-CL: A Continual Graph Learning Benchmark on Evolving Biomedical Knowledge Graphs

**arXiv:** [2605.10529v1](https://arxiv.org/abs/2605.10529v1) · 2026-05-11 · cs.AI
**Authors:** Yousef A. Radwan, Yao Li, Qing Qing, Ziqi Xu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Biomedical knowledge graphs underwrite drug repurposing and clinical decision support, yet the upstream ontologies they depend on update on independent cycles that add millions of edges and deprecate hundreds of thousands more between releases. Yet existing continual graph learning has been studied almost exclusively on synthetic random splits of static, generic KGs, a regime that cannot reproduce the asynchronous, structured evolution real biomedical KGs undergo. To this end, we introduce PrimeKG-CL, a CGL benchmark built from nine authoritative biomedical databases (129K+ nodes, 8.1M+ edges, 10 node types, 30 relation types) with two genuine temporal snapshots (June 2021, July 2023; 5.83M edges added, 889K removed, 7.21M persistent), 10 entity-type-grouped tasks, multimodal node features, and a per-task persistent/added/removed test stratification. On three tasks (biomedical relationship prediction, entity classification, KGQA), we evaluate six CL strategies across four KGE decoders, plus LKGE, an LLM-RAG agent, and CMKL. We find that decoder choice and continual learning strategy interact strongly: no single strategy performs best across all decoders, and mismatched combinations can significantly degrade performance. Moreover, only DistMult exhibits a clear separation between persistent and deprecated knowledge, indicating that standard metrics conflate retention of still-valid facts with failure to forget outdated ones; this effect is absent under RotatE. In addition, multimodal features improve entity-level tasks by up to 60%, and a recent CKGE framework (IncDE) failed to scale to our 5.67M-triple base task across five attempts up to 350GB RAM. Data, pipeline, baselines, and the stratified split are released openly. Dataset:huggingface.co/datasets/yradwan147/PrimeKGCL|Code:github.com/yradwan147/primekg-cl-neurips2026

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.10529v1)
