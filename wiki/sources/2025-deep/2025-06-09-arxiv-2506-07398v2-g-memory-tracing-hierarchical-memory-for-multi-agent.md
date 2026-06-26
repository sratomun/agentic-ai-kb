---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "G-Memory: Tracing Hierarchical Memory for Multi-Agent Systems"
authors: Guibin Zhang, Muxin Fu, Guancheng Wan, Miao Yu et al.
url: https://arxiv.org/abs/2506.07398v2
date: 2025-06-09
citationCount: 64
influentialCitationCount: 7
velocity: 5.15
ingested: 2026-06-22
tags: [embodied-agents, agent-memory, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# G-Memory: Tracing Hierarchical Memory for Multi-Agent Systems

**arXiv [2506.07398v2](https://arxiv.org/abs/2506.07398v2)** · 2025-06-09 · **64 citations** (7 influential · 5.15/mo) · Guibin Zhang, Muxin Fu, Guancheng Wan, Miao Yu et al.

## Abstract
Large language model (LLM)-powered multi-agent systems (MAS) have demonstrated cognitive and execution capabilities that far exceed those of single LLM agents, yet their capacity for self-evolution remains hampered by underdeveloped memory architectures. Upon close inspection, we are alarmed to discover that prevailing MAS memory mechanisms (1) are overly simplistic, completely disregarding the nuanced inter-agent collaboration trajectories, and (2) lack cross-trial and agent-specific customization, in stark contrast to the expressive memory developed for single agents. To bridge this gap, we introduce G-Memory, a hierarchical, agentic memory system for MAS inspired by organizational memory theory, which manages the lengthy MAS interaction via a three-tier graph hierarchy: insight, query, and interaction graphs. Upon receiving a new user query, G-Memory performs bi-directional memory traversal to retrieve both $\textit{high-level, generalizable insights}$ that enable the system to leverage cross-trial knowledge, and $\textit{fine-grained, condensed interaction trajectories}$ that compactly encode prior collaboration experiences. Upon task execution, the entire hierarchy evolves by assimilating new collaborative trajectories, nurturing the progressive evolution of agent teams. Extensive experiments across five benchmarks, three LLM backbones, and three popular MAS frameworks demonstrate that G-Memory improves success rates in embodied action and accuracy in knowledge QA by up to $20.89\%$ and $10.12\%$, respectively, without any modifications to the original frameworks. Our codes are available at https://github.com/bingreeky/GMemory.

## From the paper (full-text excerpts)
**Introduction.** Introduction As Large Language Models (LLMs) continue to redefine the frontier of artificial intelligence, LLMdriven agents have exhibited unprecedented prowess in perception [2, 3, 4, 5], planning [6, 7, 8], reasoning [9, 10], and action [11, 12], which have catalyzed remarkable progress across diverse downstream domains, including code generation [13, 14], data analysis [15], embodied tasks [16] and autonomous driving [3, 17, 18]. Building upon the impressive competencies of single agents, LLMbased Multi-Agent Systems (MAS) have been demonstrated to push the boundaries of single model capacity [19, 20, 21]. Similar to collective intelligence arising from human social collaboration [22, 23, 24], MAS orchestrates multiple agents [25, 26, 27], whether through cooperation [28, 29, 30, 31] or competition [32, 33, 34], to transcend the cognitive and specialized limitations of solitary agents. Self-Evolving Agents. What especially characterizes LLM agents is their self-evolving capacity, i.e., the ability to continuously adapt and improve through interactions with the environment, as see…

**Method / approach.** methods to provide agent role-specific memory support, which is essential in the PDDL strategic game tasks, where effective division of labor is critical to success. Even MAS-oriented designs, such as ChatDev-M, result in a 2.32% performance drop when applied to MacNet+SciWorld. We attribute this to ChatDev-M’s narrow memory scope—storing only the execution results of past queries, which provides limited utility in embodied action environments. These findings highlight the necessity of G-Memory’s core characteristics: role-specific memory cues, abstracted high-level insights, and trajectory condensation—all of which are critical for effective memory in MAS. 5.3 Cost Analysis (RQ2) To evaluate the efficiency of G-Memory in terms of token consumption, we visualize the performance versus token cost trade-off across various settings, as shown in Figures 3 and 7. Our findings are: Takeaway ➌: G-Memory achieves high-performing collective memory without excessive token consumption. As depict…

**Results.** experiments across five benchmarks, three LLM backbones, and three popular MAS frameworks demonstrate that G-Memory improves success rates in embodied action and accuracy in knowledge QA by up to 20.89% and 10.12%, respectively, without any modifications to the original frameworks. Our codes are available at https://github.com/bingreeky/GMemory. 1 Introduction As Large Language Models (LLMs) continue to redefine the frontier of artificial intelligence, LLMdriven agents have exhibited unprecedented prowess in perception [2, 3, 4, 5], planning [6, 7, 8], reasoning [9, 10], and action [11, 12], which have catalyzed remarkable progress across diverse downstream domains, including code generation [13, 14], data analysis [15], embodied tasks [16] and autonomous driving [3, 17, 18]. Building upon the impressive competencies of single agents, LLMbased Multi-Agent Systems (MAS) have been demonstrated to push the boundaries of single model cap…

**Conclusion.** conclusion on ... Status Insight Graph Check whether there are more than two oranges on the table of the kitchen? Execution fail! Query Graph I found 2 apples, 1 orange. The answer now is YES! Interaction Graph Figure 1: (Left) We report the token cost of several single-agent and MAS baselines on ALFWorld benchmark; (Right) The overview of G-Memory’s three-tier hierarchical memory architecture, encompassing the insight graph, query graph and interaction (utterance) graph. retrieve relevant information. Previous successful memory mechanism designs, including both inside-trial memory (i.e., context retained within solving one single query) and cross-trial memory (i.e., experience accumulated across multiple tasks) [39], have empowered…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2506.07398v2.md` · `raw/arxiv/2506.07398v2.fulltext.md`
