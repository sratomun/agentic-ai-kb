---
type: source
source_type: arxiv
title: "DeepRoot: A KG-Coordinated Multi-Agent System for Therapeutic Reasoning over Historical Medical Texts"
authors: Zijian Carl Ma, Sean J. Wang, Sijbren Kramer, Li Erran Li
url: https://arxiv.org/abs/2606.15931v1
date: 2026-06-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.MA
tags: [clinical-agents, science-agents, knowledge-graph, agentic-rag, tool-use, arxiv, auto-ingested]
---

# DeepRoot: A KG-Coordinated Multi-Agent System for Therapeutic Reasoning over Historical Medical Texts

**arXiv:** [2606.15931v1](https://arxiv.org/abs/2606.15931v1) · 2026-06-14 · cs.MA
**Authors:** Zijian Carl Ma, Sean J. Wang, Sijbren Kramer, Li Erran Li

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Historical medical archives and traditional medicines hold immense potential for drug discovery and remain a primary source for current drug development. However, pre-ontological prose and idiosyncratic taxonomies prevent the standardization and medical modernization of the data for use in current biomedical pipelines. Furthermore, no existing LLM agent system, whether tool-calling, retrieval-augmented, or agentic deep-research, can convert such text into verifiable drug-discovery leads at scale. We close this gap with DeepRoot, a multi-agent LLM system that jointly builds and utilizes a verified knowledge graph, showing that grounding and reasoning -- often conflated -- are separable axes the system can compose for therapeutic reasoning. Applied to the Shen Nong Ben Cao Jing, DeepRoot recovers $10$ of $21$ held-out compound-disease treatment pairs at R@$20$ ($47.6\%$ vs $4.8\%$ for a raw corpus LLM and $\sim\!2.4\%$ random) and dominates an LLM-as-judge audit for reasoning quality over baseline LLMs and LLMs with direct tool-call access to the same APIs DeepRoot itself queries. Tool-using LLMs hallucinate evidence on $87\%$ of claims, versus 7-10% for DeepRoot. Graph-only inference hallucinates $0\%$ but ranks lowest on reasoning coherence; DeepRoot KG+LLM is the only condition to win on both axes, pointing toward a route for systematic mining and repurposing of historical medical knowledge.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[science-agents|Science agents]] · [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.15931v1)
