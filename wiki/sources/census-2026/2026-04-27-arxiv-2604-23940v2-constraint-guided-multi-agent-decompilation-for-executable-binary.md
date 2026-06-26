---
type: source
source_type: arxiv
title: "Constraint-Guided Multi-Agent Decompilation for Executable Binary Recovery"
authors: Yifan Zhang, Xiaohan Wang, Yueke Zhang, Yu Huang et al.
url: https://arxiv.org/abs/2604.23940v2
date: 2026-04-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.SE
tags: [agent-reliability, agent-security, multi-agent-systems, arxiv, auto-ingested]
---

# Constraint-Guided Multi-Agent Decompilation for Executable Binary Recovery

**arXiv:** [2604.23940v2](https://arxiv.org/abs/2604.23940v2) · 2026-04-27 · cs.SE
**Authors:** Yifan Zhang, Xiaohan Wang, Yueke Zhang, Yu Huang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Decompilation -- recovering source code from compiled binaries -- is essential for security analysis, malware reverse engineering, and legacy software maintenance. However, existing decompilers produce code that often fails to compile or execute correctly, limiting their practical utility. We present a multi-agent framework that transforms decompiled code into re-executable source through Multi-level Constraint-Guided Decompilation (MCGD). Our approach employs a hierarchical validation pipeline with three constraint levels: (1) syntactic correctness via parsing, (2) compilability via GCC, and (3) behavioral equivalence via LLM-generated test cases. When validation fails, specialized LLM agents iteratively refine the code using structured error feedback. We evaluate our framework on 1,641 real-world binaries from ExeBench across three decompilers (RetDec, Ghidra, and Angr). Our framework achieves 84-97% re-executability, improving baseline decompiler output by 28-89 percentage points. In comparison with state-of-the-art LLM-based decompilation methods using the same GPT-4o backbone, our approach (84.1%) outperforms LLM4Decompile (80.3%), SK2Decompile (73.9%), and SALT4Decompile (61.8%). Our ablation study reveals that execution-based validation is critical: compile-only approaches achieve 0% behavioral correctness despite 91-99% compilation rates. The system converges efficiently, with 90%+ binaries reaching correctness within 2 iterations at an average cost of $0.03-0.05 per binary. Our results demonstrate that constraint-guided agentic refinement can bridge the gap between raw decompiler output and practically useful source code.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[gpt-5]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.23940v2)
