---
type: source
source_type: arxiv
title: "IntentRL: Training Proactive User-intent Agents for Open-ended Deep Research via Reinforcement Learning"
authors: Haohao Luo, Zexi Li, Yuexiang Xie et al.
url: https://arxiv.org/abs/2602.03468v1
date: 2026-02-03
depth: abstract
auto: true
score: 9
primary: cs.AI
tags: [intent-understanding, deep-research-agents, agentic-rl, arxiv, auto-ingested]
---

# IntentRL: Training Proactive User-intent Agents for Open-ended Deep Research via Reinforcement Learning

**arXiv:** [2602.03468v1](https://arxiv.org/abs/2602.03468v1) · 2026-02-03 · cs.AI
**Authors:** Haohao Luo, Zexi Li, Yuexiang Xie et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived. Part of the intent-understanding corpus (2026-06-23).

## Abstract
Deep Research (DR) agents extend Large Language Models (LLMs) beyond parametric knowledge by autonomously retrieving and synthesizing evidence from large web corpora into long-form reports, enabling a long-horizon agentic paradigm. However, unlike real-time conversational assistants, DR is computationally expensive and time-consuming, creating an autonomy-interaction dilemma: high autonomy on ambiguous user queries often leads to prolonged execution with unsatisfactory outcomes. To address this, we propose IntentRL, a framework that trains proactive agents to clarify latent user intents before starting long-horizon research. To overcome the scarcity of open-ended research data, we introduce a scalable pipeline that expands a few seed samples into high-quality dialogue turns via a shallow-to-deep intent refinement graph. We further adopt a two-stage reinforcement learning (RL) strategy: Stage I applies RL on offline dialogues to efficiently learn general user-interaction behavior, while Stage II uses the trained agent and a user simulator for online rollouts to strengthen adaptation to diverse user feedback. Extensive experiments show that IntentRL significantly improves both intent hit rate and downstream task performance, outperforming the built-in clarify modules of closed-source DR agents and proactive LLM baselines.

## Graph
- **Concepts:** [[intent-understanding|Intent understanding]] · [[deep-research-agents|Deep research agents]] · [[agentic-rl|Agentic RL]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.03468v1)
