---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "OWL: Optimized Workforce Learning for General Multi-Agent Assistance in Real-World Task Automation"
authors: Mengkang Hu, Yuhang Zhou, Wendong Fan, Yuzhou Nie et al.
url: https://arxiv.org/abs/2505.23885v2
date: 2025-05-29
citationCount: 123
influentialCitationCount: 19
velocity: 9.62
ingested: 2026-06-22
tags: [agentic-rl, tool-use, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# OWL: Optimized Workforce Learning for General Multi-Agent Assistance in Real-World Task Automation

**arXiv [2505.23885v2](https://arxiv.org/abs/2505.23885v2)** · 2025-05-29 · **123 citations** (19 influential · 9.62/mo) · Mengkang Hu, Yuhang Zhou, Wendong Fan, Yuzhou Nie et al.

## Abstract
Large Language Model (LLM)-based multi-agent systems show promise for automating real-world tasks but struggle to transfer across domains due to their domain-specific nature. Current approaches face two critical shortcomings: they require complete architectural redesign and full retraining of all components when applied to new domains. We introduce Workforce, a hierarchical multi-agent framework that decouples strategic planning from specialized execution through a modular architecture comprising: (i) a domain-agnostic Planner for task decomposition, (ii) a Coordinator for subtask management, and (iii) specialized Workers with domain-specific tool-calling capabilities. This decoupling enables cross-domain transferability during both inference and training phases: During inference, Workforce seamlessly adapts to new domains by adding or modifying worker agents; For training, we introduce Optimized Workforce Learning (OWL), which improves generalization across domains by optimizing a domain-agnostic planner with reinforcement learning from real-world feedback. To validate our approach, we evaluate Workforce on the GAIA benchmark, covering various realistic, multi-domain agentic tasks. Experimental results demonstrate Workforce achieves open-source state-of-the-art performance (69.70%), outperforming commercial systems like OpenAI's Deep Research by 2.34%. More notably, our OWL-trained 32B model achieves 52.73% accuracy (+16.37%) and demonstrates performance comparable to GPT-4o on challenging tasks. To summarize, by enabling scalable generalization and modular domain transfer, our work establishes a foundation for the next generation of general-purpose AI assistants.

## From the paper (full-text excerpts)
**Introduction.** Introduction Large Language Models (LLMs) have undergone a period of rapid advancement, evolving from simple text predictors into powerful autonomous agents capable of planning, tool use, and multi-step reasoning [1, 21]. Recently, multi-agent systems (MAS) have emerged as a promising approach for complex real-world tasks, demonstrating that dividing tasks among specialized agents can enhance performance [16, 27, 38]. Although current MAS have yielded impressive results, their designs are typically domain-specific, severely restricting cross-domain transferability. This shortcoming appears in two forms: (i) First, on the inference side, deploying a system in a new domain often entails a full redesign; for instance, MetaGPT [13] depends on Standard Operating Procedures tailored to software engineering, hindering its extension to other fields. (ii) Second, on the training side, existing works often optimize every agent. MALT [20], for example, follows a fixed generator-verifier-refiner pipeline, necessitating separate training for every component. Consequently, migrating such systems…

**Method / approach.** method OWL significantly improves Qwen2.5-32B-Instruct’s performance by 16.37%. 3 Multi-Agent Inference: W ORKFORCE 3.1 W ORKFORCE Motivation. Contemporary multi-agent systems are critically limited by domain specificity and architectural rigidity, requiring complete redesign and retraining for each new application domain. We introduce W ORK FORCE, which addresses this fundamental challenge through modular architecture, particularly the separation of domain-agnostic planning from domain specific execution. More details about W ORKFORCE can be found in Appendix D. Architecture. As illustrated in Figure 3, W ORKFORCE comprises three core components: (i) Planner 4 Agent analyzes incoming tasks and decomposes them into subtasks based on worker capability registry; (ii) Coordinator Agent serves as the central orchestration mechanism, managing worker assignments and task dependencies while integrating intermediate results; (iii) Worker Nodes consist of one or more specialized agents…

**Results.** Experimental results demonstrate W ORKFORCE achieves open-source state-of-the-art performance (69.70%), outperforming commercial systems like OpenAI’s Deep Research by 2.34%. More notably, our OWL-trained 32B model achieves 52.73% accuracy (+16.37%) and demonstrates performance comparable to GPT-4o on challenging tasks. To summarize, by enabling scalable generalization and modular domain transfer, our work establishes a foundation for the next generation of general-purpose AI assistants. Date: May 26, 2025 Correspondence: Guohao Li at guohao.li@eigent.ai Project Page: https://github.com/camel-ai/owl 1 1 Introduction Large Language Models (LLMs) have undergone a period of rapid advancement, evolving from simple text predictors into powerful autonomous agents capable of planning, tool use, and multi-step reasoning [1, 21]. Recently, multi-agent systems (MAS) have emerged as a promising approach for complex real-world tasks, demonstra…

**Conclusion.** conclusions could be drawn from Table 1: (i) Workforce achieves state-of-the-art performance among open-source frameworks. Our W ORKFORCE achieves 69.70%, consistently outperforming previous open-source frameworks across all difficulty levels. Under strictly controlled settings with the same model and toolkits, our GPT-4o-based W ORKFORCE achieves 60.61% accuracy - 23.03% higher than the Single Agent and 6.06% higher than the multi-agent baseline Role Playing. (ii) Workforce demonstrates comparable or even superior performance relative to commercial proprietary frameworks. While previous open-source frameworks have exhibited a substantial performance gap compared to closed-source alternatives, W ORKFORCE considerably narrows this divide. To…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[gaia-benchmark]] · [[gpt-5]]
- **Raw:** `raw/arxiv/2505.23885v2.md` · `raw/arxiv/2505.23885v2.fulltext.md`
