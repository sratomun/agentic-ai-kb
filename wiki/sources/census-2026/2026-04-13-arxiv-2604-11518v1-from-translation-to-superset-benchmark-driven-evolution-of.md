---
type: source
source_type: arxiv
title: "From Translation to Superset: Benchmark-Driven Evolution of a Production AI Agent from Rust to Python"
authors: Jinhua Wang, Biswa Sengupta
url: https://arxiv.org/abs/2604.11518v1
date: 2026-04-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.SE
tags: [coding-agents, agent-security, agent-protocols, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# From Translation to Superset: Benchmark-Driven Evolution of a Production AI Agent from Rust to Python

**arXiv:** [2604.11518v1](https://arxiv.org/abs/2604.11518v1) · 2026-04-13 · cs.SE
**Authors:** Jinhua Wang, Biswa Sengupta

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Cross-language migration of large software systems is a persistent engineering challenge, particularly when the source codebase evolves rapidly. We present a methodology for LLM-assisted continuous code translation in which a large language model translates a production Rust codebase (648K LOC, 65 crates) into Python (41K LOC, 28 modules), with public agent benchmarks as the objective function driving iterative refinement. Our subject system is Codex CLI, a production AI coding agent. We demonstrate that: (1) the Python port resolves 59/80 SWE-bench Verified tasks (73.8%) versus Rust's 56/80 (70.0%), and achieves 42.5% on Terminal-Bench versus Rust's 47.5%, confirming near-parity on real-world agentic tasks; (2) benchmark-driven debugging, revealing API protocol mismatches, environment pollution, a silent WebSocket failure mode, and an API 400 crash, is more effective than static testing alone; (3) the architecture supports continuous upstream synchronisation via an LLM-assisted diff-translate-test loop; and (4) the Python port has evolved into a capability superset with 30 feature-flagged extensions (multi-agent orchestration, semantic memory, guardian safety, cost tracking) absent from Rust, while preserving strict parity mode for comparison. Our evaluation shows that for LLM-based agents where API latency dominates, Python's expressiveness yields a 15.9x code reduction with negligible performance cost, while the benchmark-as-objective-function methodology provides a principled framework for growing a cross-language port from parity into an extended platform.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[swe-bench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.11518v1)
