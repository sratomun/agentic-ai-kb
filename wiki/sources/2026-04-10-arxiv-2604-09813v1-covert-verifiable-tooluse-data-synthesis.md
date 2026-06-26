---
type: source
source_type: arxiv
title: "Controllable and Verifiable Tool-Use Data Synthesis for Agentic Reinforcement Learning"
authors: Siyuan Xu, Shiyang Li, Xin Liu, Tianyi Liu et al.
url: https://arxiv.org/abs/2604.09813v1
date: 2026-04-10
ingested: 2026-06-21
depth: full-text
tags: [agentic-rl, tool-use, agent-evaluation, arxiv]
---

# Controllable and Verifiable Tool-Use Data Synthesis for Agentic Reinforcement Learning

**Why it matters:** RL needs executable, reward-checkable environments, not just SFT corpora — COVERT synthesizes oracle-preserving tool-use trajectories with distractors/noise so policies learn robustness under ambiguity.

## Takeaways
- COVERT: two-stage pipeline — self-evolving base trajectory synthesis with multi-level validation, then oracle-preserving augmentations (distractor tools, ambiguous queries, noisy/erroneous outputs).
- Enables automatic reward via reference matching + lightweight judge verification for special behaviors (e.g. error detection).
- Qwen2.5-14B: BFCL v3 56.5→59.9, ACEBench 53.0→59.3; stacks additively on SFT (→62.1 / 61.8).

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[bfcl]]
- **Raw:** `raw/arxiv/2604.09813v1.md` · `raw/arxiv/2604.09813v1.fulltext.md`
