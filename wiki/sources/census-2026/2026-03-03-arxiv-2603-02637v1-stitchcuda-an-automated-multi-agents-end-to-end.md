---
type: source
source_type: arxiv
title: "StitchCUDA: An Automated Multi-Agents End-to-End GPU Programing Framework with Rubric-based Agentic Reinforcement Learning"
authors: Shiyang Li, Zijian Zhang, Winson Chen, Yuebo Luo et al.
url: https://arxiv.org/abs/2603.02637v1
date: 2026-03-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 24
primary: cs.MA
tags: [coding-agents, agentic-rl, agent-skills, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# StitchCUDA: An Automated Multi-Agents End-to-End GPU Programing Framework with Rubric-based Agentic Reinforcement Learning

**arXiv:** [2603.02637v1](https://arxiv.org/abs/2603.02637v1) · 2026-03-03 · cs.MA
**Authors:** Shiyang Li, Zijian Zhang, Winson Chen, Yuebo Luo et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Modern machine learning (ML) workloads increasingly rely on GPUs, yet achieving high end-to-end performance remains challenging due to dependencies on both GPU kernel efficiency and host-side settings. Although LLM-based methods show promise on automated GPU kernel generation, prior works mainly focus on single-kernel optimization and do not extend to end-to-end programs, hindering practical deployment. To address the challenge, in this work, we propose StitchCUDA, a multi-agent framework for end-to-end GPU program generation, with three specialized agents: a Planner to orchestrate whole system design, a Coder dedicated to implementing it step-by-step, and a Verifier for correctness check and performance profiling using Nsys/NCU. To fundamentally improve the Coder's ability in end-to-end GPU programming, StitchCUDA integrates rubric-based agentic reinforcement learning over two atomic skills, task-to-code generation and feedback-driven code optimization, with combined rubric reward and rule-based reward from real executions. Therefore, the Coder learns how to implement advanced CUDA programming techniques (e.g., custom kernel fusion, cublas epilogue), and we also effectively prevent Coder's reward hacking (e.g., just copy PyTorch code or hardcoding output) during benchmarking. Experiments on KernelBench show that StitchCUDA achieves nearly 100% success rate on end-to-end GPU programming tasks, with 1.72x better speedup over the multi-agent baseline and 2.73x than the RL model baselines.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-rl|Agentic RL]] · [[agent-skills|Agent skills]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.02637v1)
