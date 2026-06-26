---
type: source
source_type: arxiv
title: "Learning from the Irrecoverable: Error-Localized Policy Optimization for Tool-Integrated LLM Reasoning"
authors: Qiao Liang, Yuke Zhu, Chao Ge, Lei Yang et al.
url: https://arxiv.org/abs/2602.09598v1
date: 2026-02-10
ingested: 2026-06-21
depth: full-text
tags: [agentic-rl, tool-use, arxiv]
---

# Learning from the Irrecoverable: Error-Localized Policy Optimization for Tool-Integrated LLM Reasoning

**Why it matters:** Long-horizon tool use fails when one early irrecoverable step dooms the trajectory — ELPO finds that step via binary-search rollout trees and concentrates credit there. A real fix for sparse-reward credit assignment.

## Takeaways
- ELPO localizes the first irrecoverable step via binary-search rollout trees under a fixed budget.
- Converts the tree into stable signals through hierarchical advantage attribution + error-localized adaptive clipping on the critical step and its suffix.
- Beats strong Agentic-RL baselines across math/science-QA/code-execution at comparable sampling budgets; gains in Pass@K/Major@K and tool-call efficiency.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]]
- **Entities:** [[grpo]]
- **Raw:** `raw/arxiv/2602.09598v1.md` · `raw/arxiv/2602.09598v1.fulltext.md`
