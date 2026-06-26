---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "The Landscape of Agentic Reinforcement Learning for LLMs: A Survey"
authors: Guibin Zhang, Hejia Geng, Xiaohang Yu, Zhenfei Yin et al.
url: https://arxiv.org/abs/2509.02547v5
date: 2025-09-02
citationCount: 152
influentialCitationCount: 4
velocity: 15.79
ingested: 2026-06-22
tags: [self-evolving-agents, agentic-rl, agent-memory, tool-use, agent-evaluation, arxiv, 2025, cited]
---

# The Landscape of Agentic Reinforcement Learning for LLMs: A Survey

**arXiv [2509.02547v5](https://arxiv.org/abs/2509.02547v5)** · 2025-09-02 · **152 citations** (4 influential · 15.79/mo) · Guibin Zhang, Hejia Geng, Xiaohang Yu, Zhenfei Yin et al.

## Abstract
The emergence of agentic reinforcement learning (Agentic RL) marks a paradigm shift from conventional reinforcement learning applied to large language models (LLM RL), reframing LLMs from passive sequence generators into autonomous, decision-making agents embedded in complex, dynamic worlds. This survey formalizes this conceptual shift by contrasting the degenerate single-step Markov Decision Processes (MDPs) of LLM-RL with the temporally extended, partially observable Markov decision processes (POMDPs) that define Agentic RL. Building on this foundation, we propose a comprehensive twofold taxonomy: one organized around core agentic capabilities, including planning, tool use, memory, reasoning, self-improvement, and perception, and the other around their applications across diverse task domains. Central to our thesis is that reinforcement learning serves as the critical mechanism for transforming these capabilities from static, heuristic modules into adaptive, robust agentic behavior. To support and accelerate future research, we consolidate the landscape of open-source environments, benchmarks, and frameworks into a practical compendium. By synthesizing over five hundred recent works, this survey charts the contours of this rapidly evolving field and highlights the opportunities and challenges that will shape the development of scalable, general-purpose AI agents.

## From the paper (full-text excerpts)
**Introduction.** Introduction Synergy between RL and LLMs LLM Agents. Research Gap and Our Contributions. Structure of the Survey. 2 Preliminary: From LLM RL to Agentic RL 2.1 Markov Decision Processes PBRFT. Agentic RL. 2.2 Environment State PBRFT. Agentic RL. 2.3 Action Space 2.4 Transition Dynamics PBRFT. Agentic RL. 2.5 Reward Function PBRFT. Agentic RL. 2.6 Learning Objective PBRFT. Agentic RL. 2.7 RL Algorithms REINFORCE: The Foundational Policy Gradient Proximal Policy Optimization (PPO) Direct Preference Optimization (DPO) Group Relative Policy Optimization (GRPO) 3 Agentic RL: The model capability perspective 3.1 Planning RL as an External Guide for Planning. RL as an Internal Driver of Planning. Prospective: The Synthesis of Deliberation and Intuition. 3.2 Tool Using ReAct-style Tool Calling. Tool-integrated RL. Prospective: Long-horizon TIR. 3.3 Memory RL in RAG-style Memory. RL for Token-level Memory. Prospective: RL for Structured Memory. 3.4 Self-Improvement RL for Verba…

**Method / approach.** Methods Search from the external Internet Search from LLM internal knowledge 4.1.2 Closed Source RL Methods Industrial Research Agents. Case Study: OpenAI Deep Research. 4.2 Code Agent 4.2.1 RL for Code Generation Outcome reward RL. Process reward RL. 4.2.2 RL for Iterative Code Refinement Outcome reward RL. Process reward RL. 4.2.3 RL for Automated Software Engineering Outcome reward RL. Process reward RL. Remark on closed-source systems. 4.2.4 Emerging Paradigms Code World Models 4.3 Mathematical Agent 4.3.1 RL for Informal Mathematical Reasoning Outcome reward RL. Process reward RL. 4.3.2 RL for Formal Mathematical Reasoning Outcome reward RL. Process reward RL. Hybrid reward RL. 4.4 GUI Agent 4.4.1 RL-free Methods Vanilla VLM-based GUI Agents Supervised Fine-Tuning (SFT) with Static Trajectory Data 4.4.2 RL in Static GUI Environments 4.4.3 RL in Interactive GUI Environments 4.5 Vision…

**Results.** experimentation and benchmarking. Section 6 discusses open challenges and future directions towards scalable, adaptive, and reliable agentic intelligence, and Section 7 concludes the survey. The overall structure is also illustrated in Figure 1 . {forest} Figure 1 : The primary organizational structure of the survey. 2 Preliminary: From LLM RL to Agentic RL LLMs are initially pre-trained using behavior cloning, which applies maximum likelihood estimation (MLE) to static datasets such as web-scraped text corpora. Subsequent post-training methods enhance capabilities and align outputs with human preferences—transforming them beyond generic web-data replicators. A common technique is supervised fine-tuning (SFT), where models are refined on human-generated (prompt, response) demonstrations. However, procuring sufficient high-quality SFT data remains challenging (Maosongcao et al. , 2025 ; Szep et al. , 2025 ; Han et al. ,…

**Conclusion.** Conclusion References License: CC BY 4.0 arXiv:2509.02547v5 [cs.AI] 17 Apr 2026 The Landscape of Agentic Reinforcement Learning for LLMs: A Survey Guibin Zhang 3† Hejia Geng 1† Xiaohang Yu 8† Zhenfei Yin 1∗ Zaibin Zhang 9,1 Zelin Tan 7,2 Heng Zhou 7,2 Zhongzhi Li 10 Xiangyuan Xue 11,2 Yijiang Li 13 Yifan Zhou 12 Yang Chen 2 Chen Zhang 7 Yutao Fan 2 Zihu Wang 14 Songtao Huang 6,2 Piedrahita-Velez, Francisco 5 Yue Liao 3 Hongru Wang 11 Mengyue Yang 15 Heng Ji 4 Jun Wang 6 Shuicheng Yan 3 Philip Torr 1 Lei Bai 2∗ 1 University of Oxford 2 Shanghai AI Laboratory 3 National University of Singapore 4 University of Illinois Urbana-Champaign 5 Brown University 6 University College London 7 U…

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2509.02547v5.md` · `raw/arxiv/2509.02547v5.fulltext.md`
