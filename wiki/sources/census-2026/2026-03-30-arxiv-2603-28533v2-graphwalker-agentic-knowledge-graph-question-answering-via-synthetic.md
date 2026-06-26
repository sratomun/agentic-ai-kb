---
type: source
source_type: arxiv
title: "GraphWalker: Agentic Knowledge Graph Question Answering via Synthetic Trajectory Curriculum"
authors: Shuwen Xu, Yao Xu, Jiaxiang Liu, Chenhao Yuan et al.
url: https://arxiv.org/abs/2603.28533v2
date: 2026-03-30
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.CL
tags: [embodied-agents, knowledge-graph, agent-reliability, agentic-rl, arxiv, auto-ingested]
---

# GraphWalker: Agentic Knowledge Graph Question Answering via Synthetic Trajectory Curriculum

**arXiv:** [2603.28533v2](https://arxiv.org/abs/2603.28533v2) · 2026-03-30 · cs.CL
**Authors:** Shuwen Xu, Yao Xu, Jiaxiang Liu, Chenhao Yuan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic knowledge graph question answering (KGQA) requires an agent to iteratively interact with knowledge graphs (KGs), posing challenges in both training data scarcity and reasoning generalization. Specifically, existing approaches often restrict agent exploration: prompting-based methods lack autonomous navigation training, while current training pipelines usually confine reasoning to predefined trajectories. To this end, this paper proposes \textit{GraphWalker}, a novel agentic KGQA framework that addresses these challenges through \textit{Automated Trajectory Synthesis} and \textit{Stage-wise Fine-tuning}. GraphWalker adopts a two-stage SFT training paradigm: First, the agent is trained on structurally diverse trajectories synthesized from constrained random-walk paths, establishing a broad exploration prior over the KG; Second, the agent is further fine-tuned on a small set of expert trajectories to develop reflection and error recovery capabilities. Extensive experiments demonstrate that our stage-wise SFT paradigm unlocks a higher performance ceiling for a lightweight reinforcement learning (RL) stage, enabling GraphWalker to achieve state-of-the-art performance on CWQ and WebQSP. Additional results on GrailQA and our constructed GraphWalkerBench confirm that GraphWalker enhances generalization to out-of-distribution reasoning paths. The code is publicly available at https://github.com/XuShuwenn/GraphWalker

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.28533v2)
