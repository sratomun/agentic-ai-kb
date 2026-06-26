---
type: source
source_type: arxiv
title: "DRBENCHER: Can Your Agent Identify the Entity, Retrieve Its Properties and Do the Math?"
authors: Young-Suk Lee, Ramon Fernandez Astudillo, Radu Florian
url: https://arxiv.org/abs/2604.09251v2
date: 2026-04-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 7
primary: cs.AI
tags: [science-agents, finance-agents, knowledge-graph, agent-security, agent-evaluation, arxiv, auto-ingested]
---

# DRBENCHER: Can Your Agent Identify the Entity, Retrieve Its Properties and Do the Math?

**arXiv:** [2604.09251v2](https://arxiv.org/abs/2604.09251v2) · 2026-04-10 · cs.AI
**Authors:** Young-Suk Lee, Ramon Fernandez Astudillo, Radu Florian

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Deep research agents increasingly interleave web browsing with multi-step computation, yet existing benchmarks evaluate these capabilities in isolation, creating a blind spot in assessing real-world performance. We introduce DRBENCHER, a synthetic benchmark generator for questions that require both browsing and computation. It enforces four criteria: verifiability (gold answers are computed by executing parameterized code over knowledge-graph values), complexity (multi-hop entity identification, property retrieval, and domain-specific computation), difficulty (a two-stage verification cascade filters out questions solvable by the generating model), and diversity (a greedy max-min embedding filter maximizes coverage). These criteria are realized via a unified answer-first pipeline spanning five domains: biochemistry, financial, geophysical, security, and history. Human evaluation shows 76% validity (84% excluding stale data), with 35% of errors due to outdated knowledge-graph entries, highlighting an inherent limitation of systems that reason over evolving data. Automatic evaluation shows that the strongest frontier model achieves only 20% answer accuracy. Compared to manually constructed benchmarks (BrowseComp+, MATH-500, GPQA), DRBENCHER achieves the highest semantic diversity.

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[finance-agents|Finance agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-security|Agent security]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.09251v2)
