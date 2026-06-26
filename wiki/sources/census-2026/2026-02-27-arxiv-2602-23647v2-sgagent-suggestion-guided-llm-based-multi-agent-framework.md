---
type: source
source_type: arxiv
title: "SGAgent: Suggestion-Guided LLM-Based Multi-Agent Framework for Repository-Level Software Repair"
authors: Quanjun Zhang, Chengyu Gao, Yu Han, Ye Shang et al.
url: https://arxiv.org/abs/2602.23647v2
date: 2026-02-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 13
primary: cs.SE
tags: [coding-agents, knowledge-graph, agent-security, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# SGAgent: Suggestion-Guided LLM-Based Multi-Agent Framework for Repository-Level Software Repair

**arXiv:** [2602.23647v2](https://arxiv.org/abs/2602.23647v2) · 2026-02-27 · cs.SE
**Authors:** Quanjun Zhang, Chengyu Gao, Yu Han, Ye Shang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) have enabled intelligent agents that autonomously interact with environments and invoke external tools. Recently, agent-based software repair has drawn wide attention, as repair agents can localize bugs, generate patches, and achieve state-of-the-art performance on repository-level benchmarks (e.g., SWE-Bench). However, existing approaches usually adopt a localize-then-fix paradigm, jumping directly from "where the bug is" to "how to fix it", leaving a fundamental reasoning gap. To this end, we propose SGAgent, a Suggestion-Guided multi-Agent framework for repository-level software repair, which follows a localize-suggest-fix paradigm. SGAgent introduces a suggestion phase to strengthen the transition from localization to repair: the suggester starts from the buggy locations, incrementally retrieves relevant context until it fully understands the bug, and provides actionable repair suggestions. We further construct a Knowledge Graph (KG) from the target repository and develop a KG-based toolkit to strengthen SGAgent's global contextual awareness and repository-level reasoning. Three specialized sub-agents (i.e., localizer, suggester, and fixer) collaborate to achieve automated end-to-end software repair. We evaluate SGAgent on SWE-Bench-Lite. SGAgent with Claude-3.5 achieves 51.3% repair accuracy, 81.2% file-level, and 52.4% function-level localization accuracy at an average cost of $1.48 per instance, outperforming all baselines using the same base model. SGAgent also generalizes well across base LLMs, reaching a 60.7% resolution rate with Claude-4. When extended to vulnerability repair, it achieves 48.0% on VUL4J and VJBench, demonstrating strong generalization across tasks and programming languages.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[claude]] · [[swe-bench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.23647v2)
