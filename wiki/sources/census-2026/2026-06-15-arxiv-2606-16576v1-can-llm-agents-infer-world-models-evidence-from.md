---
type: source
source_type: arxiv
title: "Can LLM Agents Infer World Models? Evidence from Agentic Automata Learning"
authors: Reef Menaged, Gili Lior, Shauli Ravfogel, Roee Aharoni et al.
url: https://arxiv.org/abs/2606.16576v1
date: 2026-06-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.CL
tags: [science-agents, tool-use, arxiv, auto-ingested]
---

# Can LLM Agents Infer World Models? Evidence from Agentic Automata Learning

**arXiv:** [2606.16576v1](https://arxiv.org/abs/2606.16576v1) · 2026-06-15 · cs.CL
**Authors:** Reef Menaged, Gili Lior, Shauli Ravfogel, Roee Aharoni et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We propose agentic automata learning to evaluate the extent to which tool-calling LLM agents can uncover hidden environments through interaction. In our setup, an agent should uncover a hidden deterministic finite automaton (DFA) by interacting with an oracle through (1) membership queries ("Does this string belong to the target language?") and (2) equivalence queries ("Is this the target DFA?"). This yields a scalable testbed with controlled task complexity, measurable interaction efficiency, and strong baselines (classic automata-learning algorithms). Evaluating state-of-the-art LLMs, we find that performance drops sharply as DFA size increases. Reasoning models are markedly stronger than non-reasoning models, yet trajectory analyses reveal recurring failures in query planning, evidence integration, and hypothesis construction. Overall, our results show that current LLM agents can sometimes perform non-trivial interactive discovery, but remain far less robust and efficient than classic algorithms for the task.

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.16576v1)
