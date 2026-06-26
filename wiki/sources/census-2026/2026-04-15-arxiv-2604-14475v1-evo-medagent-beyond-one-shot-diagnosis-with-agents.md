---
type: source
source_type: arxiv
title: "Evo-MedAgent: Beyond One-Shot Diagnosis with Agents That Remember, Reflect, and Improve"
authors: Weixiang Shen, Bailiang Jian, Jun Li, Che Liu et al.
url: https://arxiv.org/abs/2604.14475v1
date: 2026-04-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [clinical-agents, agent-reliability, self-evolving-agents, agentic-rl, agent-memory, arxiv, auto-ingested]
---

# Evo-MedAgent: Beyond One-Shot Diagnosis with Agents That Remember, Reflect, and Improve

**arXiv:** [2604.14475v1](https://arxiv.org/abs/2604.14475v1) · 2026-04-15 · cs.AI
**Authors:** Weixiang Shen, Bailiang Jian, Jun Li, Che Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Tool-augmented large language model (LLM) agents can orchestrate specialist classifiers, segmentation models, and visual question-answering modules to interpret chest X-rays. However, these agents still solve each case in isolation: they fail to accumulate experience across cases, correct recurrent reasoning mistakes, or adapt their tool-use behavior without expensive reinforcement learning. While a radiologist naturally improves with every case, current agents remain static. In this work, we propose Evo-MedAgent, a self-evolving memory module that equips a medical agent with the capacity for inter-case learning at test time. Our memory comprises three complementary stores: (1)~\emph{Retrospective Clinical Episodes} that retrieve problem-solving experiences from similar past cases, (2)~an \emph{Adaptive Procedural Heuristics} bank curating priority-tagged diagnostic rules that evolves via reflection, much like a physician refining their internal criteria, and (3)~a \emph{Tool Reliability Controller} that tracks per-tool trustworthiness. On ChestAgentBench, Evo-MedAgent raises multiple-choice question (MCQ) accuracy from 0.68 to 0.79 on GPT-5-mini, and from 0.76 to 0.87 on Gemini-3 Flash. With a strong base model, evolving memory improves performance more effectively than orchestrating external tools on qualitative diagnostic tasks. Because Evo-MedAgent requires no training, its per-case overhead is bounded by one additional retrieval pass and a single reflection call, making it deployable on top of any frozen model.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]]
- **Entities:** [[gpt-5]] · [[gemini]] · [[agentbench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.14475v1)
