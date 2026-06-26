---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Defeating Prompt Injections by Design"
authors: Edoardo Debenedetti, Ilia Shumailov, Tianqi Fan, Jamie Hayes et al.
url: https://arxiv.org/abs/2503.18813v2
date: 2025-03-24
citationCount: 156
influentialCitationCount: 18
velocity: 10.44
ingested: 2026-06-22
tags: [agent-security, agentic-ai, arxiv, 2025, cited]
---

# Defeating Prompt Injections by Design

**arXiv [2503.18813v2](https://arxiv.org/abs/2503.18813v2)** · 2025-03-24 · **156 citations** (18 influential · 10.44/mo) · Edoardo Debenedetti, Ilia Shumailov, Tianqi Fan, Jamie Hayes et al.

## Abstract
Large Language Models (LLMs) are increasingly deployed in agentic systems that interact with an untrusted environment. However, LLM agents are vulnerable to prompt injection attacks when handling untrusted data. In this paper we propose CaMeL, a robust defense that creates a protective system layer around the LLM, securing it even when underlying models are susceptible to attacks. To operate, CaMeL explicitly extracts the control and data flows from the (trusted) query; therefore, the untrusted data retrieved by the LLM can never impact the program flow. To further improve security, CaMeL uses a notion of a capability to prevent the exfiltration of private data over unauthorized data flows by enforcing security policies when tools are called. We demonstrate effectiveness of CaMeL by solving $77\%$ of tasks with provable security (compared to $84\%$ with an undefended system) in AgentDojo. We release CaMeL at https://github.com/google-research/camel-prompt-injection.

## From the paper (full-text excerpts)
**Introduction.** Introduction Large Language Models (LLMs) are increasingly used as the core of modern agentic systems (Wooldridge and Jennings, 1995) interacting with external environments via APIs and user interfaces (Nakano et al., 2021; Thoppilan et al., 2022; Schick et al., 2023; Yao et al., 2022; Qin et al., 2023; Lu et al., 2024; Gao et al., 2023; Shen et al., 2024). This exposes them to prompt injection attacks (Goodside, 2022; Perez and Ribeiro, 2022; Greshake et al., 2023) when data or instructions come from untrusted sources (e.g., from a compromised user, from tool call outputs, or from a web page). In these attacks, adversaries insert malicious instructions into the LLM’s context, aiming to exfiltrate data or cause harmful actions (Rehberger, 2024; AI-Security-Team et al., 2025; Anthropic, 2025; OpenAI, 2025). Current defenses often rely on training or prompting models to adhere to security policies (Wallace et al., 2024; Ghalebikesabi et al., 2024), frequently implemented as vulnerable system prompts (Carlini et al., 2023). This is largely due to the absence of robust methods to formall…

**Method / approach.** methods to formally define and enforce security policies for LLM functionalities on diverse data. This work introduces a novel defense, CaMeL1 , inspired by traditional software security concepts like Control Flow Integrity (Abadi et al., 2009), Access Control (Anderson, 2010, Chap. 6), and Information Flow Control (Denning and Denning, 1977). CaMeL effectively mitigates dangerous outcomes of prompt injection attacks, as demonstrated by practically solving the security evaluation of the AgentDojo benchmark (Debenedetti et al., 2024b). CaMeL associates, to every value, some metadata (commonly called capabilities2 in the software security literature) to restrict data and control flows, giving the possibility to express what can and cannot be done with each individual value by using fine-grained security policies. CaMeL operates by extracting control and data flows from user queries and employs a custom Python interpreter to enforce security policies, providing security guarantees withou…

**Results.** experiments where we employed more recent models. For example, OpenAI’s o3 has around 10% more utility than o1, which is less than four months older than o3. 6.1.2. How does CaMeL impact utility? To better understand the impact of CaMeL on utility, we analyze the failure modes of Claude 3.5 Sonnet across the different task suites. We pick Claude 3.5 Sonnet due to relatively high performance across all of the tasks. We categorize failures and show the amount for each category in Table 1. Table 14 in Appendix G provides a breakdown of Claude’s failures for each task. Appendix H.4 provides examples of failed tasks with the description of the failure and the whole agent interaction. We now discuss the failure modes related to the nature of CaMeL. The P-LLM cannot write a plan based on data it can’t read. One failure mode that is inherent to CaMeL (and in general to the Dual LLM Pattern) is what we call the “Data requires action” failure, wh…

**Conclusion.** limitations, some of which are explicitly outside of scope. CaMeL doesn’t aim to defend against attacks that do not affect the control nor the data flow. In particular, we recognize that it cannot defend against text-to-text attacks which have no consequences on the data flow, e.g., an attack prompting the assistant to summarize an email to something different than the actual content of the email, as long as this doesn’t cause the exfiltration of private data. This also includes prompt-injection induced phishing (e.g., “You received an email from Google saying you should click on this (malicious) link to not lose your account”). Nonetheless, CaMeL’s data flow graph enables tracing the origin of the content shown to the user. This can be lev…

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2503.18813v2.md` · `raw/arxiv/2503.18813v2.fulltext.md`
