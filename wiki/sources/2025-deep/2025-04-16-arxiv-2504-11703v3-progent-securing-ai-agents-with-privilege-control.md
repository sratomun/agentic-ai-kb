---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Progent: Securing AI Agents with Privilege Control"
authors: Tianneng Shi, Jingxuan He, Zhun Wang, Hongwei Li et al.
url: https://arxiv.org/abs/2504.11703v3
date: 2025-04-16
citationCount: 70
influentialCitationCount: 10
velocity: 4.93
ingested: 2026-06-22
tags: [agent-security, tool-use, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Progent: Securing AI Agents with Privilege Control

**arXiv [2504.11703v3](https://arxiv.org/abs/2504.11703v3)** · 2025-04-16 · **70 citations** (10 influential · 4.93/mo) · Tianneng Shi, Jingxuan He, Zhun Wang, Hongwei Li et al.

## Abstract
AI agents interact with external environments through tool calls, exposing them to attacks like indirect prompt injection that can trigger unauthorized actions. Securing these agents is challenging: they behave autonomously and probabilistically, security requirements evolve depending on the user's task and execution state, and there is an inherent tradeofff between security and utility. In this work, we introduce Progent, a novel framework that secures AI agents via privilege control. Progent represents privilege as a security policy consisting of symbolic rules over tool names and arguments. These rules specify which tool calls are allowed for task completion and which unnecessary ones are blocked for security. Every tool call is checked against such a policy through a deterministic procedure, enforcing the principle of least privilege. To handle diverse user tasks and evolving execution contexts, an LLM automatically generates the initial policy from the user's task and updates it during execution as new information arrives. Each proposed update is determined by an SMT solver to be either a narrowing (applied automatically) or an expansion (requiring explicit approval), ensuring that the agent's effective action space can only shrink without approval (monotonic confinement). This deterministic update mechanism preserves utility and prevents silent privilege escalation, even when adversarial inputs are present. Our evaluation on popular benchmarks (i.e., AgentDojo and ASB) shows that Progent significantly reduces attack success rates while maintaining high utility. We further validate Progent's practicality by showcasing its effectiveness in real-world agent frameworks such as LangChain and OpenAI Agents SDK.

## From the paper (full-text excerpts)
**Introduction.** Introduction Security Risks in AI Agents Challenges for Securing AI Agents Our Work: Progent Implementation and Evaluation Main Contributions 2 Overview 2.1 Challenges for Agent Security Motivating Example: Agent Execution and Attack. Challenge I: Non-Deterministic Agent Behavior Challenge II: Context-Dependent Security Requirements Challenge III: Balancing Security and Utility 2.2 Progent: Defense via Privilege Control Policy-Based Security Enforcement LLM-Based Policy Construction and Update Deterministic Control of Policy Expansion and Narrowing Progent’s Security Guarantee 3 Problem Statement and Threat Model 3.1 AI Agents 3.2 Threat Model Attacker Goal Attacker Capabilities Progent’s Defense Scope 4 Progent’s Privilege Control Policy 4.1 Policy Definition Effect and Conditions Fallback Action 4.2 Policy Runtime 4.3 Policy Comparison via SMT Solving 5 Securing Agent Execution with Progent Agent Execution Loop with Progent Initial Policy Generation Policy Update 6 Progent’s Security Guarante…

**Method / approach.** methodologies Artificial intelligence 1. Introduction AI agents have emerged as a promising platform for general and autonomous task solving (Wang et al . , 2024b ; Shi et al . , 2024 ; Wang et al . , 2024a ; Yao et al . , 2023 ) . At the core of these agents is a large language model (LLM), which interacts with the external environment through diverse sets of tools (Schick et al . , 2023 ; Qin et al . , 2023 ) . For instance, a personal assistant agent uses email toolkits (LangChain, 2025a ) to manage emails, and a coding agent uses code interpreters and the command line (Wang et al . , 2024a ) . Security Risks in AI Agents The ability to interact with external environments makes AI agents powerful, enabling them to perform diverse tasks across domains such as communication, scheduling, and finance. However, this same ability also creates a large attack surface. Recent research has raised serious security concerns about AI agents (Li et al . , 2024b ; He et al . , 20…

**Results.** Experimental Evaluation 8.1 Progent’s General Effectiveness Evaluation Setup AgentDojo ASB 8.2 Ablation Studies Different Approver Configurations Different Model Choices 8.3 Real-World Agents Integration MCP-Based Benchmark Real-World Agents Multi-Agent Systems 9 Limitation and Discussion User Mistakes Defense Scope Extension to Multimodal Agents 10 Related Work Security Policy Languages System-Level Defenses for Agents. Model-Level Prompt Injection Defenses 11 Conclusion References A Open Science B Ethical Considerations C Sample policies D Experiment Details E Adaptive Attacks F Integration Details Library Mode Proxy Mode G Prompts License: arXiv.org perpetual non-exclusive license arXiv:2504.11703v3 [cs.CR] 14 May 2026 Progent: Securing AI Agents with Privilege Control Tianneng Shi 1 , Jingxuan He 1 , Zhun Wang 1 , Hongwei Li 2 , Linyu Wu 3 , We…

**Conclusion.** Conclusion References A Open Science B Ethical Considerations C Sample policies D Experiment Details E Adaptive Attacks F Integration Details Library Mode Proxy Mode G Prompts License: arXiv.org perpetual non-exclusive license arXiv:2504.11703v3 [cs.CR] 14 May 2026 Progent: Securing AI Agents with Privilege Control Tianneng Shi 1 , Jingxuan He 1 , Zhun Wang 1 , Hongwei Li 2 , Linyu Wu 3 , Wenbo Guo 2 , Dawn Song 1 1 UC Berkeley 2 UC Santa Barbara 3 National University of Singapore Abstract. AI agents interact with external environments through tool calls, exposing them to attacks like indirect prompt injection that can trigger unauthorized actions. Securing these agents is challenging: they behave aut…

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.11703v3.md` · `raw/arxiv/2504.11703v3.fulltext.md`
