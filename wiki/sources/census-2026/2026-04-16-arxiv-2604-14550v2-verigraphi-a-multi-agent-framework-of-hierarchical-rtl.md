---
type: source
source_type: arxiv
title: "VeriGraphi: A Multi-Agent Framework of Hierarchical RTL Generation for Large Hardware Designs"
authors: Sazzadul Islam, Tasnim Tabassum, Hao Zheng
url: https://arxiv.org/abs/2604.14550v2
date: 2026-04-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.AR
tags: [coding-agents, knowledge-graph, agent-reliability, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# VeriGraphi: A Multi-Agent Framework of Hierarchical RTL Generation for Large Hardware Designs

**arXiv:** [2604.14550v2](https://arxiv.org/abs/2604.14550v2) · 2026-04-16 · cs.AR
**Authors:** Sazzadul Islam, Tasnim Tabassum, Hao Zheng

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Generating synthesizable Verilog for large, hierarchical hardware designs remains a significant challenge for large language models (LLMs), which struggle to replicate the structured reasoning that human experts employ when translating complex specifications into RTL. When tasked with producing hierarchical Verilog, LLMs frequently lose context across modules, hallucinate interfaces, fabricate inter-module wiring, and fail to maintain structural coherence - failures that intensify as design complexity grows and specifications involve informal prose, figures, and tables that resist direct operationalization. To address these challenges, we present VeriGraphi, a framework that introduces a spec-anchored Knowledge Graph as the architectural substrate driving the RTL generation pipeline. VeriGraphi constructs a HDA, a structured knowledge graph that explicitly encodes module hierarchy, port-level interfaces, wiring semantics, and inter-module dependencies as first-class graph entities and relations. Built through iterative multi-agent analysis of the specification, this Knowledge Graph provides a deterministic, machine-checkable structural scaffold before code generation. Guided by the KG, a progressive coding module incrementally generates pseudo-code and synthesizable RTL while enforcing interface consistency and dependency correctness at each submodule stage. We evaluate VeriGraphi on a benchmark of three representative specification documents from the National Institute of Standards and Technology and their corresponding implementations, and we present a RV32I processor as a detailed case study to illustrate the full pipeline. The results demonstrate that VeriGraphi enables reliable hierarchical RTL generation with minimal human intervention for RISC-V, marking a significant milestone for LLM-generated hardware design while maintaining strong functional correctness.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.14550v2)
