---
type: source
source_type: arxiv
title: "6GAgentGym: Tool Use, Data Synthesis, and Agentic Learning for Network Management"
authors: Jiao Chen, Jianhua Tang, Xiaotong Yang, Zuohong Lv
url: https://arxiv.org/abs/2603.29656v1
date: 2026-03-31
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.NI
tags: [agentic-rl, agent-memory, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# 6GAgentGym: Tool Use, Data Synthesis, and Agentic Learning for Network Management

**arXiv:** [2603.29656v1](https://arxiv.org/abs/2603.29656v1) · 2026-03-31 · cs.NI
**Authors:** Jiao Chen, Jianhua Tang, Xiaotong Yang, Zuohong Lv

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Autonomous 6G network management requires agents that can execute tools, observe the resulting state changes, and adapt their decisions accordingly. Existing benchmarks based on static questions or scripted episode replay, however, do not support such closed-loop interaction, limiting agents to passive evaluation without the ability to learn from environmental feedback. This paper presents 6GAgentGym to provide closed-loop capability. The framework provides an interactive environment with 42 typed tools whose effect classification distinguishes read-only observation from state-mutating configuration, backed by a learned Experiment Model calibrated on NS-3 simulation data. 6G-Forge bootstraps closed-loop training trajectories from NS-3 seeds via iterative Self-Instruct generation with execution verification against the Experiment Model. Supervised fine-tuning on the resulting corpus followed by reinforcement learning with online closed-loop interaction enables an 8B open-source model to achieve comparable overall success rate to GPT-5 on the accompanying 6GAgentBench, with stronger performance on long-horizon tasks. Together, these components provide a viable path toward autonomous, closed-loop network management.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]] · [[agentbench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.29656v1)
