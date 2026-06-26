---
type: source
source_type: arxiv
title: "VineLM: Trie-Based Fine-Grained Control for Agentic Workflows"
authors: Nikos Pagonas, Matthew Lou, Tianyi Peng, Dan Rubenstein et al.
url: https://arxiv.org/abs/2605.23914v1
date: 2026-04-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.DC
tags: [data-query-agents, arxiv, auto-ingested]
---

# VineLM: Trie-Based Fine-Grained Control for Agentic Workflows

**arXiv:** [2605.23914v1](https://arxiv.org/abs/2605.23914v1) · 2026-04-09 · cs.DC
**Authors:** Nikos Pagonas, Matthew Lou, Tianyi Peng, Dan Rubenstein et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic workflows interleave configurable LLM stages with tool stages and often include retries or refinement loops. Existing workflow managers profile full workflow configurations offline and assign each request a static workflow-level plan that binds each configurable LLM stage to a single model, reuses that model across repeated loop iterations, and does not revisit those choices at runtime. We present VineLM, a workflow manager that enables fine-grained control by choosing the model for each stage invocation as execution unfolds under request-level objectives such as maximizing accuracy under cost or latency budgets. VineLM represents feasible executions as an annotated trie of model-choice prefixes and uses checkpointing and cascade profiling to estimate path accuracy, cost, and latency without exhaustively profiling every request on every path. At runtime, VineLM re-roots the trie after each stage invocation and replans over the remaining subtrie using the realized execution prefix and remaining latency budget. On NL2SQL and math reasoning workflows, VineLM improves the cost-latency-accuracy frontier over coarse workflow-level baselines, achieving up to 18% higher accuracy at the same per-request budget with its sparse profiling reducing offline profiling cost by 98-99.8% when compared to exhaustive profiling.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.23914v1)
