---
type: source
source_type: arxiv
title: "Knowledge-Guided Manipulation Using Multi-Task Reinforcement Learning"
authors: Aditya Narendra, Mukhammadrizo Maribjonov, Dmitry Makarov, Dmitry Yudin et al.
url: https://arxiv.org/abs/2603.24083v1
date: 2026-03-25
ingested: 2026-06-21
depth: abstract
auto: true
score: 1
primary: cs.RO
tags: [embodied-agents, knowledge-graph, agent-reliability, agentic-rl, agent-memory, arxiv, auto-ingested]
---

# Knowledge-Guided Manipulation Using Multi-Task Reinforcement Learning

**arXiv:** [2603.24083v1](https://arxiv.org/abs/2603.24083v1) · 2026-03-25 · cs.RO
**Authors:** Aditya Narendra, Mukhammadrizo Maribjonov, Dmitry Makarov, Dmitry Yudin et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
This paper introduces Knowledge Graph based Massively Multi-task Model-based Policy Optimization (KG-M3PO), a framework for multi-task robotic manipulation in partially observable settings that unifies Perception, Knowledge, and Policy. The method augments egocentric vision with an online 3D scene graph that grounds open-vocabulary detections into a metric, relational representation. A dynamic-relation mechanism updates spatial, containment, and affordance edges at every step, and a graph neural encoder is trained end-to-end through the RL objective so that relational features are shaped directly by control performance. Multiple observation modalities (visual, proprioceptive, linguistic, and graph-based) are encoded into a shared latent space, upon which the RL agent operates to drive the control loop. The policy conditions on lightweight graph queries alongside visual and proprioceptive inputs, yielding a compact, semantically informed state for decision making. Experiments on a suite of manipulation tasks with occlusions, distractors, and layout shifts demonstrate consistent gains over strong baselines: the knowledge-conditioned agent achieves higher success rates, improved sample efficiency, and stronger generalization to novel objects and unseen scene configurations. These results support the premise that structured, continuously maintained world knowledge is a powerful inductive bias for scalable, generalizable manipulation: when the knowledge module participates in the RL computation graph, relational representations align with control, enabling robust long-horizon behavior under partial observability.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.24083v1)
