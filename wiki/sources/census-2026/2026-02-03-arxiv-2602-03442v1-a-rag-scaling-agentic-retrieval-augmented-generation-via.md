---
type: source
source_type: arxiv
title: "A-RAG: Scaling Agentic Retrieval-Augmented Generation via Hierarchical Retrieval Interfaces"
authors: Mingxuan Du, Benfeng Xu, Chiwei Zhu, Shaohan Wang et al.
url: https://arxiv.org/abs/2602.03442v1
date: 2026-02-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.CL
tags: [agentic-rag, agent-memory, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# A-RAG: Scaling Agentic Retrieval-Augmented Generation via Hierarchical Retrieval Interfaces

**arXiv:** [2602.03442v1](https://arxiv.org/abs/2602.03442v1) · 2026-02-03 · cs.CL
**Authors:** Mingxuan Du, Benfeng Xu, Chiwei Zhu, Shaohan Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Frontier language models have demonstrated strong reasoning and long-horizon tool-use capabilities. However, existing RAG systems fail to leverage these capabilities. They still rely on two paradigms: (1) designing an algorithm that retrieves passages in a single shot and concatenates them into the model's input, or (2) predefining a workflow and prompting the model to execute it step-by-step. Neither paradigm allows the model to participate in retrieval decisions, preventing efficient scaling with model improvements. In this paper, we introduce A-RAG, an Agentic RAG framework that exposes hierarchical retrieval interfaces directly to the model. A-RAG provides three retrieval tools: keyword search, semantic search, and chunk read, enabling the agent to adaptively search and retrieve information across multiple granularities. Experiments on multiple open-domain QA benchmarks show that A-RAG consistently outperforms existing approaches with comparable or lower retrieved tokens, demonstrating that A-RAG effectively leverages model capabilities and dynamically adapts to different RAG tasks. We further systematically study how A-RAG scales with model size and test-time compute. We will release our code and evaluation suite to facilitate future research. Code and evaluation suite are available at https://github.com/Ayanami0730/arag.

## Graph
- **Concepts:** [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.03442v1)
