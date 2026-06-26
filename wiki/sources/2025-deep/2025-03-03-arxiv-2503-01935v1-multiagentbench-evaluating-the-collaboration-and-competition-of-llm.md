---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MultiAgentBench: Evaluating the Collaboration and Competition of LLM agents"
authors: Kunlun Zhu, Hongyi Du, Zhaochen Hong, Xiaocheng Yang et al.
url: https://arxiv.org/abs/2503.01935v1
date: 2025-03-03
citationCount: 125
influentialCitationCount: 7
velocity: 7.99
ingested: 2026-06-22
tags: [multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# MultiAgentBench: Evaluating the Collaboration and Competition of LLM agents

**arXiv [2503.01935v1](https://arxiv.org/abs/2503.01935v1)** · 2025-03-03 · **125 citations** (7 influential · 7.99/mo) · Kunlun Zhu, Hongyi Du, Zhaochen Hong, Xiaocheng Yang et al.

## Abstract
Large Language Models (LLMs) have shown remarkable capabilities as autonomous agents, yet existing benchmarks either focus on single-agent tasks or are confined to narrow domains, failing to capture the dynamics of multi-agent coordination and competition. In this paper, we introduce MultiAgentBench, a comprehensive benchmark designed to evaluate LLM-based multi-agent systems across diverse, interactive scenarios. Our framework measures not only task completion but also the quality of collaboration and competition using novel, milestone-based key performance indicators. Moreover, we evaluate various coordination protocols (including star, chain, tree, and graph topologies) and innovative strategies such as group discussion and cognitive planning. Notably, gpt-4o-mini reaches the average highest task score, graph structure performs the best among coordination protocols in the research scenario, and cognitive planning improves milestone achievement rates by 3%. Code and datasets are public available at https://github.com/MultiagentBench/MARBLE.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 LLM-Based Multi-Agent Systems 2.2 Multi-Agent Collaboration 3 Methodology 3.1 Framework Design Agent Graph Module Cognitive Module 3.1.1 Coordination Engine Centralized Coordination: Star Tree. Decentralized Coordination: Graph-Mesh Chain. Planner Design and Enhancements. 3.2 Benchmark Design Agents with Mutual Goal. Agents with Conflicting Goals. Role Assignments and Graph Structures. Milestones Generation for Scenarios 3.3 Evaluation Metrics Task Completion Metrics. Coordination Metrics. 4 Experiment Setup 4.1 Experiment Settings Models. 4.2 Main Experiment One: Model Performance Across Different Scenarios 1. Superior Task Performance of gpt-4o-mini : 2. The Nuanced Role of Coordination (Collaboration) Score: 3. Model-Specific Strengths and Context-Dependent Performance: 4.3 Main Experiment Two: Effects of Collaboration Protocols and Planning Strategies 5 Ablation Study Ablation on Different Max Iteration Settings Ablation on Different Agent Numbers 6 Emergent…

**Method / approach.** Methodology 3.1 Framework Design Agent Graph Module Cognitive Module 3.1.1 Coordination Engine Centralized Coordination: Star Tree. Decentralized Coordination: Graph-Mesh Chain. Planner Design and Enhancements. 3.2 Benchmark Design Agents with Mutual Goal. Agents with Conflicting Goals. Role Assignments and Graph Structures. Milestones Generation for Scenarios 3.3 Evaluation Metrics Task Completion Metrics. Coordination Metrics. 4 Experiment Setup 4.1 Experiment Settings Models. 4.2 Main Experiment One: Model Performance Across Different Scenarios 1. Superior Task Performance of gpt-4o-mini : 2. The Nuanced Role of Coordination (Collaboration) Score: 3. Model-Specific Strengths and Context-Dependent Performance: 4.3 Main Experiment Two: Effects of Collaboration Protocols and Planning Strategies 5 Ablation Study Ablation on Different Max Iteration Settings Ablation on Different Agent Numbers 6 Emergent Behav…

**Results.** Experiment Setup 4.1 Experiment Settings Models. 4.2 Main Experiment One: Model Performance Across Different Scenarios 1. Superior Task Performance of gpt-4o-mini : 2. The Nuanced Role of Coordination (Collaboration) Score: 3. Model-Specific Strengths and Context-Dependent Performance: 4.3 Main Experiment Two: Effects of Collaboration Protocols and Planning Strategies 5 Ablation Study Ablation on Different Max Iteration Settings Ablation on Different Agent Numbers 6 Emergent Behaviors Analysis Strategic Information Sharing Trust-Polarized Collaboration Role-Driven Strategy Iteration 7 Conclusion 8 Limitations Expanding Scenario and Model Coverage. Enhancing Ablation Studies. Advancing Competition Mechanisms. Handling Open-Ended and Ill-Defined Tasks. A Appendix A.1 Contributions Kunlun Zhu Hongyi Du Zhaochen Hong Xiaochen Yang Shuyi Guo Zhe Wang ‣ A.1 Contri…

**Conclusion.** Conclusion 8 Limitations Expanding Scenario and Model Coverage. Enhancing Ablation Studies. Advancing Competition Mechanisms. Handling Open-Ended and Ill-Defined Tasks. A Appendix A.1 Contributions Kunlun Zhu Hongyi Du Zhaochen Hong Xiaochen Yang Shuyi Guo Zhe Wang ‣ A.1 Contributions A.2 More Details on Multi-agent framework design Configuration Module Environment Module Memory Module Communication Module Action Module A.3 Human Evaluation Analysis. A.4 Research Scenario A.5 Werewolf Environment A.5.1 Environment Description (Tool Description) Why Werewolf? A.5.2 Villager-Centric Scoring Rationale Consistent Werewolf Model. A.5.3 Benchmark Curation Details…

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[gpt-5]]
- **Raw:** `raw/arxiv/2503.01935v1.md` · `raw/arxiv/2503.01935v1.fulltext.md`
