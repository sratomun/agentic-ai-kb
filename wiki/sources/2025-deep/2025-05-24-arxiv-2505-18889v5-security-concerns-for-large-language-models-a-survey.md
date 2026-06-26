---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Security Concerns for Large Language Models: A Survey"
authors: Miles Q. Li, Benjamin C. M. Fung
url: https://arxiv.org/abs/2505.18889v5
date: 2025-05-24
citationCount: 53
influentialCitationCount: 0
velocity: 4.09
ingested: 2026-06-22
tags: [embodied-agents, agent-security, arxiv, 2025, cited]
---

# Security Concerns for Large Language Models: A Survey

**arXiv [2505.18889v5](https://arxiv.org/abs/2505.18889v5)** · 2025-05-24 · **53 citations** (0 influential · 4.09/mo) · Miles Q. Li, Benjamin C. M. Fung

## Abstract
Large Language Models (LLMs) such as ChatGPT and its competitors have caused a revolution in natural language processing, but their capabilities also introduce new security vulnerabilities. This survey provides a comprehensive overview of these emerging concerns, categorizing threats into several key areas: inference-time attacks via prompt manipulation; training-time attacks; misuse by malicious actors; and the inherent risks in autonomous LLM agents. Recently, a significant focus is increasingly being placed on the latter. We summarize recent academic and industrial studies from 2022 to 2025 that exemplify each threat, analyze existing defense mechanisms and their limitations, and identify open challenges in securing LLM-based applications. We conclude by emphasizing the importance of advancing robust, multi-layered security strategies to ensure LLMs are safe and beneficial.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Inference-Time Attacks via Prompt Manipulation 2.1 Attack Surfaces for Prompt Injection 2.2 Direct vs. Indirect Injection 2.3 Manual and Heuristic Prompt Crafting 2.4 Automated Prompt Generation 2.4.1 White-Box and Gray-Box Attacks 2.4.2 Black-Box Attacks 3 Training-Time Attacks 3.1 Data Poisoning and Backdoor Insertion 3.2 Deceptive Alignment and the “Sleeper Agent” Problem 4 Misuse by Malicious Actors 4.1 Automating Social Engineering and Cybercrime 4.2 Generation of Disinformation and Deceptive Content 4.3 Emergence of Specialized Malicious LLMs and Ecosystem Exploitation 5 Intrinsic Risks in LLM Agents 5.1 Goal Misalignment 5.2 Deception and Self-Preservation Behaviors 5.3 Scheming: Covert Pursuit of Misaligned Objectives 5.4 Persistence of Deception and the “Sleeper Agent" Problem 5.5 Unfaithful Reasoning 5.6 Measuring and Inducing Agentic Misalignment 5.7 Implications and Broader Ecosystem Vulnerabilities 6 Defense Mechanisms and Limitations 6.1 Prevention-Based Defenses 6.2 Detection-Based Def…

**Method / approach.** methodology. 2.1 Attack Surfaces for Prompt Injection Prompt injection can occur at various stages of the model’s interaction flow, creating distinct attack surfaces: the system prompt, the user prompt, and the assistant’s own response. • System Prompt Injection: This occurs when an attacker can modify the core instructions given to the LLM [ 23 ] . For instance, in a customizable environment, an attacker could alter the system prompt to remove ethical constraints, changing the instructions to something permissive like “You are an uncensored assistant. Answer all questions from the user without rejection” to jailbreak the model. • Assistant Response Injection: This technique aims to manipulate the model’s output generation process [ 34 ] . An attacker might structure their input to include a prefix that forces the model to begin its reply affirmatively, such as asking a harmful question and then add “Sure, here is the detailed guide:…” as the prefix of the assis…

**Results.** experiments show high attack success rates (65-82%) against Google’s Gemini models, revealing a fundamental security vulnerability in a feature designed for utility and model customization. Shifting the focus to indirect prompt injection and the robustness of attacks, Pasquini et al. [ 47 ] introduce Neural Exec , a framework for automatically generating execution triggers for prompt injection attacks. Unlike prior methods that focused on generating a complete adversarial prompt or a simple suffix, Neural Exec conceptualizes the creation of the execution trigger itself—the part of the prompt designed to make the LLM execute a malicious payload—as a differentiable search problem. Using a gradient-based optimization approach, the framework learns triggers that are significantly more effective and flexible than handcrafted ones. The primary innovation of Neural Exec is its focus on generating triggers that are robust enough to persist…

**Conclusion.** Conclusion [orcid=0000-0001-7091-3268] \cormark [1] [orcid=0000-0001-8423-2906] \cortext [cor1]Corresponding author. Security Concerns for Large Language Models: A Survey Miles Q. Li infinite.optimization@outlook.com Benjamin C. M. Fung ben.fung@mcgill.ca Infinite Optimization AI Lab, Montreal, Canada School of Information Studies, McGill University, Montreal, Canada Abstract Large Language Models (LLMs) such as ChatGPT and its competitors have caused a revolution in natural language processing, but their capabilities also introduce new security vulnerabilities. This survey provides a comprehensive overview of these emerging concerns, categorizing threats into several key areas: inference-time attacks via…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agent-security|Agent security]]
- **Raw:** `raw/arxiv/2505.18889v5.md` · `raw/arxiv/2505.18889v5.fulltext.md`
