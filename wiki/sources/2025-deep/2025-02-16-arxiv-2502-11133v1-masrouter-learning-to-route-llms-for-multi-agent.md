---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MasRouter: Learning to Route LLMs for Multi-Agent Systems"
authors: Yanwei Yue, Guibin Zhang, Boyang Liu, Guancheng Wan et al.
url: https://arxiv.org/abs/2502.11133v1
date: 2025-02-16
citationCount: 63
influentialCitationCount: 4
velocity: 3.91
ingested: 2026-06-22
tags: [multi-agent-systems, agentic-ai, arxiv, 2025, cited]
---

# MasRouter: Learning to Route LLMs for Multi-Agent Systems

**arXiv [2502.11133v1](https://arxiv.org/abs/2502.11133v1)** · 2025-02-16 · **63 citations** (4 influential · 3.91/mo) · Yanwei Yue, Guibin Zhang, Boyang Liu, Guancheng Wan et al.

## Abstract
Multi-agent systems (MAS) powered by Large Language Models (LLMs) have been demonstrated to push the boundaries of LLM capabilities, yet they often incur significant costs and face challenges in dynamic LLM selection. Current LLM routing methods effectively reduce overhead in single-agent scenarios by customizing LLM selection for each query, but they overlook the critical decisions regarding collaboration modes and agent roles in MAS. In response to this challenge, we first introduce the problem of Multi-Agent System Routing (MASR), which integrates all components of MAS into a unified routing framework. Toward this goal, we propose MasRouter, the first high-performing, cost-effective, and inductive MASR solution. MasRouter employs collaboration mode determination, role allocation, and LLM routing through a cascaded controller network, progressively constructing a MAS that balances effectiveness and efficiency. Extensive experiments demonstrate that MasRouter is (1) high-performing, achieving a $1.8\%\sim8.2\%$ improvement over the state-of-the-art method on MBPP; (2) economical, reducing overhead by up to $52.07\%$ compared to SOTA methods on HumanEval; and (3) plug-and-play, seamlessly integrating with mainstream MAS frameworks, reducing overhead by $17.21\%\sim28.17\%$ via customized routing. The code is available at https://github.com/yanweiyue/masrouter.

## From the paper (full-text excerpts)
**Introduction.** Introduction Recent advances in Large Language Model (LLM) based agents (Park et al., 2023; Yao et al., 2023; Richards and et al., 2023) have demonstrated remarkable success across various tasks, including code generation (Wu et al., 2023; Guo et al., 2024), mathematical reasoning (Swan et al., 2023; Yu et al., 2024), and embodied actions (Wang et al., † Single Agent Routing These authors contributed equally. 1 the performance and cost of multiple LLMs, subsequently selecting the model that optimizes the trade-off between exploration and exploitation (Dai et al., 2024; Mohammadshahi et al., 2024; Feng et al., 2024). Although existing LLM routing methods (Hu et al., 2024a; Stripelis et al., 2024) have been proven effective in directing the most appropriate LLM for input queries, they are limited to single-agent scenarios (Wei et al., 2022; Shinn et al., 2023; Reworkd, 2023) yet not ready for MAS. However, we argue that the availability of a routing method for MAS is even more essential. On the performance perspective, multi-agent systems have been proven to outperform single-age…

**Method / approach.** methods effectively reduce overhead in single-agent scenarios by customizing LLM selection for each query, but they overlook the critical decisions regarding collaboration modes and agent roles in MAS. In response to this challenge, we first introduce the problem of Multi-Agent System Routing (MASR), which integrates all components of MAS into a unified routing framework. Toward this goal, we propose MasRouter, the first high-performing, cost-effective, and inductive MASR solution. MasRouter employs collaboration mode determination, role allocation, and LLM routing through a cascaded controller network, progressively constructing a MAS that balances effectiveness and efficiency. Extensive experiments demonstrate that MasRouter is (1) high-performing, achieving a 1.8% ∼ 8.2% improvement over the stateof-the-art method on MBPP; (2) economical, reducing overhead by up to 52.07% compared to SOTA methods on HumanEval; and (3) plugand-play, seamlessly integrating with mainstream MAS framewo…

**Results.** experiments demonstrate that MasRouter is (1) high-performing, achieving a 1.8% ∼ 8.2% improvement over the stateof-the-art method on MBPP; (2) economical, reducing overhead by up to 52.07% compared to SOTA methods on HumanEval; and (3) plugand-play, seamlessly integrating with mainstream MAS frameworks, reducing overhead by 17.21% ∼ 28.17% via customized routing. The code is available at https://github. com/yanweiyue/masrouter. 1 Multi Agent Routing 🤔 Query 🤔 Query LLM Router Collaboration Determiner Role Allocator 🖥️ Manager Star No one can do everything! I need help! LLM Router Programmer Programmer Manager 🧮 Scientist Physicist Scientist Physicist But everyone can do something! Figure 1: Paradigm comparison between single-agent routing and multi-agent routing. 2023). Building on the impressive capabilities of single agents, the LLM-based Multi-Agent System (MAS) has been proposed (Park et al., 2023; Du et al., 2023…

**Conclusion.** Conclusion In this paper, we for the first time introduce Multi-Agent System Routing (MASR), which aims to intelligently allocate collaboration patterns, agent roles, and LLMs for each query, thereby constructing a customized MAS. Based on this concept, we present MasRouter, the first highperforming, economical, and inductive MASR solution. MasRouter progressively builds a list of mutually adaptive roles, selects an LLM proficient 8 in the task domain, and ultimately achieves a balance between effectiveness and efficiency. We believe MasRouter paves the way for the automation, economization, and scalability of MAS, contributing to the development of large-scale collective intelligence. haiku and upgraded claude 3.5 sonnet. Technical rep…

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2502.11133v1.md` · `raw/arxiv/2502.11133v1.fulltext.md`
