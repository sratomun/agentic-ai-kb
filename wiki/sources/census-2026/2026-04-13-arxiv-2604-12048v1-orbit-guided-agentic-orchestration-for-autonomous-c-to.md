---
type: source
source_type: arxiv
title: "ORBIT: Guided Agentic Orchestration for Autonomous C-to-Rust Transpilation"
authors: Muhammad Farrukh, Baris Coskun, Tapti Palit, Michalis Polychronakis
url: https://arxiv.org/abs/2604.12048v1
date: 2026-04-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.SE
tags: [coding-agents, embodied-agents, agent-security, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# ORBIT: Guided Agentic Orchestration for Autonomous C-to-Rust Transpilation

**arXiv:** [2604.12048v1](https://arxiv.org/abs/2604.12048v1) · 2026-04-13 · cs.SE
**Authors:** Muhammad Farrukh, Baris Coskun, Tapti Palit, Michalis Polychronakis

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large-scale migration of legacy C code to Rust offers a promising path toward improving memory safety, but LLM-based C-to-Rust translation remains challenging due to limited context windows and hallucinations. Prior approaches are evaluated primarily on small programs or datasets skewed toward small codebases, providing limited insight into scalability on real-world systems. They also rely on static context construction, which breaks down in the presence of complex cross-module dependencies and often requires manual intervention. Recent coding agents offer a promising alternative through dynamic codebase navigation and context curation. When used out of the box, however, they frequently produce incomplete translations that appear superficially correct. We present ORBIT, an autonomous agentic framework for project-level C-to-Rust translation that combines dynamic context collection with dependency-guided orchestration and iterative verification. ORBIT constructs a dependency-aware translation graph, generates Rust interfaces, maps C functions to Rust counterparts, and coordinates multiple specialized agents. We evaluate ORBIT on 24 programs from CRUST-Bench, with 91.7% of the programs exceeding 1,000 lines of code. ORBIT achieves 100% compilation success and 91.7% test success in both expert-interface and automatically generated-interface settings, substantially outperforming C2Rust and CRUST-Bench, while reducing unsafe Rust code blocks to nearly zero. We further evaluate ORBIT on challenging cases from the DARPA TRACTOR benchmark, where it achieves competitive performance relative to participating systems.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[embodied-agents|Embodied agents]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.12048v1)
