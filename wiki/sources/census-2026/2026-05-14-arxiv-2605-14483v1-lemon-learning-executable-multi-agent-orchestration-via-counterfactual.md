---
type: source
source_type: arxiv
title: "LEMON: Learning Executable Multi-Agent Orchestration via Counterfactual Reinforcement Learning"
authors: Xudong Chen, Yixin Liu, Hua Wei, Kaize Ding
url: https://arxiv.org/abs/2605.14483v1
date: 2026-05-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [agentic-rl, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# LEMON: Learning Executable Multi-Agent Orchestration via Counterfactual Reinforcement Learning

**arXiv:** [2605.14483v1](https://arxiv.org/abs/2605.14483v1) · 2026-05-14 · cs.AI
**Authors:** Xudong Chen, Yixin Liu, Hua Wei, Kaize Ding

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models (LLMs) have become a strong foundation for multi-agent systems, but their effectiveness depends heavily on orchestration design. Across different tasks, role design, capacity assignment, and dependency construction jointly affect both solution quality and execution efficiency. Existing approaches automate parts of this design process, yet they often optimize these decisions partially or sequentially, and rely on execution-level feedback that provides limited credit assignment for local orchestration decisions. We propose LEMON (\textbf{L}earning \textbf{E}xecutable \textbf{M}ulti-agent \textbf{O}rchestratio\textbf{N} via Counterfactual Reinforcement Learning), an LLM-based orchestrator that generates an executable orchestration specification. The specification integrates task-specific roles, customized duties, capacity levels, and dependency structure into a single deployable system. To train the orchestrator, we augment the orchestration-level GRPO objective with a localized counterfactual signal that edits role, capacity, or dependency fields and applies the resulting reward contrast only to the edited spans. Experiments on six reasoning and coding benchmarks, including MMLU, GSM8K, AQuA, MultiArith, SVAMP, and HumanEval, show that LEMON achieves state-of-the-art performance among the evaluated multi-agent orchestration methods. Our code is available at https://anonymous.4open.science/r/LEMON-B23C.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.14483v1)
