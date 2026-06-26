---
type: source
source_type: arxiv
title: "Structured Uncertainty guided Clarification for LLM Agents"
authors: Manan Suri, Puneet Mathur, Nedim Lipka et al.
url: https://arxiv.org/abs/2511.08798v2
date: 2025-11-11
depth: abstract
auto: true
score: 15
primary: cs.CL
tags: [intent-understanding, human-agent-interaction, tool-use, arxiv, auto-ingested]
---

# Structured Uncertainty guided Clarification for LLM Agents

**arXiv:** [2511.08798v2](https://arxiv.org/abs/2511.08798v2) · 2025-11-11 · cs.CL
**Authors:** Manan Suri, Puneet Mathur, Nedim Lipka et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived. Part of the intent-understanding corpus (2026-06-23).

## Abstract
LLM agents with tool-calling capabilities often fail when user instructions are ambiguous or incomplete, leading to incorrect invocations and task failures. Existing approaches operate in unstructured language spaces, generating clarifying questions through prompting strategies that lack principled criteria for determining which questions to ask and when to stop. We introduce a principled formulation of structured uncertainty that operates directly over tool parameters and their domains, cleanly separating specification uncertainty (what the user wants) from model uncertainty (what the LLM predicts). Our formulation uses Expected Value of Perfect Information (EVPI) to quantify the disambiguation value of each potential question, balanced against aspect-based cost modeling that prevents redundant questioning. We demonstrate the versatility of this formulation through two applications. First, SAGE-Agent uses structured uncertainty for inference-time question selection, achieving 7-39% higher coverage on ambiguous tasks while reducing clarification questions by 1.5-2.7x compared to strong prompting and uncertainty-based baselines. Second, we show that structured uncertainty provides effective training signals: uncertainty-guided reward modeling boosts When2Call accuracy from 36.5% to 65.2% (3B model) and 36.7% to 62.9% (7B model) through uncertainty-weighted GRPO training, demonstrating more sample-efficient reinforcement learning for tool-calling agents. To enable evaluation, we present ClarifyBench, the first multi-turn dynamic tool-calling disambiguation benchmark. Our results establish structured uncertainty as a principled framework that improves both inference-time interaction efficiency and training-time sample efficiency in tool-augmented agents.

## Graph
- **Concepts:** [[intent-understanding|Intent understanding]] · [[human-agent-interaction|Human-agent interaction]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2511.08798v2)
