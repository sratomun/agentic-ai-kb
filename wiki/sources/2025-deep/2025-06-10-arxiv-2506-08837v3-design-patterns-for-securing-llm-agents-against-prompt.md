---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Design Patterns for Securing LLM Agents against Prompt Injections"
authors: Luca Beurer-Kellner, Beat Buesser, Ana-Maria Creţu, Edoardo Debenedetti et al.
url: https://arxiv.org/abs/2506.08837v3
date: 2025-06-10
citationCount: 54
influentialCitationCount: 4
velocity: 4.36
ingested: 2026-06-22
tags: [agent-security, agentic-ai, arxiv, 2025, cited]
---

# Design Patterns for Securing LLM Agents against Prompt Injections

**arXiv [2506.08837v3](https://arxiv.org/abs/2506.08837v3)** · 2025-06-10 · **54 citations** (4 influential · 4.36/mo) · Luca Beurer-Kellner, Beat Buesser, Ana-Maria Creţu, Edoardo Debenedetti et al.

## Abstract
As AI agents powered by Large Language Models (LLMs) become increasingly versatile and capable of addressing a broad spectrum of tasks, ensuring their security has become a critical challenge. Among the most pressing threats are prompt injection attacks, which exploit the agent's resilience on natural language inputs -- an especially dangerous threat when agents are granted tool access or handle sensitive information. In this work, we propose a set of principled design patterns for building AI agents with provable resistance to prompt injection. We systematically analyze these patterns, discuss their trade-offs in terms of utility and security, and illustrate their real-world applicability through a series of case studies.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Background 3 Design Patterns for Securing LLM Agents Against Prompt Injections 3.1 Design Patterns for Securing LLM Agents 1) The Action-Selector Pattern. 2) The Plan-Then-Execute Pattern. 3) The LLM Map-Reduce Pattern. 4) The Dual LLM Pattern 5) The Code-Then-Execute Pattern. 6) The Context-Minimization pattern. 4 Case Studies 4.1 OS Assistant with Fuzzy Search 4.1.1 Threat Model 4.1.2 Possible Designs 1) LLM in the shell. 2) User confirmation. 3) The action-selector pattern. 4) The plan-then-execute pattern. 5) The dual LLM / map-reduce pattern. 4.2 SQL Agent 4.2.1 Description 4.2.2 Threat Model 4.2.3 Possible Designs 1) No AI security. 2) Plan-Then-Execute for Processing Data from Databases. 3) Action-sandboxing for the Python interpreter. 4) Ask-the-user / Guardrailing the LLMs. 4.3 Email and Calendar Assistant 4.3.1 Description 4.3.2 Threat Model 4.3.3 Possible Designs 1) User confirmation. 2) Plan-then-execute/Code-then-execute. 3) Dual LLM pattern. 4.4 Customer se…

**Method / approach.** approaches like detection and adversarial training (Wallace et al., 2024 ; Chen et al., 2024 ; Zverev et al., 2024 ; Willison, 2023a ; Yi et al., 2023 ; Zou et al., 2024 ) , to principled system-level isolation mechanisms (Bagdasarian et al., 2024 ; Balunovic et al., 2024 ; Abdelnabi et al., 2025b ; Willison, 2023b ; Wu et al., 2025 ; Debenedetti et al., 2025 ) . These proposals are primarily generic, aiming to design safe general-purpose agents. In this work, we describe a number of design patterns for LLM agents that significantly mitigate the risk of prompt injections. These design patterns constrain the actions of agents to explicitly prevent them from solving arbitrary tasks. We believe these design patterns offer a valuable trade-off between agent utility and security. To illustrate the broad applicability of these design patterns, we apply them to ten case studies of LLM agent applications, spanning from simple OS function assistants to more general software engineering ag…

**Conclusion.** Conclusions Recommendations 6 Acknowledgments A Best Practices for LLM Agent Security Design Patterns for Securing LLM Agents against Prompt Injections Luca Beurer-Kellner 1 1 1 Alphabetical author ordering. Corresponding author: florian.tramer@inf.ethz.ch Invariant Labs Beat Buesser IBM Ana-Maria Creţu EPFL Edoardo Debenedetti ETH Zurich Daniel Dobos Swisscom Daniel Fabian Google Marc Fischer Invariant Labs David Froelicher Swisscom Kathrin Grosse IBM Daniel Naeff ETH AI Center Ezinwanne Ozoani AppliedAI Institute for Europe Andrew Paverd Microsoft Florian Tramèr ETH Zurich Václav Volhejn 2 2 2 Work done while at Lakera. Kyutai Abstract As AI agents powered by Large Language Models (L…

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2506.08837v3.md` · `raw/arxiv/2506.08837v3.fulltext.md`
