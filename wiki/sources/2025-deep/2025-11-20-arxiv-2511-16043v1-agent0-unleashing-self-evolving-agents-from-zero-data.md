---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Agent0: Unleashing Self-Evolving Agents from Zero Data via Tool-Integrated Reasoning"
authors: Peng Xia, Kaide Zeng, Jiaqi Liu, Can Qin et al.
url: https://arxiv.org/abs/2511.16043v1
date: 2025-11-20
citationCount: 42
influentialCitationCount: 1
velocity: 5.97
ingested: 2026-06-22
tags: [self-evolving-agents, agentic-rl, tool-use, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Agent0: Unleashing Self-Evolving Agents from Zero Data via Tool-Integrated Reasoning

**arXiv [2511.16043v1](https://arxiv.org/abs/2511.16043v1)** · 2025-11-20 · **42 citations** (1 influential · 5.97/mo) · Peng Xia, Kaide Zeng, Jiaqi Liu, Can Qin et al.

## Abstract
Large Language Model (LLM) Agents, often trained with Reinforcement Learning (RL), are constrained by a dependency on human-curated data, limiting scalability and tethering AI to human knowledge. Existing self-evolution frameworks offer an alternative but are typically restricted by the model's inherent capabilities and single-round interactions, hindering the development of complex curricula involving tool use or dynamic reasoning. We introduce Agent0, a fully autonomous framework that evolves high-performing agents without external data through multi-step co-evolution and seamless tool integration. Agent0 establishes a symbiotic competition between two agents initialized from the same base LLM: a curriculum agent that proposes increasingly challenging frontier tasks, and an executor agent that learns to solve them. We integrate external tools to enhance the executor's problem-solving capacity; this improvement, in turn, pressures the curriculum agent to construct more complex, tool-aware tasks. Through this iterative process, Agent0 establishes a self-reinforcing cycle that continuously produces high-quality curricula. Empirically, Agent0 substantially boosts reasoning capabilities, improving the Qwen3-8B-Base model by 18% on mathematical reasoning and 24% on general reasoning benchmarks. Code is available at https://github.com/aiming-lab/Agent0.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Preliminaries 3 The Agent0 Framework 3.1 Framework Overview 3.2 Curriculum Agent Training 3.3 Executor Agent Training 3.3.1 Dataset Curation and Trajectory Generation 3.3.2 Ambiguity-Dynamic Policy Optimization 4 Experiments 4.1 Experimental Setup 4.2 Main Results 4.3 Analysis 5 Related Work 6 Conclusion A Experimental Details A.1 Hyperparameter Settings A.2 Prompt A.3 Sandbox Configuration B Overview of the Baselines C Evaluation Benchmarks D Additional Results and Analysis D.1 The Impact of the Number of Turns on Performance D.2 Detailed Results E Case Analysis Agent0 : Unleashing Self-Evolving Agents from Zero Data via Tool-Integrated Reasoning Peng Xia Kaide Zeng Jiaqi Liu Can Qin Fang Wu Yiyang Zhou Caiming Xiong Huaxiu Yao Abstract Large Language Model (LLM) Agents, often trained with Reinforcement Learning (RL), are constrained by a dependency on human-curated data, limiting scalability and tethering AI to human knowledge. Existing self-evolution frameworks offer an alte…

**Method / approach.** methods, whether Reinforcement Learning from Human Feedback (RLHF) or Reinforcement Learning from Verifiable Rewards (RLVR), relies heavily on massive, high-quality, human-curated datasets (Zhang et al., 2025c ) . This dependency not only creates a severe scalability bottleneck (Yue et al., 2025 ) , which is time-consuming, labor-intensive, and costly, but also fundamentally tethers the potential of AI to the limits of human knowledge and annotation speed. To break free from this reliance on human data, self-evolution frameworks have emerged as a promising alternative (Zhao et al., 2025 ; Liu et al., 2025a ; Huang et al., 2025 ; Wang et al., 2025d ) , offering a scalable pathway by enabling models to autonomously generate their own training data. Yet, despite their potential, existing self-play or self-challenging approaches face severe constraints. First, their capabilities are capped by the model’s inherent knowledge and reasoning abilities (Fang et al., 2025 ; Cheng et al.,…

**Results.** Experiments 4.1 Experimental Setup 4.2 Main Results 4.3 Analysis 5 Related Work 6 Conclusion A Experimental Details A.1 Hyperparameter Settings A.2 Prompt A.3 Sandbox Configuration B Overview of the Baselines C Evaluation Benchmarks D Additional Results and Analysis D.1 The Impact of the Number of Turns on Performance D.2 Detailed Results E Case Analysis Agent0 : Unleashing Self-Evolving Agents from Zero Data via Tool-Integrated Reasoning Peng Xia Kaide Zeng Jiaqi Liu Can Qin Fang Wu Yiyang Zhou Caiming Xiong Huaxiu Yao Abstract Large Language Model (LLM) Agents, often trained with Reinforcement Learning (RL), are constrained by a dependency on human-curated data, limiting scalability and tethering AI to human knowledge. Existing self-evolution frameworks offer an alternative but are typically restricted by the model’s inherent capabilities and single-round interactions…

**Conclusion.** Conclusion A Experimental Details A.1 Hyperparameter Settings A.2 Prompt A.3 Sandbox Configuration B Overview of the Baselines C Evaluation Benchmarks D Additional Results and Analysis D.1 The Impact of the Number of Turns on Performance D.2 Detailed Results E Case Analysis Agent0 : Unleashing Self-Evolving Agents from Zero Data via Tool-Integrated Reasoning Peng Xia Kaide Zeng Jiaqi Liu Can Qin Fang Wu Yiyang Zhou Caiming Xiong Huaxiu Yao Abstract Large Language Model (LLM) Agents, often trained with Reinforcement Learning (RL), are constrained by a dependency on human-curated data, limiting scalability and tethering AI to human knowledge. Existing self-evolution frameworks offer an al…

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[qwen]]
- **Raw:** `raw/arxiv/2511.16043v1.md` · `raw/arxiv/2511.16043v1.fulltext.md`
