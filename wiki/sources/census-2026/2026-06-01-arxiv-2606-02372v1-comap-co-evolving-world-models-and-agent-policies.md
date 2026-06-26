---
type: source
source_type: arxiv
title: "COMAP: Co-Evolving World Models and Agent Policies for LLM Agents"
authors: Youwei Liu, Jian Wang, Hanlin Wang, Wenjie Li
url: https://arxiv.org/abs/2606.02372v1
date: 2026-06-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [computer-use-agents, embodied-agents, agent-reliability, self-evolving-agents, agentic-rl, arxiv, auto-ingested]
---

# COMAP: Co-Evolving World Models and Agent Policies for LLM Agents

**arXiv:** [2606.02372v1](https://arxiv.org/abs/2606.02372v1) · 2026-06-01 · cs.AI
**Authors:** Youwei Liu, Jian Wang, Hanlin Wang, Wenjie Li

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Equipping language agents with world models enables them to anticipate environment dynamics and evaluate candidate actions before execution. However, existing textual world models are typically fixed after training, preventing them from adapting to the on-policy state-action distributions induced by an evolving agent. Meanwhile, agent-improvement methods often rely on external rewards or verifiers, limiting their applicability in realistic interactive environments. In this paper, we propose COMAP, a novel framework that co-evolves textual world models and agent policies through closed-loop interaction. At each decision step, the world model predicts future state feedback for candidate actions, and the agent performs future-aware reflection by estimating the reliability of this feedback and refining its action accordingly. The resulting on-policy trajectories are then used to update the world model via self-distillation, allowing it to better match the agent's evolving interaction distribution. Across embodied task planning, Web navigation, and tool-use benchmarks, COMAP consistently outperforms competitive baselines, e.g., +16.75% relative improvement with Qwen3-4B. Further analyses show that the co-evolutionary loop improves the world model's prediction accuracy over time and leads to more effective long-horizon decision-making. Our code is available at: https://github.com/loyiv/CoMAP.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.02372v1)
