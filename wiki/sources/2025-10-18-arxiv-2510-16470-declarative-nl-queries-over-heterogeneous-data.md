---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Declarative Techniques for NL Queries over Heterogeneous Data"
authors: IBM Research
url: https://arxiv.org/abs/2510.16470
date: 2025-10-18
citationCount: pending-kg-curator
ingested: 2026-06-23
tags: [arxiv, mediated-architecture, semantic-parsing, data-query-agents]
---

# Declarative Techniques for NL Queries over Heterogeneous Data

**arXiv [2510.16470](https://arxiv.org/abs/2510.16470)** · 2025-10-18 · IBM Research

**Significance.** Evidence that for the *fetch* across heterogeneous sources, a **declarative mediator beats a ReAct agent** — separate the logical query from execution planning and let mature query optimisation run. Anchor for [[mediated-semantic-architecture]].

## Abstract
Targets industrial NL questions that need *both* database and API calls. siwarex expresses intent as SQL and invokes APIs from inside SQL via User-Defined Functions, putting APIs "on the same footing as database tables" so decades of SQL optimisation apply. An Abstract Schema (source-agnostic ER view) + API Mapping Schema expose API-backed tables as virtual tables; a rule-based Query Rewriter replaces them with UDFs.

## From the paper (full-text, via subagent)
**Contribution / method.** Declarative separation of intent (SQL) from execution (planning over DB + API), with APIs as virtual tables/UDFs. Baselines: **Imperative** (LLM writes Python orchestrating DB+API) and **Agentic** (ReAct + SQLDatabaseToolkit + xLAM); all use Mistral-Large. Two Spider-augmented benchmarks released (SQL-API-Bench).
**Results.** Benchmark II (2,338 human-vetted Q/A; accuracy / exec-time-per-question): **Declarative2 0.689 / 16.24s**, Declarative 0.639 / 16.50s, Imperative 0.614 / 15.56s, **Agentic 0.357 / 37.81s**. As the API mix rises (20–80%), declarative "outshines the other two substantially"; the agent degrades most steeply, failing on sequencing, routing, and hallucinated/improperly-bound inputs.
**Takeaway.** For the mediated fetch, declarative > agentic — higher accuracy at ~half the latency of ReAct. The logical query is the contract; the wrappers (UDFs/virtual tables) handle physical access. Caveat: execution-accuracy only, tiny Spider tables, scalar-output APIs, not yet deployed.

## Graph
- **Concepts:** [[mediated-semantic-architecture|Mediated semantic architecture]] · [[semantic-parsing]] · [[data-query-agents]]
- **Entities:** [[text-to-query-wrapper]] · [[mediator-wrapper]]
- **Raw:** full-text (alphaXiv, read via subagent) 2026-06-23
