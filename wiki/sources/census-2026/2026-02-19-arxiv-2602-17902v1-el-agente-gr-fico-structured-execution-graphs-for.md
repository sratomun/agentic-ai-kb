---
type: source
source_type: arxiv
title: "El Agente Gráfico: Structured Execution Graphs for Scientific Agents"
authors: Jiaru Bai, Abdulrahman Aldossary, Thomas Swanick, Marcel Müller et al.
url: https://arxiv.org/abs/2602.17902v1
date: 2026-02-19
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [science-agents, knowledge-graph, agent-reliability, agent-security, agent-memory, arxiv, auto-ingested]
---

# El Agente Gráfico: Structured Execution Graphs for Scientific Agents

**arXiv:** [2602.17902v1](https://arxiv.org/abs/2602.17902v1) · 2026-02-19 · cs.AI
**Authors:** Jiaru Bai, Abdulrahman Aldossary, Thomas Swanick, Marcel Müller et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models (LLMs) are increasingly used to automate scientific workflows, yet their integration with heterogeneous computational tools remains ad hoc and fragile. Current agentic approaches often rely on unstructured text to manage context and coordinate execution, generating often overwhelming volumes of information that may obscure decision provenance and hinder auditability. In this work, we present El Agente Gráfico, a single-agent framework that embeds LLM-driven decision-making within a type-safe execution environment and dynamic knowledge graphs for external persistence. Central to our approach is a structured abstraction of scientific concepts and an object-graph mapper that represents computational state as typed Python objects, stored either in memory or persisted in an external knowledge graph. This design enables context management through typed symbolic identifiers rather than raw text, thereby ensuring consistency, supporting provenance tracking, and enabling efficient tool orchestration. We evaluate the system by developing an automated benchmarking framework across a suite of university-level quantum chemistry tasks previously evaluated on a multi-agent system, demonstrating that a single agent, when coupled to a reliable execution engine, can robustly perform complex, multi-step, and parallel computations. We further extend this paradigm to two other large classes of applications: conformer ensemble generation and metal-organic framework design, where knowledge graphs serve as both memory and reasoning substrates. Together, these results illustrate how abstraction and type safety can provide a scalable foundation for agentic scientific automation beyond prompt-centric designs.

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.17902v1)
