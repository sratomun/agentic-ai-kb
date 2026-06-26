---
type: source
source_type: arxiv
title: "From Experience to Skill: Multi-Agent Generative Engine Optimization via Reusable Strategy Learning"
authors: Beining Wu, Fuyou Mao, Jiong Lin, Cheng Yang et al.
url: https://arxiv.org/abs/2604.19516v1
date: 2026-04-21
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-protocols, agent-skills, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# From Experience to Skill: Multi-Agent Generative Engine Optimization via Reusable Strategy Learning

**arXiv:** [2604.19516v1](https://arxiv.org/abs/2604.19516v1) · 2026-04-21 · cs.AI
**Authors:** Beining Wu, Fuyou Mao, Jiong Lin, Cheng Yang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Generative engines (GEs) are reshaping information access by replacing ranked links with citation-grounded answers, yet current Generative Engine Optimization (GEO) methods optimize each instance in isolation, unable to accumulate or transfer effective strategies across tasks and engines. We reframe GEO as a strategy learning problem and propose MAGEO, a multi-agent framework in which coordinated planning, editing, and fidelity-aware evaluation serve as the execution layer, while validated editing patterns are progressively distilled into reusable, engine-specific optimization skills. To enable controlled assessment, we introduce a Twin Branch Evaluation Protocol for causal attribution of content edits and DSV-CF, a dual-axis metric that unifies semantic visibility with attribution accuracy. We further release MSME-GEO-Bench, a multi-scenario, multi-engine benchmark grounded in real-world queries. Experiments on three mainstream engines show that MAGEO substantially outperforms heuristic baselines in both visibility and citation fidelity, with ablations confirming that engine-specific preference modeling and strategy reuse are central to these gains, suggesting a scalable learning-driven paradigm for trustworthy GEO. Code is available at https://github.com/Wu-beining/MAGEO

## Graph
- **Concepts:** [[agent-protocols|Agent protocols]] · [[agent-skills|Agent skills]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.19516v1)
