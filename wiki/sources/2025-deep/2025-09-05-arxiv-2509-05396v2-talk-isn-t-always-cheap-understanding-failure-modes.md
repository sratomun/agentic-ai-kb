---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Talk Isn't Always Cheap: Understanding Failure Modes in Multi-Agent Debate"
authors: Andrea Wynn, Harsh Satija, Gillian Hadfield
url: https://arxiv.org/abs/2509.05396v2
date: 2025-09-05
citationCount: 42
influentialCitationCount: 7
velocity: 4.41
ingested: 2026-06-22
tags: [agent-reliability, multi-agent-systems, agentic-ai, arxiv, 2025, cited]
---

# Talk Isn't Always Cheap: Understanding Failure Modes in Multi-Agent Debate

**arXiv [2509.05396v2](https://arxiv.org/abs/2509.05396v2)** · 2025-09-05 · **42 citations** (7 influential · 4.41/mo) · Andrea Wynn, Harsh Satija, Gillian Hadfield

## Abstract
While multi-agent debate has been proposed as a promising strategy for improving AI reasoning ability, we find that debate can sometimes be harmful rather than helpful. Prior work has primarily focused on debates within homogeneous groups of agents, whereas we explore how diversity in model capabilities influences the dynamics and outcomes of multi-agent interactions. Through a series of experiments, we demonstrate that debate can lead to a decrease in accuracy over time - even in settings where stronger (i.e., more capable) models outnumber their weaker counterparts. Our analysis reveals that models frequently shift from correct to incorrect answers in response to peer reasoning, favoring agreement over challenging flawed reasoning. We perform additional experiments investigating various potential contributing factors to these harmful shifts - including sycophancy, social conformity, and model and task type. These results highlight important failure modes in the exchange of reasons during multi-agent debate, suggesting that naive applications of debate may cause performance degradation when agents are neither incentivised nor adequately equipped to resist persuasive but incorrect reasoning.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Setting: Multi-agent debate 4 Experimental Setup 4.1 Datasets 4.2 Models 4.3 Prompts 4.4 Code 5 Results 5.1 Effectiveness of Debate 5.2 Performance Degradation during Debate 6 Failure Modes of Debate 6.1 Does exchange of reasoning help in sequential revision? 6.2 Are agents influenced by social factors? 6.3 Are agents sycophantic? Correctness payoff prompt. 6.4 Influence of Model and Task Type 7 Discussion References License: CC BY 4.0 arXiv:2509.05396v2 [cs.CL] 13 Oct 2025 Talk Isn’t Always Cheap: Understanding Failure Modes in Multi-Agent Debate Andrea Wynn Department of Computer Science Johns Hopkins University awynn13@jhu.edu Harsh Satija 1 1 footnotemark: 1 Vector Institute Gillian K. Hadfield Department of Computer Science Johns Hopkins University equal contribution Abstract While multi-agent debate has been proposed as a promising strategy for improving AI reasoning ability, we find that debate can sometimes be harmful rather than helpful. Prior work has primarily…

**Method / approach.** method for the scalable oversight problem where a judge or verifier can interject and elicit hidden contradictions, using structured back-and-forth conversations (Irving et al., 2018 ; Khan et al., 2024 ; Michael et al., 2023 ; Kenton et al., 2024 ) . More recently, another form of multi-agent debate, sometimes referred to as multi-agent deliberation, investigates leveraging different LLM agents to surface better answers by having them exchange reasoning via iterative discussion (Chan et al., 2023 ; Liang et al., 2023 ; Subramaniam et al., 2025 ) . Most of these studies focus on a homogeneous setting where all LLM agents utilize the same underlying language model (Du et al., 2023 ) or a model of similar ability (Yao et al., 2025 ) , finding that this approach enhances accuracy across various Question-Answering (QA) tasks. Estornell and Liu ( 2024 ) examine the theoretical properties and effects of opinion diversity within the debate framework, reporting a “tyranny of the majority”…

**Results.** Experimental Setup 4.1 Datasets 4.2 Models 4.3 Prompts 4.4 Code 5 Results 5.1 Effectiveness of Debate 5.2 Performance Degradation during Debate 6 Failure Modes of Debate 6.1 Does exchange of reasoning help in sequential revision? 6.2 Are agents influenced by social factors? 6.3 Are agents sycophantic? Correctness payoff prompt. 6.4 Influence of Model and Task Type 7 Discussion References License: CC BY 4.0 arXiv:2509.05396v2 [cs.CL] 13 Oct 2025 Talk Isn’t Always Cheap: Understanding Failure Modes in Multi-Agent Debate Andrea Wynn Department of Computer Science Johns Hopkins University awynn13@jhu.edu Harsh Satija 1 1 footnotemark: 1 Vector Institute Gillian K. Hadfield Department of Computer Science Johns Hopkins University equal contribution Abstract While multi-agent debate has been proposed as a promising strategy for improving AI reasoning ability, we find t…

**Conclusion.** conclusions. Yet, debates between LLM agents often fail to reach majority agreement on the true answer, even when at least one agent is initially correct. Examining why these failures occur is crucial for both understanding and designing these systems. We show that there are many other factors influencing failure modes of debate, which we explore in depth in this section. This suggests a richer and more complex interplay of factors influencing the effectiveness of debate. In this section, we dissect these dynamics empirically, examining when and how agents revise their answers, what social conditions are correlated with undesirable answer revisions, and whether an explicit intervention targeting sycophancy can meaningfully improve debate pe…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2509.05396v2.md` · `raw/arxiv/2509.05396v2.fulltext.md`
