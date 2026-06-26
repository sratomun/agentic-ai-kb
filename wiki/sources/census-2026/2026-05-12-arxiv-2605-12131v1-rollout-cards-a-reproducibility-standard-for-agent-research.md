---
type: source
source_type: arxiv
title: "Rollout Cards: A Reproducibility Standard for Agent Research"
authors: Charlie Masters, Ziyuan Liu, Stefano V. Albrecht
url: https://arxiv.org/abs/2605.12131v1
date: 2026-05-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [coding-agents, agentic-rl, agent-security, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# Rollout Cards: A Reproducibility Standard for Agent Research

**arXiv:** [2605.12131v1](https://arxiv.org/abs/2605.12131v1) · 2026-05-12 · cs.AI
**Authors:** Charlie Masters, Ziyuan Liu, Stefano V. Albrecht

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Reproducibility problems that have long affected machine learning and reinforcement learning are now surfacing in agent research: papers compare systems by reported scores while leaving the rollout records behind those scores difficult to inspect. For agentic tasks, this matters because the same behaviour can receive different reported scores when evaluations select different parts of a rollout or apply different reporting rules. In a structured audit of 50 popular training and evaluation repositories, we find that none report how many runs failed, errored, or were skipped alongside headline scores. We also document 37 cases where reporting rules can change task-success rates, cost/token accounting, or timing measurements for fixed evidence, sometimes dramatically. We treat rollout records, not reported scores, as the unit of reproducibility for agent research. We introduce rollout cards: publication bundles that preserve the rollout record and declare the views, reporting rules, and drops manifests behind reported scores. We validate rollout cards in two settings. First, four partial public releases in tool safety, multi-agent systems, theorem proving, and search let us compute analyses their original reports did not include. Second, re-grading preserved benchmark outputs across short-answer, code-generation, and tool-use tasks shows that changing only the reporting rule can change reported scores by 20.9 absolute percentage points and, in some cases, invert rankings of frontier models. We release a reference implementation integrated into Ergon, an open-source reinforcement learning gym, and publicly publish Ergon-produced rollout-card exports for benchmarks spanning tool use, software engineering, web interaction, multi-agent coordination, safety, and search to support future research.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.12131v1)
