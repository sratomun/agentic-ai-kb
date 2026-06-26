---
type: source
source_type: arxiv
title: "Code Broker: A Multi-Agent System for Automated Code Quality Assessment"
authors: Samer Attrah
url: https://arxiv.org/abs/2604.23088v2
date: 2026-04-25
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.SE
tags: [recommendation-agents, coding-agents, agent-reliability, agent-security, agent-memory, arxiv, auto-ingested]
---

# Code Broker: A Multi-Agent System for Automated Code Quality Assessment

**arXiv:** [2604.23088v2](https://arxiv.org/abs/2604.23088v2) · 2026-04-25 · cs.SE
**Authors:** Samer Attrah

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We present Code Broker, a multi agent system built on Google s Agent Development Kit ADK that analyses Python source code from individual files, local directory trees, or remote GitHub repositories and generates structured, actionable quality assessment reports. The system realises a hierarchical five agent architecture in which a root orchestrator coordinates a sequential pipeline agent that, in turn, dispatches three specialised agents concurrently a Correctness Assessor, a Style Assessor, and a Description Generator before synthesising their findings through an Improvement Recommender. Reports quantify four quality dimensions correctness, security, style, and maintainability on a normalised scale and are rendered in both Markdown and HTML for integration into diverse developer workflows. Code Broker fuses LLM based semantic reasoning with deterministic static analysis signals from Pylint, employs asynchronous execution with exponential backoff retry logic to improve robustness under transient API failures, and explores lightweight session memory for retaining and querying prior assessment context across runs. We frame this paper as a technical report on system design, prompt engineering, and tool orchestration, and present a preliminary qualitative evaluation on representative Python codebases of varying scale. The results indicate that parallel specialised agents produce readable, developer oriented feedback that complements traditional linting, while also foregrounding current limitations in evaluation depth, security tooling, large repository handling, and the exclusive reliance on in memory persistence. All code and reproducibility materials are publicly available: https://github.com/Samir-atra/agents_intensive_dev.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[coding-agents|Coding agents]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.23088v2)
