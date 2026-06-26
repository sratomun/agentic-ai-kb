---
type: source
source_type: arxiv
title: "Retrieval as Reasoning: Self-Evolving Agent-Native Retrieval via LLM-Wiki"
authors: Haoliang Ming, Feifei Li, Xiaoqing Wu, Wenhui Que
url: https://arxiv.org/abs/2605.25480v2
date: 2026-05-25
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.CL
tags: [knowledge-graph, self-evolving-agents, agentic-rag, tool-use, arxiv, auto-ingested]
---

# Retrieval as Reasoning: Self-Evolving Agent-Native Retrieval via LLM-Wiki

**arXiv:** [2605.25480v2](https://arxiv.org/abs/2605.25480v2) · 2026-05-25 · cs.CL
**Authors:** Haoliang Ming, Feifei Li, Xiaoqing Wu, Wenhui Que

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM agents require retrieval to behave less like one-shot context fetching and more like reasoning: searching, reading, traversing, and deciding when evidence is sufficient. Yet current Retrieval-Augmented Generation (RAG) systems organize external knowledge as flat chunks retrieved by embedding similarity, exposing a retrieval-as-lookup interface ill-suited to iterative reasoning agents. We propose LLM-Wiki, an agent-native retrieval system that operationalizes the Retrieval-as-Reasoning paradigm by treating external knowledge as a compilable, composable, and self-evolving structure rather than a static retrieval index. LLM-Wiki compiles documents into structured Wiki pages with bidirectional links, exposes search, read, and link-following operations through standard tool-calling interfaces, and introduces an Error Book for persistent structural and semantic self-correction. LLM-Wiki achieves state-of-the-art results on HotpotQA, MuSiQue, and 2WikiMultiHopQA, outperforming HippoRAG 2, LightRAG, and GraphRAG by 2.0-8.1 F1 points. On AuthTrace, LLM-Wiki achieves the best overall accuracy, with especially strong gains on multi-document structured queries, confirming that compilation-based retrieval generalizes beyond chain-style multi-hop reasoning.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rag|Agentic RAG]] · [[tool-use|Tool use]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.25480v2)
