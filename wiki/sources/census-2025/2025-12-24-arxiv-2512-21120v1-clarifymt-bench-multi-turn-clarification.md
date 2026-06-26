---
type: source
source_type: arxiv
title: "ClarifyMT-Bench: Benchmarking and Improving Multi-Turn Clarification for Conversational Large Language Models"
authors: Sichun Luo, Yi Huang, Mukai Li et al.
url: https://arxiv.org/abs/2512.21120v1
date: 2025-12-24
depth: abstract
auto: true
score: 8
primary: cs.CL
tags: [intent-understanding, agent-evaluation, human-agent-interaction, arxiv, auto-ingested]
---

# ClarifyMT-Bench: Benchmarking and Improving Multi-Turn Clarification for Conversational Large Language Models

**arXiv:** [2512.21120v1](https://arxiv.org/abs/2512.21120v1) · 2025-12-24 · cs.CL
**Authors:** Sichun Luo, Yi Huang, Mukai Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived. Part of the intent-understanding corpus (2026-06-23).

## Abstract
Large language models (LLMs) are increasingly deployed as conversational assistants in open-domain, multi-turn settings, where users often provide incomplete or ambiguous information. However, existing LLM-focused clarification benchmarks primarily assume single-turn interactions or cooperative users, limiting their ability to evaluate clarification behavior in realistic settings. We introduce \textbf{ClarifyMT-Bench}, a benchmark for multi-turn clarification grounded in a five-dimensional ambiguity taxonomy and a set of six behaviorally diverse simulated user personas. Through a hybrid LLM-human pipeline, we construct 6,120 multi-turn dialogues capturing diverse ambiguity sources and interaction patterns. Evaluating ten representative LLMs uncovers a consistent under-clarification bias: LLMs tend to answer prematurely, and performance degrades as dialogue depth increases. To mitigate this, we propose \textbf{ClarifyAgent}, an agentic approach that decomposes clarification into perception, forecasting, tracking, and planning, substantially improving robustness across ambiguity conditions. ClarifyMT-Bench establishes a reproducible foundation for studying when LLMs should ask, when they should answer, and how to navigate ambiguity in real-world human-LLM interactions.

## Graph
- **Concepts:** [[intent-understanding|Intent understanding]] · [[agent-evaluation|Agent evaluation]] · [[human-agent-interaction|Human-agent interaction]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2512.21120v1)
