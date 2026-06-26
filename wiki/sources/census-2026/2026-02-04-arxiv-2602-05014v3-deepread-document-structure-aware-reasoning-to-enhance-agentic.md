---
type: source
source_type: arxiv
title: "DeepRead: Document Structure-Aware Reasoning to Enhance Agentic Search"
authors: Zhanli Li, Huiwen Tian, Lvzhou Luo, Yixuan Cao et al.
url: https://arxiv.org/abs/2602.05014v3
date: 2026-02-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.AI
tags: [embodied-agents, agentic-rag, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# DeepRead: Document Structure-Aware Reasoning to Enhance Agentic Search

**arXiv:** [2602.05014v3](https://arxiv.org/abs/2602.05014v3) · 2026-02-04 · cs.AI
**Authors:** Zhanli Li, Huiwen Tian, Lvzhou Luo, Yixuan Cao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
With the rapid advancement of tool-use capabilities in Large Language Models (LLMs), Retrieval-Augmented Generation (RAG) is shifting from static, one-shot retrieval toward autonomous, multi-turn evidence acquisition. However, existing agentic search frameworks typically treat long documents as flat collections of unstructured chunks, disregarding the native hierarchical organization and sequential logic essential for human comprehension. To bridge this gap, we introduce \textbf{DeepRead}, a structure-aware document reasoning agent designed to operationalize document-native structural priors into actionable reasoning capabilities. Leveraging the structural fidelity of modern OCR, DeepRead constructs a paragraph-level, coordinate-based navigation system and equips the LLM with two synergistic tools: \textsf{Retrieve} for scanning-aware localization, and \textsf{ReadSection} for contiguous, order-preserving reading within specific hierarchical scopes. This design elicits a human-like ``locate-then-read'' reasoning paradigm, effectively mitigating the context fragmentation inherent in traditional retrieval methods. Extensive evaluations across four benchmarks spanning diverse document types demonstrate that DeepRead outperforms Search-o1-style agentic search baselines by an average of 10.3\%. Fine-grained behavioral analysis further confirms that DeepRead autonomously adopts human-aligned reading strategies, validating the critical role of structural awareness in achieving precise document reasoning. Our code is available at https://github.com/Zhanli-Li/DeepRead.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agentic-rag|Agentic RAG]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.05014v3)
