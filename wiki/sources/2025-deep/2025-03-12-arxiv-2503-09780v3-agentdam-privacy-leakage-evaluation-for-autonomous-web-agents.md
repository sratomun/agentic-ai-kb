---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "AgentDAM: Privacy Leakage Evaluation for Autonomous Web Agents"
authors: Arman Zharmagambetov, Chuan Guo, Ivan Evtimov, Maya Pavlova et al.
url: https://arxiv.org/abs/2503.09780v3
date: 2025-03-12
citationCount: 59
influentialCitationCount: 8
velocity: 3.85
ingested: 2026-06-22
tags: [computer-use-agents, embodied-agents, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# AgentDAM: Privacy Leakage Evaluation for Autonomous Web Agents

**arXiv [2503.09780v3](https://arxiv.org/abs/2503.09780v3)** · 2025-03-12 · **59 citations** (8 influential · 3.85/mo) · Arman Zharmagambetov, Chuan Guo, Ivan Evtimov, Maya Pavlova et al.

## Abstract
Autonomous AI agents that can follow instructions and perform complex multi-step tasks have tremendous potential to boost human productivity. However, to perform many of these tasks, the agents need access to personal information from their users, raising the question of whether they are capable of using it appropriately. In this work, we introduce a new benchmark AgentDAM that measures if AI web-navigation agents follow the privacy principle of ``data minimization''. For the purposes of our benchmark, data minimization means that the agent uses a piece of potentially sensitive information only if it is ``necessary'' to complete a particular task. Our benchmark simulates realistic web interaction scenarios end-to-end and is adaptable to all existing web navigation agents. We use AgentDAM to evaluate how well AI agents built on top of GPT-4, Llama-3 and Claude can limit processing of potentially private information, and show that they are prone to inadvertent use of unnecessary sensitive information. We also propose a prompting-based defense that reduces information leakage, and demonstrate that our end-to-end benchmarking provides a more realistic measure than probing LLMs about privacy. Our results highlight that further research is needed to develop AI agents that can prioritize data minimization at inference time.

## From the paper (full-text excerpts)
**Introduction.** Introduction Disclaimer. 2 Related Work 3 AgentDAM : Privacy Benchmark for Web Agents 3.1 Preliminaries: Agentic setup Threat Model State space S S and observation space Ω \Omega . Action space A A . State transition function F F . Illustrative example 3.2 Task Design and Data Generation Tasks. Collecting human-written seed data. 3.3 Evaluation Evaluating utility. Evaluating privacy. 3.4 Privacy leakage mitigations 4 Experiments 4.1 Setup 4.2 Is Probing LLMs sufficient to assess agents’ performance in action? 4.3 Main Evaluation Main Observations. Mitigation. 4.4 Analyzing privacy leakages 5 Discussions and Conclusion A Details of the agentic environment B Details of dataset generation B.1 Example data seeds B.2 Regarding our dataset size Why this size is sufficient? C Prompts D Detailed evaluation results E Additional examples of agentic traces E.1 Example 1 E.2 Example 2 AgentDAM : Privacy Leakage Evaluation for Autonomous Web Agents Arman Zharmagambetov FAIR at Meta a…

**Method / approach.** Method agentic multistep multimodal full-stack agentic diverse set tasks trajectories inputs environment of tasks ConfAIde [ 24 ] ✓ ✗ ✗ ✗ ✗ PrivacyLens [ 31 ] ✓ ✓ ✗ ✗ ✗ AirGapAgent [ 4 ] ✓ ✗ ✗ ✗ ✓ Ghalebikesabi et.al. [ 15 ] ✓ ✗ ✗ ✗ ✗ CI-Bench [ 10 ] ✓ ✗ ✗ ✗ ✓ AgentDAM (ours) ✓ ✓ ✓ ✓ ✓ AI Agents. While there is a great deal of interest in developing AI agents, there is no standardization in their setup and operation. So far, one of the most widespread practical implementation involves scaffolding around LLMs , where code is built around an LLM to augment its capabilities and enable interaction with tools such as browsers and email clients [ 41 , 19 , 12 , 40 ] . An important use case is web navigation, where the implementations utilize a representation of the website, such as textual (e.g. DOM tree) and/or image (e.g. screenshot), and pair it with a browser interaction ba…

**Results.** Experiments 4.1 Setup 4.2 Is Probing LLMs sufficient to assess agents’ performance in action? 4.3 Main Evaluation Main Observations. Mitigation. 4.4 Analyzing privacy leakages 5 Discussions and Conclusion A Details of the agentic environment B Details of dataset generation B.1 Example data seeds B.2 Regarding our dataset size Why this size is sufficient? C Prompts D Detailed evaluation results E Additional examples of agentic traces E.1 Example 1 E.2 Example 2 AgentDAM : Privacy Leakage Evaluation for Autonomous Web Agents Arman Zharmagambetov FAIR at Meta armanz@meta.com Chuan Guo FAIR at Meta chuanguo@meta.com Ivan Evtimov 1 1 footnotemark: 1 FAIR at Meta ivanevtimov@meta.com Maya Pavlova Meta mayapavlova@meta.com Ruslan Salakhutdinov FAIR at Meta rsalakhu@meta.com Kamalika Chaudhuri FAIR at Meta kamalika@meta.com equal contribution Abstr…

**Conclusion.** Conclusion A Details of the agentic environment B Details of dataset generation B.1 Example data seeds B.2 Regarding our dataset size Why this size is sufficient? C Prompts D Detailed evaluation results E Additional examples of agentic traces E.1 Example 1 E.2 Example 2 AgentDAM : Privacy Leakage Evaluation for Autonomous Web Agents Arman Zharmagambetov FAIR at Meta armanz@meta.com Chuan Guo FAIR at Meta chuanguo@meta.com Ivan Evtimov 1 1 footnotemark: 1 FAIR at Meta ivanevtimov@meta.com Maya Pavlova Meta mayapavlova@meta.com Ruslan Salakhutdinov FAIR at Meta rsalakhu@meta.com Kamalika Chaudhuri FAIR at Meta kamalika@meta.com equal contribution Abstract Autonomous…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[claude]]
- **Raw:** `raw/arxiv/2503.09780v3.md` · `raw/arxiv/2503.09780v3.fulltext.md`
