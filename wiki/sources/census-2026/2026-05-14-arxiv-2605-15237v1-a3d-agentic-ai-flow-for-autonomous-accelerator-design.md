---
type: source
source_type: arxiv
title: "A3D: Agentic AI flow for autonomous Accelerator Design"
authors: Abinand Nallathambi, Christopher Knight, Shantanu Ganguly, Wilfried Haensch et al.
url: https://arxiv.org/abs/2605.15237v1
date: 2026-05-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.AR
tags: [science-agents, agentic-rag, multi-agent-systems, arxiv, auto-ingested]
---

# A3D: Agentic AI flow for autonomous Accelerator Design

**arXiv:** [2605.15237v1](https://arxiv.org/abs/2605.15237v1) · 2026-05-14 · cs.AR
**Authors:** Abinand Nallathambi, Christopher Knight, Shantanu Ganguly, Wilfried Haensch et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Accelerating applications through the design of hardware accelerators can significantly enhance system performance and energy efficiency. Despite advances, such as high-level synthesis (HLS), designing accelerators for complex applications still remains highly labor-intensive, demanding considerable expertise in understanding workloads to be accelerated, hardware design, micro-architecture, and EDA tool usage, posing challenges for application domain experts. Therefore, most accelerator solutions are limited to applications with a regular predictable dataflow. Advances in AI have enabled agents that perform autonomous planning, reasoning, execution and reflection, leading to unprecedented potential for automation through agentic AI. We present A3D, an Agentic AI flow for end-to-end Automation of hardware Accelerator Design. A3D automates workload analysis, performance bottleneck identification, code refactoring for HLS compatibility and micro-architecture generation. A3D also generates diverse accelerator designs by automatically exploring the speed-area tradeoff space. Recent efforts have explored the use of AI for specific tasks such as design space exploration in HLS, leaving several tasks to still be performed manually. A3D addresses the challenges in applying modern LLMs to accelerator design by judiciously partitioning tasks among specialist agents, orchestrating process loops with specialist and verifier agents, utilizing pre-existing and custom tools, and employing agentic RAG for codebase and proprietary EDA tool documentation exploration. Our implementation of A3D, using commercial components like Claude Sonnet 4.5 and the Catapult HLS tool, demonstrates its effectiveness by generating accelerator designs with no human intervention from complex scientific applications like LAMMPS (molecular dynamics simulation) and QMCPACK (quantum chemistry).

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[claude]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.15237v1)
