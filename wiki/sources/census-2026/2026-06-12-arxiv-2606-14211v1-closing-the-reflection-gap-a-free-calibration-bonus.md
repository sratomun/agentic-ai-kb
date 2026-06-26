---
type: source
source_type: arxiv
title: "Closing the Reflection Gap: A Free Calibration Bonus for Agentic RL"
authors: Yinglun Zhu
url: https://arxiv.org/abs/2606.14211v1
date: 2026-06-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 15
primary: cs.AI
tags: [data-query-agents, self-evolving-agents, agentic-rl, agent-evaluation, arxiv, auto-ingested]
---

# Closing the Reflection Gap: A Free Calibration Bonus for Agentic RL

**arXiv:** [2606.14211v1](https://arxiv.org/abs/2606.14211v1) · 2026-06-12 · cs.AI
**Authors:** Yinglun Zhu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLMs are increasingly deployed as agents that interact with external environments and observe feedback such as execution results, error messages, and tool outputs. A well-functioning agent should be able to leverage this feedback to accurately assess its own performance. Yet we find a persistent reflection gap: LLM agents tend to mis-assess their own outputs after observing concrete environment feedback -- even for questions they correctly answered -- and standard RL barely helps due to a credit-assignment mismatch. To close this gap, we propose RefGRPO, a simple yet effective fix that augments standard RL algorithms with two key ingredients: a free calibration bonus computed by contrasting the agent's own reflection with the actual outcome (requiring no additional reward model, LLM judge, or external annotation), and a dynamic schedule on its coefficient. Compared to standard RL baselines, our method simultaneously improves reflection calibration (e.g., reduces underconfidence rate $44.4\% \to 7.7\%$) and task accuracy (e.g., $75.1\% \to 76.5\%$) on text-to-SQL across five benchmarks. The resulting calibrated reflection turns the agent into its own verifier grounded in environment feedback, which further enables (i) better self-improvement that uses reflections as pseudo-rewards without outcome supervision, and (ii) more effective test-time selective prediction by committing only to rollouts flagged as correct.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.14211v1)
