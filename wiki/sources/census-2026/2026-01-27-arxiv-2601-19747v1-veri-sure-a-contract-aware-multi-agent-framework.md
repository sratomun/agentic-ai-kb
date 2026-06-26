---
type: source
source_type: arxiv
title: "Veri-Sure: A Contract-Aware Multi-Agent Framework with Temporal Tracing and Formal Verification for Correct RTL Code Generation"
authors: Jiale Liu, Taiyu Zhou, Tianqi Jiang
url: https://arxiv.org/abs/2601.19747v1
date: 2026-01-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.AR
tags: [coding-agents, agent-reliability, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Veri-Sure: A Contract-Aware Multi-Agent Framework with Temporal Tracing and Formal Verification for Correct RTL Code Generation

**arXiv:** [2601.19747v1](https://arxiv.org/abs/2601.19747v1) · 2026-01-27 · cs.AR
**Authors:** Jiale Liu, Taiyu Zhou, Tianqi Jiang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
In the rapidly evolving field of Electronic Design Automation (EDA), the deployment of Large Language Models (LLMs) for Register-Transfer Level (RTL) design has emerged as a promising direction. However, silicon-grade correctness remains bottlenecked by: (i) limited test coverage and reliability of simulation-centric evaluation, (ii) regressions and repair hallucinations introduced by iterative debugging, and (iii) semantic drift as intent is reinterpreted across agent handoffs. In this work, we propose Veri-Sure, a multi-agent framework that establishes a design contract to align agents' intent and uses a patching mechanism guided by static dependency slicing to perform precise, localized repairs. By integrating a multi-branch verification pipeline that combines trace-driven temporal analysis with formal verification consisting of assertion-based checking and boolean equivalence proofs, Veri-Sure enables functional correctness beyond pure simulations. We also introduce VerilogEval-v2-EXT, extending the original benchmark with 53 more industrial-grade design tasks and stratified difficulty levels, and show that Veri-Sure achieves state-of-the-art verified-correct RTL code generation performance, surpassing standalone LLMs and prior agentic systems.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.19747v1)
