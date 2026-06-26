---
type: source
source_type: arxiv
title: "Robust and Efficient Tool Orchestration via Layered Execution Structures with Reflective Correction"
authors: Tao Zhe, Haoyu Wang, Bo Luo, Min Wu et al.
url: https://arxiv.org/abs/2602.18968v2
date: 2026-02-21
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.AI
tags: [tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# Robust and Efficient Tool Orchestration via Layered Execution Structures with Reflective Correction

**arXiv:** [2602.18968v2](https://arxiv.org/abs/2602.18968v2) · 2026-02-21 · cs.AI
**Authors:** Tao Zhe, Haoyu Wang, Bo Luo, Min Wu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Tool invocation is a core capability of agentic systems, yet failures often arise not from individual tool calls but from how multiple tools are organized and executed together. Existing approaches tightly couple tool execution with stepwise language reasoning or explicit planning, leading to brittle behavior and high execution overhead. To overcome these limitations, we revisit tool invocation from the perspective of tool orchestration. Our key insight is that effective orchestration does not require precise dependency graphs or fine-grained planning. Instead, a coarse-grained layer structure suffices to provide global guidance, while execution-time errors can be corrected locally. Specifically, we model tool orchestration as learning a layered execution structure that captures high-level tool dependencies, inducing layer-wise execution through context constraints. To handle execution-time failures, we introduce a schema-aware reflective correction mechanism that detects and repairs errors locally. This design confines errors to individual tool calls and avoids re-planning entire execution trajectories. This structured execution paradigm enables a lightweight and reusable orchestration component for agentic systems. Experimental results show that our approach achieves robust tool execution while reducing execution complexity and overhead. Code will be made publicly available.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.18968v2)
