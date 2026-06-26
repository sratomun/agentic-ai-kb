---
type: source
source_type: arxiv
title: "Verified Multi-Agent Orchestration: A Plan-Execute-Verify-Replan Framework for Complex Query Resolution"
authors: Xing Zhang, Yanwei Cui, Guanghui Wang, Wei Qiu et al.
url: https://arxiv.org/abs/2603.11445v2
date: 2026-03-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [multi-agent-systems, arxiv, auto-ingested]
---

# Verified Multi-Agent Orchestration: A Plan-Execute-Verify-Replan Framework for Complex Query Resolution

**arXiv:** [2603.11445v2](https://arxiv.org/abs/2603.11445v2) · 2026-03-12 · cs.AI
**Authors:** Xing Zhang, Yanwei Cui, Guanghui Wang, Wei Qiu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We present Verified Multi-Agent Orchestration (VMAO), a framework that coordinates specialized LLM-based agents through a verification-driven iterative loop. Given a complex query, our system decomposes it into a directed acyclic graph (DAG) of sub-questions, executes them through domain-specific agents in parallel, verifies result completeness via LLM-based evaluation, and adaptively replans to address gaps. The key contributions are: (1) dependency-aware parallel execution over a DAG of sub-questions with automatic context propagation, (2) verification-driven adaptive replanning that uses an LLM-based verifier as an orchestration-level coordination signal, and (3) configurable stop conditions that balance answer quality against resource usage. On 25 expert-curated market research queries, VMAO improves answer completeness from 3.1 to 4.2 and source quality from 2.6 to 4.1 (1-5 scale) compared to a single-agent baseline, demonstrating that orchestration-level verification is an effective mechanism for multi-agent quality assurance.

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.11445v2)
