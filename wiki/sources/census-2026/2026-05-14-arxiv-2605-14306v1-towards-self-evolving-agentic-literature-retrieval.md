---
type: source
source_type: arxiv
title: "Towards Self-Evolving Agentic Literature Retrieval"
authors: Yuwen Du, Tian Jin, Jing Kang, Xianghe Pang et al.
url: https://arxiv.org/abs/2605.14306v1
date: 2026-05-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 14
primary: cs.IR
tags: [recommendation-agents, agent-reliability, self-evolving-agents, agent-evaluation, arxiv, auto-ingested]
---

# Towards Self-Evolving Agentic Literature Retrieval

**arXiv:** [2605.14306v1](https://arxiv.org/abs/2605.14306v1) · 2026-05-14 · cs.IR
**Authors:** Yuwen Du, Tian Jin, Jing Kang, Xianghe Pang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As large language models reshape scientific research, literature retrieval faces a twofold challenge: ensuring source authenticity while maintaining a deep comprehension of academic search intents. While reliable, traditional keyword-centric search fails to capture complex research intents. Frontier LLMs can handle complex research intents, but their high cost and tendency to hallucinate remain key limitations. Here we introduce PaSaMaster, a self-evolving agentic literature retrieval system that produces relevance-scored paper rankings with evidence-grounded recommendations through iterative intent analysis, retrieval, and ranking. It is built on three key designs. First, it transforms literature retrieval from a one shot query--document matching problem into a search process that evolves over time, using ranked evidence to reveal gaps, refine intents, and guide follow-up searches. Second, it prevents hallucinated sources by treating retrieval as intent--paper relevance ranking rather than generation. Finally, PaSaMaster improves cost efficiency by separating planning from retrieval: a frontier LLM is used only for intent understanding, while large scale retrieval and relevance scoring are delegated to customized corpora and lightweight models. Evaluated on the PaSaMaster Benchmark across 38 scientific disciplines, our system exposes the severe inaccuracy and incompleteness of traditional keyword retrieval (improving F1-score by 15.6X) and the unreliability of generative LLMs (which exhibit hallucination rates up to 37.79%). Remarkably, PaSaMaster outperforms GPT-5.2 by 30.0% at a mere 1% of the computational cost while ensuring zero source hallucination: https://github.com/sjtu-sai-agents/PaSaMaster

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.14306v1)
