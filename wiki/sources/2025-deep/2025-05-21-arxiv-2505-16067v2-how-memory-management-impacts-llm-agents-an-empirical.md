---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "How Memory Management Impacts LLM Agents: An Empirical Study of Experience-Following Behavior"
authors: Zidi Xiong, Yuping Lin, Wenya Xie, Pengfei He et al.
url: https://arxiv.org/abs/2505.16067v2
date: 2025-05-21
citationCount: 57
influentialCitationCount: 5
velocity: 4.37
ingested: 2026-06-22
tags: [agent-memory, agentic-ai, arxiv, 2025, cited]
---

# How Memory Management Impacts LLM Agents: An Empirical Study of Experience-Following Behavior

**arXiv [2505.16067v2](https://arxiv.org/abs/2505.16067v2)** · 2025-05-21 · **57 citations** (5 influential · 4.37/mo) · Zidi Xiong, Yuping Lin, Wenya Xie, Pengfei He et al.

## Abstract
Memory is a critical component in large language model (LLM)-based agents, enabling them to store and retrieve past executions to improve task performance over time. In this paper, we conduct an empirical study on how memory management choices impact the LLM agents' behavior, especially their long-term performance. Specifically, we focus on two fundamental memory management operations that are widely used by many agent frameworks-memory addition and deletion-to systematically study their impact on the agent behavior. Through our quantitative analysis, we find that LLM agents display an experience-following property: high similarity between a task input and the input in a retrieved memory record often results in highly similar agent outputs. Our analysis further reveals two significant challenges associated with this property: error propagation, where inaccuracies in past experiences compound and degrade future performance, and misaligned experience replay, where some seemingly correct executions can provide limited or even misleading value as experiences. Through controlled experiments, we demonstrate the importance of regulating experience quality within the memory bank and show that future task evaluations can serve as free quality labels for stored memory. Our findings offer insights into the behavioral dynamics of LLM agent memory systems and provide practical guidance for designing memory components that support robust, long-term agent performance.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Background and Related Works 2.1 Memory Module of LLM Agents 2.2 Memory Management and Limitations Memory Reading: Memory Management and Limitations: 3 Addition of Memory 3.1 Setup Setup for Agents Setup for Memory Addition 3.2 Execution quality and memory size jointly determine long-term agent performance. 3.3 Experience-Following Property 3.4 Error Propagation in Agent Memory 4 Deletion of Memory 4.1 Setup for Memory Deletion Experiments 4.2 Strategic Memory Deletion Improves the Agent Performance 4.3 Misaligned Experience Replay 5 Memory Management under Challenging Scenarios 5.1 Memory Management with Task distribution shift Results 5.2 Memory Management with Resource Constraints Results 6 Conclusion A Detailed experimental setups. A.1 Agent details and functionality RegAgents EHRAgents AgentDriver CIC-IoT A.2 RegAgent design A.3 CIC-IoT Agent design A.4 Coarse evaluator prompts A.5 Additional setup for task distribution shift B Additional results B.1 Additional res…

**Method / approach.** methods start with the same initial memory, their long-term performances diverge notably. The fixed-memory baseline maintains strong results with RegAgent, AgentDriver, and CIC-IoT Agent—sometimes even surpassing runs guided by coarse evaluators—indicating that noisy or low-quality additions can harm memory utility. In contrast, using a strict evaluator that selectively expands memory with high-quality records consistently yields superior performance, showing that both memory quality and capacity are key to effective long-term learning. Furthermore, performance relies on the judge’s capability for coarse evaluators. For the three model judged agents, fine-tuning the evaluator on only 300 trajectories (C3) already achieves strong long-term improvements, outperforming other coarse evaluators and unfiltered additions. As shown in Figure 2 and Figure 8 in Appendix B.1 , the add-all and some coarse addition approach exhibits flat or declining success rates, suggesting accumulation…

**Results.** Experiments 4.2 Strategic Memory Deletion Improves the Agent Performance 4.3 Misaligned Experience Replay 5 Memory Management under Challenging Scenarios 5.1 Memory Management with Task distribution shift Results 5.2 Memory Management with Resource Constraints Results 6 Conclusion A Detailed experimental setups. A.1 Agent details and functionality RegAgents EHRAgents AgentDriver CIC-IoT A.2 RegAgent design A.3 CIC-IoT Agent design A.4 Coarse evaluator prompts A.5 Additional setup for task distribution shift B Additional results B.1 Additional results on addition experiments B.2 Experiments on different LLM backbones B.3 Error-free variant of history-based deletion B.4 History-based deletion on different evaluators B.5 Comparison between deleted records and retained records B.6 Results under memory resource constraints. How Memory Management Impacts LLM Agents: An Em…

**Conclusion.** Conclusion A Detailed experimental setups. A.1 Agent details and functionality RegAgents EHRAgents AgentDriver CIC-IoT A.2 RegAgent design A.3 CIC-IoT Agent design A.4 Coarse evaluator prompts A.5 Additional setup for task distribution shift B Additional results B.1 Additional results on addition experiments B.2 Experiments on different LLM backbones B.3 Error-free variant of history-based deletion B.4 History-based deletion on different evaluators B.5 Comparison between deleted records and retained records B.6 Results under memory resource constraints. How Memory Management Impacts LLM Agents: An Empirical Study of Experience-Following Behavior Zidi Xiong 1 , Yuping Lin 3∗ , Wenya Xie 4∗ ,…

## Graph
- **Concepts:** [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2505.16067v2.md` · `raw/arxiv/2505.16067v2.fulltext.md`
