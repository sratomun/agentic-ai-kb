---
type: source
source_type: arxiv
kind: survey
title: "Generate, Filter, Control, Replay: A Comprehensive Survey of Rollout Strategies for LLM Reinforcement Learning"
authors: Rohan Surana, Gagan Mundada, Xunyi Jiang, Chuhan Wang et al.
url: https://arxiv.org/abs/2605.02913v1
date: 2026-04-08
ingested: 2026-06-21
depth: full-text
tags: [agentic-rl, self-evolving-agents, arxiv, survey]
---

# Generate, Filter, Control, Replay: A Comprehensive Survey of Rollout Strategies for LLM Reinforcement Learning

**SURVEY** · arXiv [2605.02913v1](https://arxiv.org/abs/2605.02913v1) · 2026-04-08 · Rohan Surana, Gagan Mundada, Xunyi Jiang, Chuhan Wang et al.

**Why it matters:** The systems-level reference for *how* agentic RL training data is generated — the lever most teams under-engineer.

## What it surveys
Rollout strategies for RL-based post-training of reasoning LLMs — the often-underreported design space that determines what the optimizer learns from.

## Framework / taxonomy
An optimizer-agnostic GFCR lifecycle taxonomy: Generate (propose trajectories/topologies) → Filter (verifiers/judges/critics) → Control (compute allocation, branch/stop under budget) → Replay (reuse artifacts, self-evolving curricula), plus a reliability/coverage/cost criterion taxonomy.

## Notable points
- Synthesizes RLVR, process supervision, judge-gating, tree/segment rollouts, adaptive compute, early-exit, and replay/self-improvement.
- Case studies span math, code/SQL, multimodal, tool-using and agentic-skill benchmarks.
- Provides a diagnostic index mapping rollout pathologies to GFCR modules and mitigations.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[self-evolving-agents|Self-evolving agents]]
- **Raw:** `raw/arxiv/2605.02913v1.md` · `raw/arxiv/2605.02913v1.fulltext.md`

