---
type: source
source_type: arxiv
title: "FundaPod: A Multi-Persona Agent Pod Platform with Knowledge Graph Memory for AI-Assisted Fundamental Investment Research"
authors: Di Zhu, Lei Nico Zheng, Zihan Chen
url: https://arxiv.org/abs/2605.27864v4
date: 2026-05-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 3
primary: cs.AI
tags: [finance-agents, knowledge-graph, agent-skills, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# FundaPod: A Multi-Persona Agent Pod Platform with Knowledge Graph Memory for AI-Assisted Fundamental Investment Research

**arXiv:** [2605.27864v4](https://arxiv.org/abs/2605.27864v4) · 2026-05-27 · cs.AI
**Authors:** Di Zhu, Lei Nico Zheng, Zihan Chen

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models (LLMs) are increasingly applied in finance, yet most existing work emphasizes trading signals or financial NLP tasks centered on prediction. Institutional fundamental research, by contrast, requires human analysts or AI agents to gather evidence, identify business drivers, compare competing viewpoints, and generate investment memos. Its broader goal is not merely to predict outcomes, but to produce investment plans that are transparent, reusable, and verifiable, while contributing to the cumulative development of investment knowledge. We present FundaPod, a multi-persona agent platform for AI-assisted fundamental investment research. We argue that fundamental research is a human-centric decision-support task that is qualitatively distinct from trading-signal generation, and is therefore better served by an independence-preserving architecture. In FundaPod, AI agents with different personas, such as value investors or macro strategists, conduct research independently under a shared provenance contract. Their disagreements are then surfaced post hoc for adjudication by the human portfolio manager (PM) through a knowledge-graph memory system. This paper contributes five design principles for human-AI hybrid systems supporting fundamental research, grounded in design-science practice and theories of cognitive isolation and human-machine coordination. It also describes four architectural mechanisms: a persona distillation pipeline that turns public investor materials into deployable agents; a declarative skill registry that lets the planner derive typed task graphs; a grounded evidence model that links memo claims to verifiable sources; and a knowledge-graph "second brain" that connects tickers, memos, analysts, and themes. We demonstrate the architecture through a complete case study and a persona-based memo comparison.

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.27864v4)
