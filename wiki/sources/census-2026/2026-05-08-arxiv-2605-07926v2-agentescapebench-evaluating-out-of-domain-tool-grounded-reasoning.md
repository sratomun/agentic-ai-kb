---
type: source
source_type: arxiv
title: "AgentEscapeBench: Evaluating Out-of-Domain Tool-Grounded Reasoning in LLM Agents"
authors: Zhengkang Guo, Yiyang Li, Lin Qiu, Xiaohua Wang et al.
url: https://arxiv.org/abs/2605.07926v2
date: 2026-05-08
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [clinical-agents, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# AgentEscapeBench: Evaluating Out-of-Domain Tool-Grounded Reasoning in LLM Agents

**arXiv:** [2605.07926v2](https://arxiv.org/abs/2605.07926v2) · 2026-05-08 · cs.AI
**Authors:** Zhengkang Guo, Yiyang Li, Lin Qiu, Xiaohua Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As LLM-based agents increasingly rely on external tools, it is important to evaluate their ability to sustain tool-grounded reasoning beyond familiar workflows and short-range interactions. We introduce AgentEscapeBench, an escape-room-style benchmark that tests whether agents can infer, execute, and revise novel tool-use procedures under explicit long-range dependency constraints. Each task defines a directed acyclic dependency graph over tools and items, requiring agents to invoke real external functions, track hidden state revealed incrementally, propagate intermediate results, and submit a deterministically verifiable final answer. AgentEscapeBench includes 270 instances across five difficulty tiers and supports fully automated evaluation. Experiments with sixteen LLM agents and human participants show that performance drops sharply as dependency depth increases: humans decline from 98.3% success at difficulty-5 to 80.0% at difficulty-25, while the best model drops from 90.0% to 60.0%. Trajectory analysis attributes model failures mainly to breakdowns in long-range state tracking, clue adherence, and intermediate-result propagation. These findings suggest that current agents can often handle local tool use but still struggle with deep contextual dependencies. We hope AgentEscapeBench can serve as a diagnostic testbed for measuring current agent capabilities and informing future training efforts toward more robust general-purpose reasoning, action, and adaptation.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.07926v2)
