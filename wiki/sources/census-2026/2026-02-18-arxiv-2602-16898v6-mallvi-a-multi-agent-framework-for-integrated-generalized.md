---
type: source
source_type: arxiv
title: "MALLVI: A Multi-Agent Framework for Integrated Generalized Robotics Manipulation"
authors: Mehrshad Taji, Arad Mahdinezhad Kashani, Iman Ahmadi, AmirHossein Jadidi et al.
url: https://arxiv.org/abs/2602.16898v6
date: 2026-02-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.RO
tags: [embodied-agents, agent-reliability, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# MALLVI: A Multi-Agent Framework for Integrated Generalized Robotics Manipulation

**arXiv:** [2602.16898v6](https://arxiv.org/abs/2602.16898v6) · 2026-02-18 · cs.RO
**Authors:** Mehrshad Taji, Arad Mahdinezhad Kashani, Iman Ahmadi, AmirHossein Jadidi et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Task planning for robotic manipulation with large language models (LLMs) is an emerging area. Prior approaches rely on specialized models, fine tuning, or prompt tuning, and often operate in an open loop manner without robust environmental feedback, making them fragile in dynamic settings. MALLVI presents a Multi Agent Large Language and Vision framework that enables closed-loop feedback driven robotic manipulation. Given a natural language instruction and an image of the environment, MALLVI generates executable atomic actions for a robot manipulator. After action execution, a Vision Language Model (VLM) evaluates environmental feedback and decides whether to repeat the process or proceed to the next step. Rather than using a single model, MALLVI coordinates specialized agents, Decomposer, Localizer, Thinker, and Reflector, to manage perception, localization, reasoning, and high level planning. An optional Descriptor agent provides visual memory of the initial state. The Reflector supports targeted error detection and recovery by reactivating only relevant agents, avoiding full replanning. Experiments in simulation and real-world settings show that iterative closed loop multi agent coordination improves generalization and increases success rates in zero shot manipulation tasks. Code available at https://github.com/iman1234ahmadi/MALLVI .

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.16898v6)
