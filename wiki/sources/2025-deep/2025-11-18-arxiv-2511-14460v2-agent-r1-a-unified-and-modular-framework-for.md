---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Agent-R1: A Unified and Modular Framework for Agentic Reinforcement Learning"
authors: Mingyue Cheng, Shuo Yu, Daoyu Wang, Qingchuan Li et al.
url: https://arxiv.org/abs/2511.14460v2
date: 2025-11-18
citationCount: 35
influentialCitationCount: 2
velocity: 4.93
ingested: 2026-06-22
tags: [agentic-rl, agent-memory, tool-use, agentic-ai, arxiv, 2025, cited]
---

# Agent-R1: A Unified and Modular Framework for Agentic Reinforcement Learning

**arXiv [2511.14460v2](https://arxiv.org/abs/2511.14460v2)** · 2025-11-18 · **35 citations** (2 influential · 4.93/mo) · Mingyue Cheng, Shuo Yu, Daoyu Wang, Qingchuan Li et al.

## Abstract
Large language models (LLMs) have rapidly evolved from single-turn text generators into the foundation of increasingly capable agents. As these agents take on more complex reasoning, decision making, tool use, and long-horizon tasks, reinforcement learning (RL) is becoming increasingly important for shaping their behavior. This shift is especially visible in agentic RL, where models must interact with tools and environments across multiple rounds rather than produce a single standalone response. In this regime, the usual view of a trajectory as one ever-growing token sequence becomes increasingly inadequate: it makes context evolution rigid and creates representation mismatches between rollout and training. This paper presents Agent-R1, a unified and modular framework for agentic RL built around step-level trajectory representation, flexible context management, and layered interfaces for workflows, environments and optimization. The key idea is to treat each interaction step as the basic reinforcement-learning transition, while keeping the optimization layer flexible: once the interaction is modeled at the step level, the framework can support token-level credit assignment, step-level credit assignment, or other compatible designs. These design choices make the framework compatible with a range of optimization strategies rather than tying it to a single algorithm. Together, these components provide a principled, extensible, and reusable substrate for agentic RL.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Preliminaries 2.1 Infrastructure for LLM Inference and Training 2.2 From Supervised LLM Training to RL Training 2.3 From Single-Turn LLM RL to Agentic RL 2.4 From LLMs to Agents: An MDP Perspective 3 Agent-R1 3.1 Overview of Agent-R1 3.2 Step-level Trajectory Representation 3.3 Flexible Context Management 4 Experiments 4.1 Experimental Setting 4.2 Different Application Scenarios 4.3 Different RL Algorithms 4.4 Context-Management Strategies 5 Future Directions 6 Limitation Discussion 7 Related Work 7.1 Agentic RL Algorithms 7.2 Agentic RL Training Frameworks 8 Conclusion References License: arXiv.org perpetual non-exclusive license arXiv:2511.14460v2 [cs.CL] 30 May 2026 \correspondence Agent-R1: A Unified and Modular Framework for Agentic Reinforcement Learning Mingyue Cheng, Shuo Yu, Daoyu Wang, Qingchuan Li, Xiaoyu Tao, Jie Ouyang, Yucong Luo, Yitong Zhou, Qi Liu, Enhong Chen State Key Laboratory of Cognitive Intelligence, University of Science and Technology of China mycheng@ustc.edu.cn…

**Method / approach.** methods such as PPO [ 23 ] and GRPO [ 25 ] . Compared with standard LLM training, the pipeline must now support sampling, reward computation, and replay in addition to optimization itself. As a result, LLM RL training is not just a new loss function layered on top of LLM training; it is a different end-to-end loop that must coordinate rollout and optimization. 2.3 From Single-Turn LLM RL to Agentic RL Figure 1 : Rollout in agentic RL. The agent repeatedly observes the current context, produces actions, and receives feedback from tools or environments, forming a multi-step trajectory rather than a single prompt-response pair. Figure 2 : Optimization in agentic RL. Interactive trajectories collected during rollout are replayed by the training loop and used to update the policy through reinforcement-learning objectives. Agentic RL extends this change one step further. In single-turn or short-horizon LLM RL, rollout still mostly takes the form of one prompt and one response. I…

**Results.** Experiments 4.1 Experimental Setting 4.2 Different Application Scenarios 4.3 Different RL Algorithms 4.4 Context-Management Strategies 5 Future Directions 6 Limitation Discussion 7 Related Work 7.1 Agentic RL Algorithms 7.2 Agentic RL Training Frameworks 8 Conclusion References License: arXiv.org perpetual non-exclusive license arXiv:2511.14460v2 [cs.CL] 30 May 2026 \correspondence Agent-R1: A Unified and Modular Framework for Agentic Reinforcement Learning Mingyue Cheng, Shuo Yu, Daoyu Wang, Qingchuan Li, Xiaoyu Tao, Jie Ouyang, Yucong Luo, Yitong Zhou, Qi Liu, Enhong Chen State Key Laboratory of Cognitive Intelligence, University of Science and Technology of China mycheng@ustc.edu.cn Abstract Large language models (LLMs) have rapidly evolved from single-turn text generators into the foundation of increasingly capable agents. As these agents take on more complex reasoning, decision…

**Conclusion.** Conclusion References License: arXiv.org perpetual non-exclusive license arXiv:2511.14460v2 [cs.CL] 30 May 2026 \correspondence Agent-R1: A Unified and Modular Framework for Agentic Reinforcement Learning Mingyue Cheng, Shuo Yu, Daoyu Wang, Qingchuan Li, Xiaoyu Tao, Jie Ouyang, Yucong Luo, Yitong Zhou, Qi Liu, Enhong Chen State Key Laboratory of Cognitive Intelligence, University of Science and Technology of China mycheng@ustc.edu.cn Abstract Large language models (LLMs) have rapidly evolved from single-turn text generators into the foundation of increasingly capable agents. As these agents take on more complex reasoning, decision making, tool use, and long-horizon tasks, reinforcement learning (RL) is becoming in…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2511.14460v2.md` · `raw/arxiv/2511.14460v2.fulltext.md`
