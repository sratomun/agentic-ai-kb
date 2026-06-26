---
type: source
source_type: arxiv
title: "TOBench: A Task-Oriented Omni-Modal Benchmark for Real-World Tool-Using Agents"
authors: Zhiqiang Liu, Wenhui Dong, Yilang Tan, Yuwen Qu et al.
url: https://arxiv.org/abs/2605.16909v1
date: 2026-05-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.AI
tags: [computer-use-agents, agent-protocols, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# TOBench: A Task-Oriented Omni-Modal Benchmark for Real-World Tool-Using Agents

**arXiv:** [2605.16909v1](https://arxiv.org/abs/2605.16909v1) · 2026-05-16 · cs.AI
**Authors:** Zhiqiang Liu, Wenhui Dong, Yilang Tan, Yuwen Qu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Tool-using agents are increasingly expected to operate across realistic professional workflows, where they must interpret multimodal inputs, coordinate external tools, inspect intermediate artifacts, and revise their actions before producing a final result. Existing benchmarks, however, often evaluate tool use, computer use, and multimodal reasoning in isolation, leaving a gap between benchmark settings and end-to-end omni-modal tool use in the real world. To address this gap, we introduce MM-ToolBench, a benchmark and evaluation harness for task-oriented omni-modal tool use. MM-ToolBench contains 100 executable tasks from two macro task families, Customer Service and Intelligent Creation, covering 20 subcategory slices and supported by 27 MCP servers with 324 tools. The central design of MM-ToolBench is closed-loop multimodal verification: agents must execute tools, inspect rendered or transformed artifacts, and self-correct when outputs fail task-specific requirements. To make such evaluation scalable and verifiable, MM-ToolBench couples MCP-based execution with task-specific grounded evaluators and a semi-automated construction pipeline for scenario discovery, task instantiation, evaluator synthesis, and human audit. Experiments on 15 contemporary agentic models show that MM-ToolBench remains highly challenging: Claude Opus 4.6, commonly regarded as one of the strongest coding-agent models, achieves only 32.0% task success, far below the 94.0% human benchmark. We envision MM-ToolBench as a practical foundation for evaluating and advancing next-generation omni-modal tool-using agents through closed-loop multimodal verification.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]] · [[claude]] · [[toolbench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.16909v1)
