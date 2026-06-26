---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Memory Injection Attacks on LLM Agents via Query-Only Interaction"
authors: Shen Dong, Shaochen Xu, Pengfei He, Yige Li et al.
url: https://arxiv.org/abs/2503.03704v5
date: 2025-03-05
citationCount: 69
influentialCitationCount: 13
velocity: 4.43
ingested: 2026-06-22
tags: [agent-security, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# Memory Injection Attacks on LLM Agents via Query-Only Interaction

**arXiv [2503.03704v5](https://arxiv.org/abs/2503.03704v5)** · 2025-03-05 · **69 citations** (13 influential · 4.43/mo) · Shen Dong, Shaochen Xu, Pengfei He, Yige Li et al.

## Abstract
Agents powered by large language models (LLMs) have demonstrated strong capabilities in a wide range of complex, real-world applications. However, LLM agents with a compromised memory bank may easily produce harmful outputs when the past records retrieved for demonstration are malicious. In this paper, we propose a novel Memory INJection Attack, MINJA, without assuming that the attacker can directly modify the memory bank of the agent. The attacker injects malicious records into the memory bank by only interacting with the agent via queries and output observations. These malicious records are designed to elicit a sequence of malicious reasoning steps corresponding to a different target query during the agent's execution of the victim user's query. Specifically, we introduce a sequence of bridging steps to link victim queries to the malicious reasoning steps. During the memory injection, we propose an indication prompt that guides the agent to autonomously generate similar bridging steps, with a progressive shortening strategy that gradually removes the indication prompt, such that the malicious record will be easily retrieved when processing later victim queries. Our extensive experiments across diverse agents demonstrate the effectiveness of MINJA in compromising agent memory. With minimal requirements for execution, MINJA enables any user to influence agent memory, highlighting the risk.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work LLM Agents Memory Utilization Poisoning of Agent Memory 3 Threat Model Agent Settings Attacker’s Objectives Realistic Constraints and Assumptions 4 Method 4.1 Design Malicious Records with Bridging Steps 4.2 Injection of Malicious Records via Indication Prompts with Progressive Shortening 5 Experiments 5.1 Experimental Settings 5.2 Main Results 5.3 Ablation Studies 5.4 Potential Defense 6 Conclusion A Algorithm of progressive shortening Strategy B EHRAgent QA Agent normal user agent interaction B.1 EHRAgent B.2 QA Agent C Vitim-target pairs for each dataset D Example attack queries on four datasets E Details of MINJA on each agent E.1 EHRAgent - MIMIC-III E.2 EHRAgent - eICU E.3 RAP - Webshop E.4 QA Agent - MMLU F Comparison between MINJA and prior reasoning-based attacks G Analysis of moderate UD on MMLU H Details of embedding models used in ablation studies I Validation of experimental setup under memory retrieval filtering J Extended evaluation on model variants K…

**Method / approach.** Method 4.1 Design Malicious Records with Bridging Steps 4.2 Injection of Malicious Records via Indication Prompts with Progressive Shortening 5 Experiments 5.1 Experimental Settings 5.2 Main Results 5.3 Ablation Studies 5.4 Potential Defense 6 Conclusion A Algorithm of progressive shortening Strategy B EHRAgent QA Agent normal user agent interaction B.1 EHRAgent B.2 QA Agent C Vitim-target pairs for each dataset D Example attack queries on four datasets E Details of MINJA on each agent E.1 EHRAgent - MIMIC-III E.2 EHRAgent - eICU E.3 RAP - Webshop E.4 QA Agent - MMLU F Comparison between MINJA and prior reasoning-based attacks G Analysis of moderate UD on MMLU H Details of embedding models used in ablation studies I Validation of experimental setup under memory retrieval filtering J Extended evaluation on model variants K Stability evaluation of MINJA ’s ASR L Number of shortening steps in PSS M Stepwise Injection S…

**Results.** Experiments 5.1 Experimental Settings 5.2 Main Results 5.3 Ablation Studies 5.4 Potential Defense 6 Conclusion A Algorithm of progressive shortening Strategy B EHRAgent QA Agent normal user agent interaction B.1 EHRAgent B.2 QA Agent C Vitim-target pairs for each dataset D Example attack queries on four datasets E Details of MINJA on each agent E.1 EHRAgent - MIMIC-III E.2 EHRAgent - eICU E.3 RAP - Webshop E.4 QA Agent - MMLU F Comparison between MINJA and prior reasoning-based attacks G Analysis of moderate UD on MMLU H Details of embedding models used in ablation studies I Validation of experimental setup under memory retrieval filtering J Extended evaluation on model variants K Stability evaluation of MINJA ’s ASR L Number of shortening steps in PSS M Stepwise Injection Success Rate of Progressive Shortening N Additional Visualization O Potential Extension to More Agent…

**Conclusion.** Conclusion A Algorithm of progressive shortening Strategy B EHRAgent QA Agent normal user agent interaction B.1 EHRAgent B.2 QA Agent C Vitim-target pairs for each dataset D Example attack queries on four datasets E Details of MINJA on each agent E.1 EHRAgent - MIMIC-III E.2 EHRAgent - eICU E.3 RAP - Webshop E.4 QA Agent - MMLU F Comparison between MINJA and prior reasoning-based attacks G Analysis of moderate UD on MMLU H Details of embedding models used in ablation studies I Validation of experimental setup under memory retrieval filtering J Extended evaluation on model variants K Stability evaluation of MINJA ’s ASR L Number of shortening steps in PSS M Stepwise Injection Success Rate of Pr…

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2503.03704v5.md` · `raw/arxiv/2503.03704v5.fulltext.md`
