---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Prompt Flow Integrity to Prevent Privilege Escalation in LLM Agents"
authors: Juhee Kim, Woohyuk Choi, Byoungyoung Lee
url: https://arxiv.org/abs/2503.15547v2
date: 2025-03-17
citationCount: 57
influentialCitationCount: 4
velocity: 3.76
ingested: 2026-06-22
tags: [agent-security, agentic-ai, arxiv, 2025, cited]
---

# Prompt Flow Integrity to Prevent Privilege Escalation in LLM Agents

**arXiv [2503.15547v2](https://arxiv.org/abs/2503.15547v2)** · 2025-03-17 · **57 citations** (4 influential · 3.76/mo) · Juhee Kim, Woohyuk Choi, Byoungyoung Lee

## Abstract
Large Language Models (LLMs) are combined with tools to create powerful LLM agents that provide a wide range of services. Unlike traditional software, LLM agent's behavior is determined at runtime by natural language prompts from either user or tool's data. This flexibility enables a new computing paradigm with unlimited capabilities and programmability, but also introduces new security risks, vulnerable to privilege escalation attacks. Moreover, user prompts are prone to be interpreted in an insecure way by LLM agents, creating non-deterministic behaviors that can be exploited by attackers. To address these security risks, we propose Prompt Flow Integrity (PFI), a system security-oriented solution to prevent privilege escalation in LLM agents. Analyzing the architectural characteristics of LLM agents, PFI features three mitigation techniques -- i.e., agent isolation, secure untrusted data processing, and privilege escalation guardrails. Our evaluation result shows that PFI effectively mitigates privilege escalation attacks while successfully preserving the utility of LLM agents.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 LLM Agents 3 Motivation 3.1 Threat Model 3.2 Privilege Escalation Attacks 3.2.1 Prompt Injection Attack 3.2.2 Data Injection Attack 3.3 Previous Defenses 4 Prompt Flow Integrity 4.1 Agent Isolation 4.2 Secure Untrusted Data Processing 4.3 Privilege Escalation Guardrails 4.4 Prompt Flow Policy 5 Evaluation 5.1 Evaluation Setup 5.2 Evaluation Results 6 Discussion 7 Conclusion A Policies A.1 Access Token Privilege A.2 Data Trust Policy B Evaluation Details B.1 Benchmark Suites B.2 Full Performance Evaluation Results C PFI System Prompts \WarningFilter *captionUnsupported document class \mdfdefinestyle AddFramenobreak=true, linewidth=0pt, innertopmargin=0pt, innerbottommargin=0pt, innerrightmargin=0pt, innerleftmargin=0pt, Prompt Flow Integrity to Prevent Privilege Escalation in LLM Agents Juhee Kim Seoul National University kimjuhi96@snu.ac.kr Co-first author Woohyuk Choi 1 1 footnotemark: 1 Seoul National University 00cwooh@snu.ac.kr Byoungyoung Lee Seoul National Univers…

**Method / approach.** approaches to secure LLM agents against prompt injection attacks. \IfEndWith ML-based Defenses.ML-based DefensesML-based Defenses. ML-based defenses enforce security guidelines on LLM agents based on model fine-tuning or in-context learning. Fine-tuning the LLM model with security guidelines (e.g., adhering to user prompts, and avoiding harmful responses) can improve the agent’s robustness against malicious data [ 29 , 36 , 60 , 11 ] . In-context learning approaches guide the agent to adhere to security policies by system prompts [ 55 , 63 ] . However, both fine-tuning and in-context learning align the agent’s behavior only probabilistically, and thus can be bypassed [ 62 , 64 , 33 , 61 ] . \IfEndWith Secure Agent Designs.Secure Agent DesignsSecure Agent Designs. Several approaches proposed secure agent designs [ 7 , 57 , 58 ] , which divide an agent into trusted and untrusted parts, isolating untrusted data from privileged operations, providing more deterministic sec…

**Results.** Evaluation 5.1 Evaluation Setup 5.2 Evaluation Results 6 Discussion 7 Conclusion A Policies A.1 Access Token Privilege A.2 Data Trust Policy B Evaluation Details B.1 Benchmark Suites B.2 Full Performance Evaluation Results C PFI System Prompts \WarningFilter *captionUnsupported document class \mdfdefinestyle AddFramenobreak=true, linewidth=0pt, innertopmargin=0pt, innerbottommargin=0pt, innerrightmargin=0pt, innerleftmargin=0pt, Prompt Flow Integrity to Prevent Privilege Escalation in LLM Agents Juhee Kim Seoul National University kimjuhi96@snu.ac.kr Co-first author Woohyuk Choi 1 1 footnotemark: 1 Seoul National University 00cwooh@snu.ac.kr Byoungyoung Lee Seoul National University byoungyoung@snu.ac.kr Abstract Large Language Models (LLMs) are combined with tools to create powerful LLM agents that provide a wide range of services. Unlike traditional software, LLM agen…

**Conclusion.** Conclusion A Policies A.1 Access Token Privilege A.2 Data Trust Policy B Evaluation Details B.1 Benchmark Suites B.2 Full Performance Evaluation Results C PFI System Prompts \WarningFilter *captionUnsupported document class \mdfdefinestyle AddFramenobreak=true, linewidth=0pt, innertopmargin=0pt, innerbottommargin=0pt, innerrightmargin=0pt, innerleftmargin=0pt, Prompt Flow Integrity to Prevent Privilege Escalation in LLM Agents Juhee Kim Seoul National University kimjuhi96@snu.ac.kr Co-first author Woohyuk Choi 1 1 footnotemark: 1 Seoul National University 00cwooh@snu.ac.kr Byoungyoung Lee Seoul National University byoungyoung@snu.ac.kr Abstract Large Language Models (LLMs) are combine…

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2503.15547v2.md` · `raw/arxiv/2503.15547v2.fulltext.md`
