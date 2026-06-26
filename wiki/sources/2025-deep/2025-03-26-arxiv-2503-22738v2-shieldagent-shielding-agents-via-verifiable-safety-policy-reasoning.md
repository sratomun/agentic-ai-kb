---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "ShieldAgent: Shielding Agents via Verifiable Safety Policy Reasoning"
authors: Zhaorun Chen, Mintong Kang, Bo Li
url: https://arxiv.org/abs/2503.22738v2
date: 2025-03-26
citationCount: 98
influentialCitationCount: 16
velocity: 6.59
ingested: 2026-06-22
tags: [finance-agents, agent-security, agent-evaluation, governance-gap, agentic-ai, arxiv, 2025, cited]
---

# ShieldAgent: Shielding Agents via Verifiable Safety Policy Reasoning

**arXiv [2503.22738v2](https://arxiv.org/abs/2503.22738v2)** · 2025-03-26 · **98 citations** (16 influential · 6.59/mo) · Zhaorun Chen, Mintong Kang, Bo Li

## Abstract
Autonomous agents powered by foundation models have seen widespread adoption across various real-world applications. However, they remain highly vulnerable to malicious instructions and attacks, which can result in severe consequences such as privacy breaches and financial losses. More critically, existing guardrails for LLMs are not applicable due to the complex and dynamic nature of agents. To tackle these challenges, we propose ShieldAgent, the first guardrail agent designed to enforce explicit safety policy compliance for the action trajectory of other protected agents through logical reasoning. Specifically, ShieldAgent first constructs a safety policy model by extracting verifiable rules from policy documents and structuring them into a set of action-based probabilistic rule circuits. Given the action trajectory of the protected agent, ShieldAgent retrieves relevant rule circuits and generates a shielding plan, leveraging its comprehensive tool library and executable code for formal verification. In addition, given the lack of guardrail benchmarks for agents, we introduce ShieldAgent-Bench, a dataset with 3K safety-related pairs of agent instructions and action trajectories, collected via SOTA attacks across 6 web environments and 7 risk categories. Experiments show that ShieldAgent achieves SOTA on ShieldAgent-Bench and three existing benchmarks, outperforming prior methods by 11.3% on average with a high recall of 90.1%. Additionally, ShieldAgent reduces API queries by 64.7% and inference time by 58.2%, demonstrating its high precision and efficiency in safeguarding agents.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 2.1 Safety of LLM Agents 2.2 LLM Guardrails 3 ShieldAgent 3.1 Overview 3.2 Action-based Safety Policy Model 3.2.1 Ovewview of ASPM 3.2.2 Automatic Policy and Rule Extraction 3.2.3 ASPM Structure Optimization 3.2.4 ASPM Inference Training 3.3 ShieldAgent Framework 4 ShieldAgent-Bench Dataset 5 Experiment 5.1 Setup 5.2 Results 6 Conclusion A Detailed Introduction to ShieldAgent A.1 Notations A.2 Solution Space B Additional Results B.1 ST-WebAgentBench B.2 VWA-Adv B.3 AgentHarm C Action-based Probabilistic Safety Policy Model C.1 Automated Policy Extraction C.2 Safety Policy Model Construction C.2.1 Automatic Policy And Rule Extraction C.3 Linear Temporal Logic (LTL) Rules C.4 ASPM Structure Optimization C.5 Training ASPM D ShieldAgent Framework E ShieldAgent-Bench E.1 Risk Categories F Detailed Experiment Results F.1 Dataset Distribution G Case Study H Prompt Template ShieldAgent : Shielding Agents via Verifiable Safety Policy Reasoning…

**Method / approach.** methods by 11.3 % 11.3\% on average with a high recall of 90.1 % 90.1\% . Additionally, ShieldAgent reduces API queries by 64.7 % 64.7\% and inference time by 58.2 % 58.2\% , demonstrating its high precision and efficiency in safeguarding agents. Our project is available and continuously maintained here: https://shieldagent-aiguard.github.io/ Machine Learning, ICML 1 Introduction LLM-based autonomous agents are rapidly gathering momentum across various applications, integrating their ability to call external tools and make autonomous decisions in real-world tasks such as web browsing ( zhou2023webarena ) , GUI navigation ( lin2024showui ) , and embodied control ( mao2023language ) . Among these, LLM-based web agents , such as OpenAI’s Operator ( operator2025 ) , deep research agent ( deepresearch2025 ) , and Anthropic’s computer assistant agent ( mcp2025 ) , have become particularly prominent, driving automation in areas like online shopping, stock trading, and informa…

**Results.** Experiment 5.1 Setup 5.2 Results 6 Conclusion A Detailed Introduction to ShieldAgent A.1 Notations A.2 Solution Space B Additional Results B.1 ST-WebAgentBench B.2 VWA-Adv B.3 AgentHarm C Action-based Probabilistic Safety Policy Model C.1 Automated Policy Extraction C.2 Safety Policy Model Construction C.2.1 Automatic Policy And Rule Extraction C.3 Linear Temporal Logic (LTL) Rules C.4 ASPM Structure Optimization C.5 Training ASPM D ShieldAgent Framework E ShieldAgent-Bench E.1 Risk Categories F Detailed Experiment Results F.1 Dataset Distribution G Case Study H Prompt Template ShieldAgent : Shielding Agents via Verifiable Safety Policy Reasoning Zhaorun Chen Mintong Kang Bo Li Abstract Autonomous agents powered by foundation models have seen widespread adoption across various real-world applications. However, they remain highly vulnerable to malici…

**Conclusion.** Conclusion A Detailed Introduction to ShieldAgent A.1 Notations A.2 Solution Space B Additional Results B.1 ST-WebAgentBench B.2 VWA-Adv B.3 AgentHarm C Action-based Probabilistic Safety Policy Model C.1 Automated Policy Extraction C.2 Safety Policy Model Construction C.2.1 Automatic Policy And Rule Extraction C.3 Linear Temporal Logic (LTL) Rules C.4 ASPM Structure Optimization C.5 Training ASPM D ShieldAgent Framework E ShieldAgent-Bench E.1 Risk Categories F Detailed Experiment Results F.1 Dataset Distribution G Case Study H Prompt Template ShieldAgent : Shielding Agents via Verifiable Safety Policy Reasoning Zhaorun Chen Mintong Kang Bo Li Abstract Autonomou…

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[agent-security|Agent security]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2503.22738v2.md` · `raw/arxiv/2503.22738v2.fulltext.md`
