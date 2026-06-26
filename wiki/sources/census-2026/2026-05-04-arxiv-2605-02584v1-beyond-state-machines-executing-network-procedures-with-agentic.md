---
type: source
source_type: arxiv
title: "Beyond State Machines: Executing Network Procedures with Agentic Tool-Calling Sequences"
authors: Purna Sai Garigipati, Onur Ayan, Kishor Chandra Joshi, Xueli An
url: https://arxiv.org/abs/2605.02584v1
date: 2026-05-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.NI
tags: [agent-reliability, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# Beyond State Machines: Executing Network Procedures with Agentic Tool-Calling Sequences

**arXiv:** [2605.02584v1](https://arxiv.org/abs/2605.02584v1) · 2026-05-04 · cs.NI
**Authors:** Purna Sai Garigipati, Onur Ayan, Kishor Chandra Joshi, Xueli An

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic AI will be an essential enabling technology for designing future mobile communication systems, which could provide flexible and customized services, automate complex network operations, and drive autonomous decision-making across the network. This work studies how Large Language Model (LLM)-based network AI agents can be utilized to execute network procedures expressed as sequences of tool invocations. We investigate four approaches, which differ in how the agent obtains the procedure and in how execution is distributed between the agent and the underlying tools. We evaluated the latency and execution correctness across these approaches using a User Equipment (UE) IP allocation procedure as a case study. Furthermore, we conduct a stress test to examine how many sequential procedural steps an LLM agent can reliably execute before failure. Our results show that approaches relying on iterative agent-side reasoning incur higher latency and are more prone to execution errors, while approaches where the procedure is encapsulated within a single tool, which internally orchestrates the required steps by invoking other tools, reduce latency by limiting repeated reasoning. The stress-test results further show that the model with advanced tool-calling capability maintains reliable execution over longer procedures than the other evaluated models; however, all models exhibit reliability degradation as procedure length increases, revealing clear execution limits in multi-step tool-based workflows. To systematically analyze failures in procedure execution, we introduce a procedure-specific error taxonomy that categorizes deviations in multi-step procedural execution.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.02584v1)
