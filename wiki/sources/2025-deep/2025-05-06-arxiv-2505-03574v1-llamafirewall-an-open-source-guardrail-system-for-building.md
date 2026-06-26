---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "LlamaFirewall: An open source guardrail system for building secure AI agents"
authors: Sahana Chennabasappa, Cyrus Nikolaidis, Daniel Song, David Molnar et al.
url: https://arxiv.org/abs/2505.03574v1
date: 2025-05-06
citationCount: 81
influentialCitationCount: 8
velocity: 5.98
ingested: 2026-06-22
tags: [coding-agents, agent-security, multi-agent-systems, governance-gap, agentic-ai, arxiv, 2025, cited]
---

# LlamaFirewall: An open source guardrail system for building secure AI agents

**arXiv [2505.03574v1](https://arxiv.org/abs/2505.03574v1)** · 2025-05-06 · **81 citations** (8 influential · 5.98/mo) · Sahana Chennabasappa, Cyrus Nikolaidis, Daniel Song, David Molnar et al.

## Abstract
Large language models (LLMs) have evolved from simple chatbots into autonomous agents capable of performing complex tasks such as editing production code, orchestrating workflows, and taking higher-stakes actions based on untrusted inputs like webpages and emails. These capabilities introduce new security risks that existing security measures, such as model fine-tuning or chatbot-focused guardrails, do not fully address. Given the higher stakes and the absence of deterministic solutions to mitigate these risks, there is a critical need for a real-time guardrail monitor to serve as a final layer of defense, and support system level, use case specific safety policy definition and enforcement. We introduce LlamaFirewall, an open-source security focused guardrail framework designed to serve as a final layer of defense against security risks associated with AI Agents. Our framework mitigates risks such as prompt injection, agent misalignment, and insecure code risks through three powerful guardrails: PromptGuard 2, a universal jailbreak detector that demonstrates clear state of the art performance; Agent Alignment Checks, a chain-of-thought auditor that inspects agent reasoning for prompt injection and goal misalignment, which, while still experimental, shows stronger efficacy at preventing indirect injections in general scenarios than previously proposed approaches; and CodeShield, an online static analysis engine that is both fast and extensible, aimed at preventing the generation of insecure or dangerous code by coding agents. Additionally, we include easy-to-use customizable scanners that make it possible for any developer who can write a regular expression or an LLM prompt to quickly update an agent's security guardrails.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Prompt Injection and Guardrail Systems 2.2 Static Analysis of LLM-Generated Code 2.3 Alignment and Agent Behavior Monitoring 2.4 Open-Source vs. Proprietary Approaches 3 LLamaFirewall workflow and detection components 3.1 Scenario 1: Preventing Goal Hijacking and Data Exfiltration 3.2 Scenario 2: Preventing Accidental SQL Injection in Code Generation 4 LlamaFirewall Scanners: Design and Evaluation 4.1 PromptGuard 2 4.2 AlignmentCheck 4.3 Evaluating Combined Prompt Injection Defenses with PromptGuard and AlignmentCheck 4.3.1 Experimental Setup 4.3.2 Results 4.4 CodeShield 5 Limitations and future Work 6 Conclusion 7 Acknowledgements A Prompt Injection Evaluation Dataset A.1 Tool-use agentic prompt injection benchmark A.2 Direct Jailbreak Evaluation Dataset B PromptGuard 2 B.1 Development Methodology B.2 Evaluating PromptGuard in an Agentic Environment C AlignmentCheck C.1 Implementation Methodology C.1.1 AlignmentCheck Input Structure C.1.2 Prompt and Generalization C.1…

**Method / approach.** Methodology B.2 Evaluating PromptGuard in an Agentic Environment C AlignmentCheck C.1 Implementation Methodology C.1.1 AlignmentCheck Input Structure C.1.2 Prompt and Generalization C.1.3 Effectiveness of Alignment Checks C.2 Comparison of Effectiveness of diffent Llama Models backing AlignmentCheck C.3 Recommended Use Cases C.4 Limitations and Risks C.5 Example Trace C.6 AlignmentCheck System and User Prompts \metadata [Author Legend] *Co-equal primary author, †Contributor \correspondence Joshua Saxe at \metadata [Code] https://github.com/meta-llama/PurpleLlama/tree/main/LlamaFirewall \metadata [Blogpost] https://ai.meta.com/blog/ai-defenders-program-llama-protection-tools/ LlamaFirewall: An open source guardrail system for building secure AI agents Sahana Chennabasappa Cyrus Nikolaidis Daniel Song David Molnar Stephanie Ding Shengye Wan Spencer Whitman Lauren Deason Nicholas Doucette Abraham Montilla Alekhya Gampa…

**Results.** Experimental Setup 4.3.2 Results 4.4 CodeShield 5 Limitations and future Work 6 Conclusion 7 Acknowledgements A Prompt Injection Evaluation Dataset A.1 Tool-use agentic prompt injection benchmark A.2 Direct Jailbreak Evaluation Dataset B PromptGuard 2 B.1 Development Methodology B.2 Evaluating PromptGuard in an Agentic Environment C AlignmentCheck C.1 Implementation Methodology C.1.1 AlignmentCheck Input Structure C.1.2 Prompt and Generalization C.1.3 Effectiveness of Alignment Checks C.2 Comparison of Effectiveness of diffent Llama Models backing AlignmentCheck C.3 Recommended Use Cases C.4 Limitations and Risks C.5 Example Trace C.6 AlignmentCheck System and User Prompts \metadata [Author Legend] *Co-equal primary author, †Contributor \correspondence Joshua Saxe at \metadata [Code] https://github.com/meta-llama/PurpleLlama/tree/main/LlamaFirewall \metadata [Blogpost]…

**Conclusion.** Conclusion 7 Acknowledgements A Prompt Injection Evaluation Dataset A.1 Tool-use agentic prompt injection benchmark A.2 Direct Jailbreak Evaluation Dataset B PromptGuard 2 B.1 Development Methodology B.2 Evaluating PromptGuard in an Agentic Environment C AlignmentCheck C.1 Implementation Methodology C.1.1 AlignmentCheck Input Structure C.1.2 Prompt and Generalization C.1.3 Effectiveness of Alignment Checks C.2 Comparison of Effectiveness of diffent Llama Models backing AlignmentCheck C.3 Recommended Use Cases C.4 Limitations and Risks C.5 Example Trace C.6 AlignmentCheck System and User Prompts \metadata [Author Legend] *Co-equal primary author, †Contributor \correspondence Joshua Saxe at…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]] · [[governance-gap|Governance gap]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2505.03574v1.md` · `raw/arxiv/2505.03574v1.fulltext.md`
