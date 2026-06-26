---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Evo-Memory: Benchmarking LLM Agent Test-time Learning with Self-Evolving Memory"
authors: Tianxin Wei, Noveen Sachdeva, Benjamin Coleman, Zhankui He et al.
url: https://arxiv.org/abs/2511.20857v2
date: 2025-11-25
citationCount: 89
influentialCitationCount: 6
velocity: 12.96
ingested: 2026-06-22
tags: [embodied-agents, self-evolving-agents, agent-memory, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Evo-Memory: Benchmarking LLM Agent Test-time Learning with Self-Evolving Memory

**arXiv [2511.20857v2](https://arxiv.org/abs/2511.20857v2)** · 2025-11-25 · **89 citations** (6 influential · 12.96/mo) · Tianxin Wei, Noveen Sachdeva, Benjamin Coleman, Zhankui He et al.

## Abstract
Statefulness is essential for large language model (LLM) agents to perform long-term planning and problem-solving. This makes memory a critical component, yet its management and evolution remain largely underexplored. Existing evaluations mostly focus on static conversational settings, where memory is passively retrieved from dialogue to answer queries, overlooking the dynamic ability to accumulate and reuse experience across evolving task streams. In real-world environments such as interactive problem assistants or embodied agents, LLMs are required to handle continuous task streams, yet often fail to learn from accumulated interactions, losing valuable contextual insights, a limitation that calls for test-time evolution, where LLMs retrieve, integrate, and update memory continuously during deployment. To bridge this gap, we introduce Evo-Memory, a comprehensive streaming benchmark and framework for evaluating self-evolving memory in LLM agents. Evo-Memory structures datasets into sequential task streams, requiring LLMs to search, adapt, and evolve memory after each interaction. We unify and implement over ten representative memory modules and evaluate them across 10 diverse multi-turn goal-oriented and single-turn reasoning and QA datasets. To better benchmark experience reuse, we provide a baseline method, ExpRAG, for retrieving and utilizing prior experience, and further propose ReMem, an action-think-memory refine pipeline that tightly integrates reasoning, task actions, and memory updates to achieve continual improvement.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Test-time Learning 2.2 Self-evolving Memory 3 Evo-Memory: Evaluating Self-Evolving Memory in LLM Agents 3.1 Problem Formulation Search. Synthesis. Evolve. Dataset Preparation. 3.2 ExpRAG : Experience Retrieval and Aggregation 3.3 ReMem: Synergizing Reasoning, Acting, and Memory 4 Experiments 4.1 Experimental Setup 4.1.1 Datasets 4.1.2 Methods 4.2 Experimental Results 4.2.1 Analysis of Results (RQ1) 4.2.2 Analysis of Memory Improvement (RQ2) 4.2.3 Task Sequence: Easy v.s. Hard (RQ3) 4.2.4 Analysis of Feedback (RQ4) 5 Conclusion References A Experimental Details A.1 Datasets A.2 Configuration A.3 Evaluation A.4 Methods Agent Pipelines without Procedural Memory. Adaptive Agentic Memory Methods. Memory-Based Agents for Procedural Memory. Proposed: Evolving Memory Framework. B Experiments B.1 Additional Experiments B.2 Additional Analysis of Memory Pruning B.3 Cumulative Accuracy Across Tasks and Models C Potential Risks D Prompts E Ethical Considerati…

**Method / approach.** Methods 4.2 Experimental Results 4.2.1 Analysis of Results (RQ1) 4.2.2 Analysis of Memory Improvement (RQ2) 4.2.3 Task Sequence: Easy v.s. Hard (RQ3) 4.2.4 Analysis of Feedback (RQ4) 5 Conclusion References A Experimental Details A.1 Datasets A.2 Configuration A.3 Evaluation A.4 Methods Agent Pipelines without Procedural Memory. Adaptive Agentic Memory Methods. Memory-Based Agents for Procedural Memory. Proposed: Evolving Memory Framework. B Experiments B.1 Additional Experiments B.2 Additional Analysis of Memory Pruning B.3 Cumulative Accuracy Across Tasks and Models C Potential Risks D Prompts E Ethical Considerations and Artifact Documentation E.1 Cite Creators of Artifacts E.2 Discuss the License for Artifacts E.3 Artifact Use Consistent with Intended Purpose E.4 Personally Identifying Information or Offensive Content E.5 Documentation of Artifacts F Statistics for Data F.1 Single-Turn Reasoning Dat…

**Results.** Experiments 4.1 Experimental Setup 4.1.1 Datasets 4.1.2 Methods 4.2 Experimental Results 4.2.1 Analysis of Results (RQ1) 4.2.2 Analysis of Memory Improvement (RQ2) 4.2.3 Task Sequence: Easy v.s. Hard (RQ3) 4.2.4 Analysis of Feedback (RQ4) 5 Conclusion References A Experimental Details A.1 Datasets A.2 Configuration A.3 Evaluation A.4 Methods Agent Pipelines without Procedural Memory. Adaptive Agentic Memory Methods. Memory-Based Agents for Procedural Memory. Proposed: Evolving Memory Framework. B Experiments B.1 Additional Experiments B.2 Additional Analysis of Memory Pruning B.3 Cumulative Accuracy Across Tasks and Models C Potential Risks D Prompts E Ethical Considerations and Artifact Documentation E.1 Cite Creators of Artifacts E.2 Discuss the License for Artifacts E.3 Artifact Use Consistent with Intended Purpose E.4 Personally Identifying Informatio…

**Conclusion.** Conclusion References A Experimental Details A.1 Datasets A.2 Configuration A.3 Evaluation A.4 Methods Agent Pipelines without Procedural Memory. Adaptive Agentic Memory Methods. Memory-Based Agents for Procedural Memory. Proposed: Evolving Memory Framework. B Experiments B.1 Additional Experiments B.2 Additional Analysis of Memory Pruning B.3 Cumulative Accuracy Across Tasks and Models C Potential Risks D Prompts E Ethical Considerations and Artifact Documentation E.1 Cite Creators of Artifacts E.2 Discuss the License for Artifacts E.3 Artifact Use Consistent with Intended Purpose E.4 Personally Identifying Information or Offensive Content E.5 Documentation of Artifacts F Stati…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2511.20857v2.md` · `raw/arxiv/2511.20857v2.fulltext.md`
