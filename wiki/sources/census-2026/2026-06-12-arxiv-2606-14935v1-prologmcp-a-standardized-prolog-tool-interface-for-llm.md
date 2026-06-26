---
type: source
source_type: arxiv
title: "PrologMCP: A Standardized Prolog Tool Interface for LLM Agents"
authors: Agnieszka Mensfelt, Adarsh Prabhakaran, Adrian Haret, Vince Trencsenyi et al.
url: https://arxiv.org/abs/2606.14935v1
date: 2026-06-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-protocols, arxiv, auto-ingested]
---

# PrologMCP: A Standardized Prolog Tool Interface for LLM Agents

**arXiv:** [2606.14935v1](https://arxiv.org/abs/2606.14935v1) · 2026-06-12 · cs.AI
**Authors:** Agnieszka Mensfelt, Adarsh Prabhakaran, Adrian Haret, Vince Trencsenyi et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Frontier reasoning-tuned language models still fail on deductive tasks at depth, and the cost of improved performance through extended internal reasoning scales poorly. Symbolic delegation offers a complementary route: a language model translates the problem, while a solver performs the inference. However, current autoformalization pipelines for logic programming are typically bespoke integrations tied to particular tasks or agents. We introduce PrologMCP, a task-agnostic, open-source server that exposes Prolog as a stateful tool through the Model Context Protocol (MCP). Its compact tool interface, structured error reporting, and per-session isolation make the translate-run-inspect-repair loop a reusable primitive for MCP-capable agents. We evaluate a formalizer agent enhanced with PrologMCP against standard and reasoning LLMs (Claude Sonnet 4.6, GPT-4.1, and o4-mini) on two subsets of PARARULE-Plus: a general-purpose sample and a more challenging one targeting a specific failure mode of natural-language reasoning. On the general sample, the formalizer matches or exceeds reasoning LLMs (accuracy 1.00 vs.\ 1.00 / 0.998), with the largest gains over standard models (0.762 for GPT-4.1). On the challenging subset, the formalizer remains near-perfect (1.00 / 0.99) while reasoning LLMs drop to 0.95 / 0.94. These results suggest that delegating inference to Prolog via MCP is a robust and inspectable alternative to extended natural-language reasoning.

## Graph
- **Concepts:** [[agent-protocols|Agent protocols]]
- **Entities:** [[mcp]] · [[claude]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.14935v1)
