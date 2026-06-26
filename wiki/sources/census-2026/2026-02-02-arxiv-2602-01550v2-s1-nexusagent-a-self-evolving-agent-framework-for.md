---
type: source
source_type: arxiv
title: "S1-NexusAgent: a Self-Evolving Agent Framework for Multidisciplinary Scientific Research"
authors: S1-NexusAgent Team
url: https://arxiv.org/abs/2602.01550v2
date: 2026-02-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 25
primary: cs.AI
tags: [science-agents, self-evolving-agents, agent-protocols, agent-skills, agent-memory, arxiv, auto-ingested]
---

# S1-NexusAgent: a Self-Evolving Agent Framework for Multidisciplinary Scientific Research

**arXiv:** [2602.01550v2](https://arxiv.org/abs/2602.01550v2) · 2026-02-02 · cs.AI
**Authors:** S1-NexusAgent Team

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Modern scientific research relies on large-scale data, complex workflows, and specialized tools, which existing LLMs and tool-based agents struggle to handle due to limitations in long-horizon planning, robust goal maintenance, and continual learning from execution. To address these issues, in this work, we propose S1-NexusAgent, a self-evolving agent framework designed for multidisciplinary scientific research. S1-NexusAgent adopts a hierarchical Plan-and-CodeAct execution paradigm, decoupling global scientific planning from subtask-level tool execution through a dual-loop architecture, thereby enabling stable modeling of complex research workflows. The system natively supports the Model Context Protocol (MCP), integrates up to thousands of cross-disciplinary scientific tools, and achieves efficient orchestration of heterogeneous research tools via intention-aware dynamic tool retrieval and hot-plug mechanisms. To address long-context and large-scale data challenges in scientific settings, S1-NexusAgent introduces object-reference-based sparse context management, which enables sub-task context isolation and intermediate result compression. Building on this, a Critic Agent automatically evaluates complete execution trajectories and distills high-quality research paths into reusable Scientific Skills, forming a closed loop for continuous self-evolution, which is valuable for sustainable and long-horizon scientific research. Experiments on authoritative scientific benchmarks involving long-horizon planning and complex specialized tool orchestration, including biomini-eval (biology), ChemBench (chemistry), and MatSciBench (material science), demonstrate that S1-NexusAgent achieves state-of-the-art performance, validating its effectiveness and generalization capability in complex scientific tasks.

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-protocols|Agent protocols]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.01550v2)
