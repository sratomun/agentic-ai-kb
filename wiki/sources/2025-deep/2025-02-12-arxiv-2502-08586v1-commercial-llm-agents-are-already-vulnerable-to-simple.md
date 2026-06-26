---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Commercial LLM Agents Are Already Vulnerable to Simple Yet Dangerous Attacks"
authors: Ang Li, Yin Zhou, Vethavikashini Chithrra Raghuram, Tom Goldstein et al.
url: https://arxiv.org/abs/2502.08586v1
date: 2025-02-12
citationCount: 50
influentialCitationCount: 0
velocity: 3.07
ingested: 2026-06-22
tags: [agent-reliability, agent-security, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# Commercial LLM Agents Are Already Vulnerable to Simple Yet Dangerous Attacks

**arXiv [2502.08586v1](https://arxiv.org/abs/2502.08586v1)** · 2025-02-12 · **50 citations** (0 influential · 3.07/mo) · Ang Li, Yin Zhou, Vethavikashini Chithrra Raghuram, Tom Goldstein et al.

## Abstract
A high volume of recent ML security literature focuses on attacks against aligned large language models (LLMs). These attacks may extract private information or coerce the model into producing harmful outputs. In real-world deployments, LLMs are often part of a larger agentic pipeline including memory systems, retrieval, web access, and API calling. Such additional components introduce vulnerabilities that make these LLM-powered agents much easier to attack than isolated LLMs, yet relatively little work focuses on the security of LLM agents. In this paper, we analyze security and privacy vulnerabilities that are unique to LLM agents. We first provide a taxonomy of attacks categorized by threat actors, objectives, entry points, attacker observability, attack strategies, and inherent vulnerabilities of agent pipelines. We then conduct a series of illustrative attacks on popular open-source and commercial agents, demonstrating the immediate practical implications of their vulnerabilities. Notably, our attacks are trivial to implement and require no understanding of machine learning.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Taxonomy of Attacks on LLM Agents 2.1 Threat Actors 2.2 Attack Objectives 2.3 Entry Points in LLM Agents 2.4 Observability of Agent for Attackers 2.5 Attack Strategies 3 Breaking Commercial Web Agents 3.1 Stealing Users’ Private Information 3.2 Disrupting a User’s Local System 3.3 Manipulating a User’s Agent to Launch a Phishing Attack Against Their Own Contacts 4 Breaking Scientific Discovery Agents 4.1 Polluting Databases for Retrieval 4.2 Bypassing Agent Safeguards Through Obfuscation and Indirect References 5 Related Work 6 Discussion 6.1 Defenses 6.2 Opposing Views: Are Attacks on Agents Really a Problem? 6.3 Paths Forward Commercial LLM Agents Are Already Vulnerable to Simple Yet Dangerous Attacks Ang Li Yin Zhou Vethavikashini Chithrra Raghuram Tom Goldstein Micah Goldblum Abstract A high volume of recent ML security literature focuses on attacks against aligned large language models (LLMs). These attacks may extract private information or coerce the model into producing harmful outputs. In r…

**Method / approach.** method. Labeled as “the most efficient method” to synthesize the chemical, the document includes harmful modifications, such as procedures that could inadvertently produce hazardous substances. We then query the PaperQA agent for the optimal synthesis route, evaluating whether it would select the malicious document over legitimate alternatives. Results and observations. In our experiments, the agent retrieved the fabricated malicious document in all 100 100 100 100 out of 100 100 100 100 trials when specifically queried for the best synthesis route. This means that in every test case, when the PaperQA agent was asked how to synthesize a particular chemical, it prioritized and retrieved the malicious document over legitimate alternatives. Furthermore, in each trial using IUPAC nomenclature and indirect referencing, when queried for synthesis instructions, the ChemCrow agent reconstructs and outputs a step-by-step procedure leading to the production of nerve gas. This outcome undersc…

**Results.** experiments, we show instead that hand-crafted prompts which do not require any sophisticated optimizers or RL can be highly effective against existing agents. More sophisticated automated attack algorithms may be inapplicable to agents since they often require access to model outputs in order to provide signal to the optimizer. Designing such automated attacks on agents is an area for future work. See Section 5 for a further discussion of attacks on LLMs and agents and Section 6.1 for a discussion of defenses against attacks on agents. 3 Breaking Commercial Web Agents Web agents are among the most popular and powerful applications of LLM agents. Those powerful agents have attracted a lot of attention from both academia (Gur et al., 2023 ; He et al., 2024b ; Zhou et al., 2023 ) and industry (OpenAI, 2025 ; DeepMind, 2024 ; Anthropic, 2024 ; MultiOn, 2024 ; Putta et al., 2024 ) . They can process user queries, execute complex…

**Conclusion.** Discussion 6.1 Defenses 6.2 Opposing Views: Are Attacks on Agents Really a Problem? 6.3 Paths Forward Commercial LLM Agents Are Already Vulnerable to Simple Yet Dangerous Attacks Ang Li Yin Zhou Vethavikashini Chithrra Raghuram Tom Goldstein Micah Goldblum Abstract A high volume of recent ML security literature focuses on attacks against aligned large language models (LLMs). These attacks may extract private information or coerce the model into producing harmful outputs. In real-world deployments, LLMs are often part of a larger agentic pipeline including memory systems, retrieval, web access, and API calling. Such additional components introduce vulnerabilities that make these LLM-powered agents much easier to a…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2502.08586v1.md` · `raw/arxiv/2502.08586v1.fulltext.md`
