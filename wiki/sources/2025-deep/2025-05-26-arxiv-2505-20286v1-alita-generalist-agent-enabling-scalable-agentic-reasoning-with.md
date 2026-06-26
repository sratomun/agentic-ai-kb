---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Alita: Generalist Agent Enabling Scalable Agentic Reasoning with Minimal Predefinition and Maximal Self-Evolution"
authors: Jiahao Qiu, Xuan Qi, Tongcheng Zhang, Xinzhe Juan et al.
url: https://arxiv.org/abs/2505.20286v1
date: 2025-05-26
citationCount: 99
influentialCitationCount: 8
velocity: 7.69
ingested: 2026-06-22
tags: [agent-protocols, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Alita: Generalist Agent Enabling Scalable Agentic Reasoning with Minimal Predefinition and Maximal Self-Evolution

**arXiv [2505.20286v1](https://arxiv.org/abs/2505.20286v1)** · 2025-05-26 · **99 citations** (8 influential · 7.69/mo) · Jiahao Qiu, Xuan Qi, Tongcheng Zhang, Xinzhe Juan et al.

## Abstract
Recent advances in large language models (LLMs) have enabled agents to autonomously perform complex, open-ended tasks. However, many existing frameworks depend heavily on manually predefined tools and workflows, which hinder their adaptability, scalability, and generalization across domains. In this work, we introduce Alita--a generalist agent designed with the principle of "Simplicity is the ultimate sophistication," enabling scalable agentic reasoning through minimal predefinition and maximal self-evolution. For minimal predefinition, Alita is equipped with only one component for direct problem-solving, making it much simpler and neater than previous approaches that relied heavily on hand-crafted, elaborate tools and workflows. This clean design enhances its potential to generalize to challenging questions, without being limited by tools. For Maximal self-evolution, we enable the creativity of Alita by providing a suite of general-purpose components to autonomously construct, refine, and reuse external capabilities by generating task-related model context protocols (MCPs) from open source, which contributes to scalable agentic reasoning. Notably, Alita achieves 75.15% pass@1 and 87.27% pass@3 accuracy, which is top-ranking among general-purpose agents, on the GAIA benchmark validation dataset, 74.00% and 52.00% pass@1, respectively, on Mathvista and PathVQA, outperforming many agent systems with far greater complexity. More details will be updated at $\href{https://github.com/CharlesQ9/Alita}{https://github.com/CharlesQ9/Alita}$.

## From the paper (full-text excerpts)
**Introduction.** Introduction — Leonardo da Vinci "Simplicity is the ultimate sophistication." Large language models (LLMs) have rapidly evolved from merely generating text to autonomous agents capable of independently planning and executing complex tasks on behalf of users with limited human oversight [2]. These capabilities have enabled a wide range of applications, ranging from travel planning [3], computer use [4, 5, 6], to the multi-step research tasks [7]. To support such diverse and demanding tasks, a new class of systems called generalist agents has emerged. These agents are designed to handle a wide range of domains and tasks through a unified architecture, allowing them to generalize beyond task-specific solutions, such as OpenAI Deep Research [1] and Manus. However, most of the current general-purpose agents heavily rely on large-scale manual engineering, including tediously designed workflows, considerable pre-defined tools, and hardcoded components [8, 9]. This reliance introduces several critical limitations: i) It is impractical, if not impossible, to predefine all the tools required…

**Method / approach.** method that decomposes complex tasks into subtasks and dynamically allocates them to worker nodes with specialized toolkits. Omne [11] proposes a multiagent collaborative development framework, where each agent possesses an independent system structure, enabling autonomous learning and the storage of a comprehensive world model to build an independent understanding of the environment. OpenAI Deep Research2 employs reinforcement learning for training on real-world tasks, aiming to provide precise and reliable research reports for knowledge-intensive tasks. A-World [12] offers a highly configurable, modular, and scalable simulation environment, allowing developers to flexibly define and integrate different types of AI agents. The Magentic-One [13] framework merges the Magentic and Autogen systems, distinguishing between the micro-level LLM-driven function generation and the macro-level multi-agent orchestration, resulting in a clearer and more efficient construction of agent systems. Al…

**Results.** experiments on several benchmarks to assess Alita in real-world applications, especially on the most popular GAIA [10]. Alita proves that simplicity is not a constraint, but a strength, and that creative agent behavior can emerge from a design that prioritizes autonomy over manual engineering. To sum up, our key contributions can be summarized as follows. • We propose a new agent architecture centered on minimal predefinition and maximal self-evolution, challenging conventional design norms in generalist agents, aiming to call for a more scalable and generalizable agent framework. 1 https://www.anthropic.com/news/model-context-protocol 2 • We present Alita, a generalist agent that achieves scalable agentic reasoning with a radically simple design. • We empirically demonstrate that Alita, despite using no complex predefined tools and workflows for specific tasks, outperforms many systems with significantly more handcrafted complexity…

**Conclusion.** Conclusion In this work, we introduced Alita, a generalist agent designed with the principles of minimal predefinition and maximal self-evolution. By significantly reducing reliance on manually predefined tools and workflows for direct solving, Alita leverages creative, autonomous capabilities in real time, facilitating scalable agentic reasoning. Our approach demonstrates that simplicity in design does not undermine, but rather enhances, the performance and adaptability of generalist agents. 9 References [1] OpenAI. Introducing deep research. [2] Noam Kolt. Governing ai agents. arXiv preprint arXiv:2501.07913, 2025. [3] Jian Xie, Kai Zhang, Jiangjie Chen, Tinghui Zhu, Renze Lou, Yuandong Tian, Yanghua Xiao, and Yu Su. Travelplanner: A…

## Graph
- **Concepts:** [[agent-protocols|Agent protocols]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[mcp]] · [[gaia-benchmark]]
- **Raw:** `raw/arxiv/2505.20286v1.md` · `raw/arxiv/2505.20286v1.fulltext.md`
