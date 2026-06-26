---
type: source
source_type: arxiv
title: "DomAgent: Leveraging Knowledge Graphs and Case-Based Reasoning for Domain-Specific Code Generation"
authors: Shuai Wang, Dhasarathy Parthasarathy, Robert Feldt, Yinan Yu
url: https://arxiv.org/abs/2603.21430v2
date: 2026-03-22
ingested: 2026-06-21
depth: abstract
auto: true
score: 10
primary: cs.AI
tags: [coding-agents, knowledge-graph, agent-evaluation, arxiv, auto-ingested]
---

# DomAgent: Leveraging Knowledge Graphs and Case-Based Reasoning for Domain-Specific Code Generation

**arXiv:** [2603.21430v2](https://arxiv.org/abs/2603.21430v2) · 2026-03-22 · cs.AI
**Authors:** Shuai Wang, Dhasarathy Parthasarathy, Robert Feldt, Yinan Yu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models (LLMs) have shown impressive capabilities in code generation. However, because most LLMs are trained on public domain corpora, directly applying them to real-world software development often yields low success rates, as these scenarios frequently require domain-specific knowledge. In particular, domain-specific tasks usually demand highly specialized solutions, which are often underrepresented or entirely absent in the training data of generic LLMs. To address this challenge, we propose DomAgent, an autonomous coding agent that bridges this gap by enabling LLMs to generate domain-adapted code through structured reasoning and targeted retrieval. A core component of DomAgent is DomRetriever, a novel retrieval module that emulates how humans learn domain-specific knowledge, by combining conceptual understanding with experiential examples. It dynamically integrates top-down knowledge-graph reasoning with bottom-up case-based reasoning, enabling iterative retrieval and synthesis of structured knowledge and representative cases to ensure contextual relevance and broad task coverage. DomRetriever can operate as part of DomAgent or independently with any LLM for flexible domain adaptation. We evaluate DomAgent on an open benchmark dataset in the data science domain (DS-1000) and further apply it to real-world truck software development tasks. Experimental results show that DomAgent significantly enhances domain-specific code generation, enabling small open-source models to close much of the performance gap with large proprietary LLMs in complex, real-world applications. The code is available at: https://github.com/Wangshuaiia/DomAgent.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.21430v2)
