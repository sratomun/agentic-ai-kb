---
type: source
source_type: arxiv
title: "OmniRAG-Agent: Agentic Omnimodal Reasoning for Low-Resource Long Audio-Video Question Answering"
authors: Yifan Zhu, Xinyu Mu, Tao Feng, Zhonghong Ou et al.
url: https://arxiv.org/abs/2602.03707v4
date: 2026-02-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CL
tags: [agentic-rl, agentic-rag, agent-memory, tool-use, arxiv, auto-ingested]
---

# OmniRAG-Agent: Agentic Omnimodal Reasoning for Low-Resource Long Audio-Video Question Answering

**arXiv:** [2602.03707v4](https://arxiv.org/abs/2602.03707v4) · 2026-02-03 · cs.CL
**Authors:** Yifan Zhu, Xinyu Mu, Tao Feng, Zhonghong Ou et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Long-horizon omnimodal question answering answers questions by reasoning over text, images, audio, and video. Despite recent progress on OmniLLMs, low-resource long audio-video QA still suffers from costly dense encoding, weak fine-grained retrieval, limited proactive planning, and no clear end-to-end optimization. To address these issues, we propose OmniRAG-Agent, an agentic omnimodal QA method for budgeted long audio-video reasoning. It builds an image-audio retrieval-augmented generation module that lets an OmniLLM fetch short, relevant frames and audio snippets from external banks. Moreover, it uses an agent loop that plans, calls tools across turns, and merges retrieved evidence to answer complex queries. Furthermore, we apply group relative policy optimization to jointly improve tool use and answer quality over time. Experiments on OmniVideoBench, WorldSense, and Daily-Omni show that OmniRAG-Agent consistently outperforms prior methods under low-resource settings and achieves strong results, with ablations validating each component.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.03707v4)
