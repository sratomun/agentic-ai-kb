---
type: source
source_type: arxiv
title: "Text2Model: Modeling Copilots for Text-to-Model Translation"
authors: Serdar Kadioglu, Karthik Uppuluri, Akash Singirikonda
url: https://arxiv.org/abs/2604.12955v3
date: 2026-04-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 6
primary: cs.AI
tags: [knowledge-graph, agent-evaluation, arxiv, auto-ingested]
---

# Text2Model: Modeling Copilots for Text-to-Model Translation

**arXiv:** [2604.12955v3](https://arxiv.org/abs/2604.12955v3) · 2026-04-14 · cs.AI
**Authors:** Serdar Kadioglu, Karthik Uppuluri, Akash Singirikonda

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
There is growing interest in leveraging large language models (LLMs) for text-to-model translation and optimization tasks. This paper aims to advance this line of research by introducing \textsc{Text2Model} and \textsc{Text2Zinc}. \textsc{Text2Model} is a suite of copilots based on several LLM strategies with varying complexity, along with an online leaderboard. \textsc{Text2Zinc} is a cross-domain dataset for capturing optimization and satisfaction problems specified in natural language, along with an interactive editor with built-in AI assistant. While there is an emerging literature on using LLMs for translating combinatorial problems into formal models, our work is the first attempt to integrate \textit{both} satisfaction and optimization problems within a \textit{unified architecture} and \textit{dataset}. Moreover, our approach is \textit{solver-agnostic} unlike existing work that focuses on translation to a solver-specific model. To achieve this, we leverage \textsc{MiniZinc}'s solver-and-paradigm-agnostic modeling capabilities to formulate combinatorial problems. We conduct comprehensive experiments to compare execution and solution accuracy across several single- and multi-call strategies, including; zero-shot prompting, chain-of-thought reasoning, intermediate representations via knowledge-graphs, grammar-based syntax encoding, and agentic approaches that decompose the model into sequential sub-tasks. Our copilot strategies are competitive, and in parts improve, recent research in this domain. Our findings indicate that while LLMs are promising they are not yet a push-button technology for combinatorial modeling. We contribute \textsc{Text2Model} copilots and leaderboard, and \textsc{Text2Zinc} and interactive editor to open-source to support closing this performance gap.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.12955v3)
