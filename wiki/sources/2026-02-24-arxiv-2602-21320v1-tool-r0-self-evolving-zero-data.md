---
type: source
source_type: arxiv
title: "Tool-R0: Self-Evolving LLM Agents for Tool-Learning from Zero Data"
authors: Emre Can Acikgoz, Cheng Qian, Jonas Hübotter, Heng Ji et al.
url: https://arxiv.org/abs/2602.21320v1
date: 2026-02-24
ingested: 2026-06-21
depth: full-text
tags: [self-evolving-agents, agentic-rl, tool-use, arxiv]
---

# Tool-R0: Self-Evolving LLM Agents for Tool-Learning from Zero Data

**Why it matters:** Trains tool-calling agents from scratch with self-play RL under a zero-data assumption — a Generator/Solver co-evolution loop that needs no task datasets. A concrete step toward open-ended self-improvement.

## Takeaways
- Tool-R0 co-evolves a Generator (proposes tasks at the Solver's competence frontier) and a Solver (learns to solve with real tool calls) from the same base model.
- Zero-data self-play: no pre-existing task-solution pairs or human supervision required.
- 92.5% relative improvement over base; surpasses fully supervised tool-calling baselines under the same setting; analyzes co-evolution/curriculum/scaling dynamics.

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]]
- **Raw:** `raw/arxiv/2602.21320v1.md` · `raw/arxiv/2602.21320v1.fulltext.md`
