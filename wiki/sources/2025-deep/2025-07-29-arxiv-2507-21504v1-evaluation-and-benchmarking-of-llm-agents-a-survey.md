---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Evaluation and Benchmarking of LLM Agents: A Survey"
authors: Mahmoud Mohammadi, Yipeng Li, Jane Lo, Wendy Yip
url: https://arxiv.org/abs/2507.21504v1
date: 2025-07-29
citationCount: 136
influentialCitationCount: 4
velocity: 12.62
ingested: 2026-06-22
tags: [agent-reliability, agent-security, agent-memory, agent-evaluation, governance-gap, arxiv, 2025, cited]
---

# Evaluation and Benchmarking of LLM Agents: A Survey

**arXiv [2507.21504v1](https://arxiv.org/abs/2507.21504v1)** · 2025-07-29 · **136 citations** (4 influential · 12.62/mo) · Mahmoud Mohammadi, Yipeng Li, Jane Lo, Wendy Yip

## Abstract
The rise of LLM-based agents has opened new frontiers in AI applications, yet evaluating these agents remains a complex and underdeveloped area. This survey provides an in-depth overview of the emerging field of LLM agent evaluation, introducing a two-dimensional taxonomy that organizes existing work along (1) evaluation objectives -- what to evaluate, such as agent behavior, capabilities, reliability, and safety -- and (2) evaluation process -- how to evaluate, including interaction modes, datasets and benchmarks, metric computation methods, and tooling. In addition to taxonomy, we highlight enterprise-specific challenges, such as role-based access to data, the need for reliability guarantees, dynamic and long-horizon interactions, and compliance, which are often overlooked in current research. We also identify future research directions, including holistic, more realistic, and scalable evaluation. This work aims to bring clarity to the fragmented landscape of agent evaluation and provide a framework for systematic assessment, enabling researchers and practitioners to evaluate LLM agents for real-world deployment.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Taxonomy for LLM-based Agent Evaluation 3 Evaluation Objectives 3.1 Agent Behavior 3.1.1 Task Completion: 3.1.2 Output Quality: 3.1.3 Latency Cost: 3.2 Agent Capabilities 3.2.1 Tool Use: 3.2.2 Planning and Reasoning: 3.2.3 Memory and Context Retention: 3.2.4 Multi-Agent Collaboration: 3.3 Reliability 3.3.1 Consistency: 3.3.2 Robustness: 3.4 Safety and Alignment 3.4.1 Fairness: 3.4.2 Harm, Toxicity, and Bias: 3.4.3 Compliance and Privacy: 4 Evaluation Process 4.1 Interaction Mode 4.1.1 Static Offline Evaluation 4.1.2 Dynamic Online Evaluation 4.2 Evaluation Data 4.3 Metrics Computation Methods 4.4 Evaluation Tooling 4.5 Evaluation Contexts 5 Enterprise-Specific Challenges 5.1 Complexity from Role-based Access 5.2 Reliability Guarantees 5.3 Dynamic and Long-Horizon Interactions 5.4 Adherence to Domain-Specific Policies and Compliance Requirements 6 Future Research Directions \setcctype by Evaluation and Benchmarking of LLM Agents: A Survey Mahmoud Mohammadi mahmoud.moham…

**Method / approach.** Methods 4.4 Evaluation Tooling 4.5 Evaluation Contexts 5 Enterprise-Specific Challenges 5.1 Complexity from Role-based Access 5.2 Reliability Guarantees 5.3 Dynamic and Long-Horizon Interactions 5.4 Adherence to Domain-Specific Policies and Compliance Requirements 6 Future Research Directions \setcctype by Evaluation and Benchmarking of LLM Agents: A Survey Mahmoud Mohammadi mahmoud.mohammadi@sap.com 0000-0001-6829-1420 SAP Labs Bellevue WA USA , Yipeng Li yipeng.li@sap.com 0009-0002-4076-864X SAP Labs Bellevue WA USA , Jane Lo jane.lo@sap.com 0009-0007-6117-5022 SAP Labs Palo Alto CA USA and Wendy Yip wendy.yip@sap.com 0009-0008-1734-2935 SAP Labs Palo Alto CA USA (2025) Abstract. The rise of LLM-based agents has opened new frontiers in AI applications, yet evaluating these agents remains a complex and underdeveloped area. This survey provides an in-depth overview of the emerging field…

**Conclusion.** conclusions, benchmarks must include a representative dataset that reflects the types of tasks and conditions the agent may encounter. Some efforts have begun to tackle this challenge. For example, the τ \tau italic_τ -benchmark (Yao et al., 2024 ) explicitly incorporates the pass^ k k italic_k metric to evaluate the consistency of an agent. By applying this to domains such as retail and airline booking, the authors show that current agents struggle with consistency. 5.3. Dynamic and Long-Horizon Interactions One major challenge in evaluating LLM-based agents is assessing their performance on long-horizon tasks in dynamic, evolving environments. Unlike most current benchmarks that focus on short episodes or single interactions, re…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]]
- **Raw:** `raw/arxiv/2507.21504v1.md` · `raw/arxiv/2507.21504v1.fulltext.md`
