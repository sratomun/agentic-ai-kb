---
type: source
source_type: arxiv
title: "MedSAM-Agent: Empowering Interactive Medical Image Segmentation with Multi-turn Agentic Reinforcement Learning"
authors: Shengyuan Liu, Liuxin Bao, Qi Yang, Wanting Geng et al.
url: https://arxiv.org/abs/2602.03320v1
date: 2026-02-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.CV
tags: [clinical-agents, agentic-rl, multi-agent-systems, arxiv, auto-ingested]
---

# MedSAM-Agent: Empowering Interactive Medical Image Segmentation with Multi-turn Agentic Reinforcement Learning

**arXiv:** [2602.03320v1](https://arxiv.org/abs/2602.03320v1) · 2026-02-03 · cs.CV
**Authors:** Shengyuan Liu, Liuxin Bao, Qi Yang, Wanting Geng et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Medical image segmentation is evolving from task-specific models toward generalizable frameworks. Recent research leverages Multi-modal Large Language Models (MLLMs) as autonomous agents, employing reinforcement learning with verifiable reward (RLVR) to orchestrate specialized tools like the Segment Anything Model (SAM). However, these approaches often rely on single-turn, rigid interaction strategies and lack process-level supervision during training, which hinders their ability to fully exploit the dynamic potential of interactive tools and leads to redundant actions. To bridge this gap, we propose MedSAM-Agent, a framework that reformulates interactive segmentation as a multi-step autonomous decision-making process. First, we introduce a hybrid prompting strategy for expert-curated trajectory generation, enabling the model to internalize human-like decision heuristics and adaptive refinement strategies. Furthermore, we develop a two-stage training pipeline that integrates multi-turn, end-to-end outcome verification with a clinical-fidelity process reward design to promote interaction parsimony and decision efficiency. Extensive experiments across 6 medical modalities and 21 datasets demonstrate that MedSAM-Agent achieves state-of-the-art performance, effectively unifying autonomous medical reasoning with robust, iterative optimization. Code is available \href{https://github.com/CUHK-AIM-Group/MedSAM-Agent}{here}.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.03320v1)
