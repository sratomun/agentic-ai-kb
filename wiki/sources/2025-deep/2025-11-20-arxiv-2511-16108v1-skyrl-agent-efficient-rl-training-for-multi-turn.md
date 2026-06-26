---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SkyRL-Agent: Efficient RL Training for Multi-turn LLM Agent"
authors: Shiyi Cao, Dacheng Li, Fangzhou Zhao, Shuo Yuan et al.
url: https://arxiv.org/abs/2511.16108v1
date: 2025-11-20
citationCount: 30
influentialCitationCount: 4
velocity: 4.27
ingested: 2026-06-22
tags: [coding-agents, computer-use-agents, embodied-agents, agentic-rl, agent-protocols, arxiv, 2025, cited]
---

# SkyRL-Agent: Efficient RL Training for Multi-turn LLM Agent

**arXiv [2511.16108v1](https://arxiv.org/abs/2511.16108v1)** · 2025-11-20 · **30 citations** (4 influential · 4.27/mo) · Shiyi Cao, Dacheng Li, Fangzhou Zhao, Shuo Yuan et al.

## Abstract
We introduce SkyRL-Agent, a framework for efficient, multi-turn, long-horizon agent training and evaluation. It provides efficient asynchronous dispatching, lightweight tool integration, and flexible backend interoperability, enabling seamless use with existing RL frameworks such as SkyRL-train, VeRL, and Tinker. Using SkyRL-Agent, we train SA-SWE-32B, a software engineering agent trained from Qwen3-32B (24.4% Pass@1) purely with reinforcement learning. We introduce two key components: an optimized asynchronous pipeline dispatcher that achieves a 1.55x speedup over naive asynchronous batching, and a tool-enhanced training recipe leveraging an AST-based search tool to facilitate code navigation, boost rollout Pass@K, and improve training efficiency. Together, these optimizations enable SA-SWE-32B to reach 39.4% Pass@1 on SWE-Bench Verified with more than 2x cost reduction compared to prior models reaching similar performance. Despite being trained solely on SWE tasks, SA-SWE-32B generalizes effectively to other agentic tasks, including Terminal-Bench, BrowseComp-Plus, and WebArena. We further demonstrate SkyRL-Agent's extensibility through case studies on deep research, computer use, and memory agents, each trained using a different training backend.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Background Multi-Turn LLM Agent Training. Training Frameworks for LLM Agents. 3 Framework Architecture 3.1 Tool-centric agent loop. 3.2 Fine‑grained heterogeneous scheduling via the dispatcher. 3.3 Connecting to training backends. 3.4 Error Handling 4 SWE Agent 4.1 Background 4.2 Training Recipe Bootstrapping training with better tools. RL algorithms and hyper-parameters. Hints for agent to recover and proceed. 4.3 Evaluations SWE-Bench Verified Terminal-Bench WebArena BrowseComp-Plus 5 Other Agents 5.1 Deep Research Experiment setup. 5.2 Memory Agent 5.3 Computer Use Agent Experiement Setup. Observations. SkyRL-Agent: Efficient RL Training for Multi-turn LLM Agent Shiyi Cao §∗ , Dacheng Li § , Fangzhou Zhao § † {}^{\S^{\dagger}} , Shuo Yuan § † {}^{\S^{\dagger}} , Sumanth R Hegde ¶ † {}^{\P^{\dagger}} , Connor Chen § † {}^{\S^{\dagger}} , Charlie Ruan § † {}^{\S^{\dagger}} , Tyler Griggs § , Shu Liu § , Eric Tang ¶ , Richard Liaw ¶ , Philipp Moritz ¶ , Matei Zaharia § , Joseph E…

**Method / approach.** method difficult to generalize beyond short, tool-integrated reasoning tasks. Building on the POMDP formulation, recent work instead adopts a more general transition-based data representation (Tan et al., 2025 ; Luo et al., 2025b ) , where each model invocation and its resulting feedback are represented as a tuple ( o t , a t , r t ) (o_{t},a_{t},r_{t}) . This representation supports flexible reward assignment and decouples learning from the details of agent execution and context management. It also naturally applies to multi-agent or sub-agent systems, where different policies interact within a shared environment. Training Frameworks for LLM Agents. Existing agent training frameworks such as VeRL-Tool (Jiang et al., 2025 ) , rLLM (Tan et al., 2025 ) , GEM (Liu et al., 2025c ) , and Agent-Lightning (Luo et al., 2025b ) have advanced large-scale RL training for LLM agents, yet remain limited by naive asynchronous batching (i.e., data-parallel) execution. SkyRL-Agent supp…

**Results.** Experiment setup. 5.2 Memory Agent 5.3 Computer Use Agent Experiement Setup. Observations. SkyRL-Agent: Efficient RL Training for Multi-turn LLM Agent Shiyi Cao §∗ , Dacheng Li § , Fangzhou Zhao § † {}^{\S^{\dagger}} , Shuo Yuan § † {}^{\S^{\dagger}} , Sumanth R Hegde ¶ † {}^{\P^{\dagger}} , Connor Chen § † {}^{\S^{\dagger}} , Charlie Ruan § † {}^{\S^{\dagger}} , Tyler Griggs § , Shu Liu § , Eric Tang ¶ , Richard Liaw ¶ , Philipp Moritz ¶ , Matei Zaharia § , Joseph E. Gonzalez § , Ion Stoica § NovaSky AI, § UC Berkeley, ¶ Anyscale GitHub: https://github.com/NovaSky-AI/SkyRL HuggingFace: https://huggingface.co/NovaSky-AI/SA-SWE-32B Co-lead the project. † Main Contributors. Abstract We introduce SkyRL-Agent , a framework for efficient, multi-turn, long-horizon agent training and evaluation. It provides efficient asynchronous dispatching, lightweight tool integration, and flexible backend intero…

**Conclusion.** discussion and feedback. References min (2025) The 100 line ai agent that solves github issues more. https://github.com/SWE-agent/mini-swe-agent , 2025. An et al. (2025) Chenxin An, Zhihui Xie, Xiaonan Li, Lei Li, Jun Zhang, Shansan Gong, Ming Zhong, Jingjing Xu, Xipeng Qiu, Mingxuan Wang, and Lingpeng Kong. Polaris: A post-training recipe for scaling reinforcement learning on advanced reasoning models, 2025. URL https://hkunlp.github.io/blog/2025/Polaris . AutoGen (2025) AutoGen. AutoGen. https://github.com/microsoft/autogen, 2025. Cao et al. (2025) Shiyi Cao, Sumanth Hegde, Dacheng Li, Tyler Griggs, Shu Liu, Eric Tang, Jiayi Pan, Xingyao Wang, Akshay Malik, Graham Neubig, Kourosh Hakhamaneshi, Richard Lia…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agentic-rl|Agentic RL]] · [[agent-protocols|Agent protocols]]
- **Entities:** [[swe-bench]] · [[webarena]] · [[qwen]]
- **Raw:** `raw/arxiv/2511.16108v1.md` · `raw/arxiv/2511.16108v1.fulltext.md`
