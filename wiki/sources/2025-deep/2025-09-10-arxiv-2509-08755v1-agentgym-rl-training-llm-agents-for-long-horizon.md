---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "AgentGym-RL: Training LLM Agents for Long-Horizon Decision Making through Multi-Turn Reinforcement Learning"
authors: Zhiheng Xi, Jixuan Huang, Chenyang Liao, Baodai Huang et al.
url: https://arxiv.org/abs/2509.08755v1
date: 2025-09-10
citationCount: 54
influentialCitationCount: 6
velocity: 5.77
ingested: 2026-06-22
tags: [agentic-rl, agent-skills, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# AgentGym-RL: Training LLM Agents for Long-Horizon Decision Making through Multi-Turn Reinforcement Learning

**arXiv [2509.08755v1](https://arxiv.org/abs/2509.08755v1)** · 2025-09-10 · **54 citations** (6 influential · 5.77/mo) · Zhiheng Xi, Jixuan Huang, Chenyang Liao, Baodai Huang et al.

## Abstract
Developing autonomous LLM agents capable of making a series of intelligent decisions to solve complex, real-world tasks is a fast-evolving frontier. Like human cognitive development, agents are expected to acquire knowledge and skills through exploration and interaction with the environment. Despite advances, the community still lacks a unified, interactive reinforcement learning (RL) framework that can effectively train such agents from scratch -- without relying on supervised fine-tuning (SFT) -- across diverse and realistic environments. To bridge this gap, we introduce AgentGym-RL, a new framework to train LLM agents for multi-turn interactive decision-making through RL. The framework features a modular and decoupled architecture, ensuring high flexibility and extensibility. It encompasses a wide variety of real-world scenarios, and supports mainstream RL algorithms. Furthermore, we propose ScalingInter-RL, a training approach designed for exploration-exploitation balance and stable RL optimization. In early stages, it emphasizes exploitation by restricting the number of interactions, and gradually shifts towards exploration with larger horizons to encourage diverse problem-solving strategies. In this way, the agent develops more diverse behaviors and is less prone to collapse under long horizons. We perform extensive experiments to validate the stability and effectiveness of both the AgentGym-RL framework and the ScalingInter-RL approach. Our agents match or surpass commercial models on 27 tasks across diverse environments. We offer key insights and will open-source the complete AgentGym-RL framework -- including code and datasets -- to empower the research community in developing the next generation of intelligent agents.

## From the paper (full-text excerpts)
**Introduction.** Introduction As Large Language Models (LLMs) have largely developed [2, 11, 41, 65, 84], their applications have extended from chatbots to autonomous agents that can handle long-horizon real-world tasks [39, 79]. Given a complex task, these agents interact with the environment, making a series of intelligent decisions to achieve the goal [95]. Analogous to human cognitive development, LLM agents are expected to acquire new knowledge and skills by actively exploring and interacting with the environment [42, 77]. Therefore, a natural approach is to train these agents using Reinforcement Learning (RL) [62]. Despite the progress of RL in areas like LLM reasoning [12, 18, 23, 66, 68, 76], most existing studies are restricted to single-turn tasks, where models are not required to engage in multi-turn interaction with complex environments [71]. While some recent efforts have attempted to extend RL to train LLM agents with multi-turn capabilities [3, 26, 30, 47, 71, 95], these works are limited in task complexity and environment diversity. Furthermore, they struggle with optimization stabil…

**Method / approach.** method substantially enhances the open-sourced 7B-scale models’ capabilities to a level that rivals or even surpasses top-tier proprietary large models. 1 Introduction As Large Language Models (LLMs) have largely developed [2, 11, 41, 65, 84], their applications have extended from chatbots to autonomous agents that can handle long-horizon real-world tasks [39, 79]. Given a complex task, these agents interact with the environment, making a series of intelligent decisions to achieve the goal [95]. Analogous to human cognitive development, LLM agents are expected to acquire new knowledge and skills by actively exploring and interacting with the environment [42, 77]. Therefore, a natural approach is to train these agents using Reinforcement Learning (RL) [62]. Despite the progress of RL in areas like LLM reasoning [12, 18, 23, 66, 68, 76], most existing studies are restricted to single-turn tasks, where models are not required to engage in multi-turn interaction with complex environmen…

**Results.** experiments to validate the stability and effectiveness of both the AgentGym-RL framework and ScalingInter-RL approach. Our agents match or surpass commercial models on 27 tasks across diverse environments. We offer key insights and will open-source complete AgentGym-RL framework—including code and datasets—to empower the research community in developing the next generation of intelligent agents. Correspondence: zhxi22@m.fudan.edu.cn, tgui@fudan.edu.cn, qz@fudan.edu.cn Code: https://github.com/woooodyy/AgentGym-RL Project: https://AgentGym-RL.github.io 1 60 91.0 Overall Accuracy (%) Average Success Rate / Percentile (%) 100 96.7 90 80 70 60 50 40 30 20 10 0 BabyAI 57.0 38.2 26.0 TextCraft Ours-7B Qwen2.5-3B Qwen2.5-7B Qwen2.5-72B Qwen3-4B Qwen3-8B Qwen3-32B Qwen3-235B-A22B Llama3.1-8B Llama3.1-70B SciWorld WebArena DeepSeek-V3 DeepSeek-R1 Gemini-2.5-Flash Gemini-2.5-Pro Qwen-Max Deep Search GPT-4o OpenAI o4-mini OpenAI o…

**Conclusion.** discussion forums, collaborative development, and business content management; for deep search, we include a RAG-based environment [19, 26, 28, 32, 38, 46, 67, 85] which enables LLMs to interact with search engines and solve multi-turn retrieval and reasoning tasks; for digital games, we include TextCraft [45], a text-based crafting game environment in which agents complete tasks via natural language interactions and task-based planning; for embodied tasks, we include BabyAI [7] which provides a controllable grid world with text instructions for embodied reasoning in simulated environments; for scientific tasks, we include SciWorld [69] which offers a scientific exploration simulator where agents conduct scientific experiments through text-…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2509.08755v1.md` · `raw/arxiv/2509.08755v1.fulltext.md`
