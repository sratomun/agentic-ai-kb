---
type: source
source_type: arxiv
title: "ToolCUA: Towards Optimal GUI-Tool Path Orchestration for Computer Use Agents"
authors: Xuhao Hu, Xi Zhang, Haiyang Xu, Kyle Qiao et al.
url: https://arxiv.org/abs/2605.12481v1
date: 2026-05-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 23
primary: cs.AI
tags: [computer-use-agents, agentic-rl, agent-protocols, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# ToolCUA: Towards Optimal GUI-Tool Path Orchestration for Computer Use Agents

**arXiv:** [2605.12481v1](https://arxiv.org/abs/2605.12481v1) · 2026-05-12 · cs.AI
**Authors:** Xuhao Hu, Xi Zhang, Haiyang Xu, Kyle Qiao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Computer Use Agents (CUAs) can act through both atomic GUI actions, such as click and type, and high-level tool calls, such as API-based file operations, but this hybrid action space often leaves them uncertain about when to continue with GUI actions or switch to tools, leading to suboptimal execution paths. This difficulty stems from the scarcity of high-quality interleaved GUI-Tool trajectories, the cost and brittleness of collecting real tool trajectories, and the lack of trajectory-level supervision for GUI-Tool path selection. In this paper, we propose ToolCUA, an end-to-end agent designed to learn optimal GUI-Tool path selection through a staged training paradigm. We first introduce an Interleaved GUI-Tool Trajectory Scaling Pipeline that repurposes abundant static GUI trajectories and synthesizes a grounded tool library, enabling diverse GUI-Tool trajectories without manual engineering or real tool-trajectory collection. We then perform Tool-Bootstrapped GUI RFT, combining warmup SFT with single-turn RL to improve decisions at critical GUI-Tool switching points. Finally, we optimize ToolCUA with Online Agentic RL in a high-fidelity GUI-Tool environment, guided by a Tool-Efficient Path Reward that encourages appropriate tool use and shorter execution paths. Experiments on OSWorld-MCP show that ToolCUA achieves 46.85% accuracy, a relative improvement of approximately 66% over the baseline, establishing a new state of the art among models of comparable scale. It also improves by 3.9% over GUI-only settings, demonstrating effective GUI-Tool orchestration. The results further suggest that training in a hybrid action space is a promising paradigm for real-world digital agents. Open-sourced here: https://x-plug.github.io/ToolCUA/

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agentic-rl|Agentic RL]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[mcp]] · [[osworld]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.12481v1)
