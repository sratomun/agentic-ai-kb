---
type: source
source_type: arxiv
title: "MOSAIC: Modular Orchestration for Structured Agentic Intelligence and Composition"
authors: Yifan Bao, Xinyu Xi, Xinyu Liu, Wen Ge et al.
url: https://arxiv.org/abs/2606.00708v1
date: 2026-05-30
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [clinical-agents, coding-agents, finance-agents, agent-reliability, agentic-rl, arxiv, auto-ingested]
---

# MOSAIC: Modular Orchestration for Structured Agentic Intelligence and Composition

**arXiv:** [2606.00708v1](https://arxiv.org/abs/2606.00708v1) · 2026-05-30 · cs.AI
**Authors:** Yifan Bao, Xinyu Xi, Xinyu Liu, Wen Ge et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Automated data science is a structured model-selection problem. A solution must choose data transformations, feature representations, architecture, training procedure, evaluation protocol, and refinement strategy for a task. AutoML systems automate parts of this process, but typically search within predefined pipeline, model, and hyperparameter spaces. LLM-based agents offer greater flexibility through retrieval, code generation, and execution feedback, yet their modelling decisions are often unstructured, difficult to verify, and hard to reuse. We introduce \textsc{MOSAIC} (Modular Orchestration for Structured Agentic Intelligence and Composition), a structured agentic framework for memory-grounded model selection and workflow construction. Given a task and dataset, \textsc{MOSAIC} builds a semantic task profile, retrieves prior cases and source-code modules, and constructs a blueprint: an intermediate representation specifying selected modelling components, composition, interface constraints, and execution requirements. This blueprint turns model selection into a staged, context-grounded search and grounds LLM-based code generation in retrieved evidence rather than unconstrained synthesis. Candidate models are validated by execution and refined using diagnostic feedback, training traces, task metrics, and a failure-aware reinforcement learning policy. We instantiate \textsc{MOSAIC} on financial time-series forecasting and generation, where models must satisfy predictive accuracy, distributional fidelity, execution reliability, and downstream financial criteria such as risk and tail behaviour. Experiments against AutoML and agentic baselines show that \textsc{MOSAIC} improves task performance, execution success, and decision traceability, demonstrating the value of treating automated data science as structured, reusable, and execution-grounded model selection.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[coding-agents|Coding agents]] · [[finance-agents|Finance agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.00708v1)
