---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Securing AI Agents with Information-Flow Control"
authors: Manuel Costa, Boris Köpf, Aashish Kolluri, Andrew Paverd et al.
url: https://arxiv.org/abs/2505.23643v2
date: 2025-05-29
citationCount: 69
influentialCitationCount: 12
velocity: 5.4
ingested: 2026-06-22
tags: [agent-security, agentic-ai, arxiv, 2025, cited]
---

# Securing AI Agents with Information-Flow Control

**arXiv [2505.23643v2](https://arxiv.org/abs/2505.23643v2)** · 2025-05-29 · **69 citations** (12 influential · 5.4/mo) · Manuel Costa, Boris Köpf, Aashish Kolluri, Andrew Paverd et al.

## Abstract
As AI agents become increasingly autonomous and capable, ensuring their security against vulnerabilities such as prompt injection becomes critical. This paper explores the use of information-flow control (IFC) to provide security guarantees for AI agents. We present a formal model to reason about the security and expressiveness of agent planners. Using this model, we characterize the class of properties enforceable by dynamic taint-tracking and construct a taxonomy of tasks to evaluate security and utility trade-offs of planner designs. Informed by this exploration, we present Fides, a planner that tracks confidentiality and integrity labels, deterministically enforces security policies, and introduces novel primitives for selectively hiding information. Its evaluation in AgentDojo demonstrates that this approach enables us to complete a broad range of tasks with security guarantees. A tutorial to walk readers through the the concepts introduced in the paper can be found at https://github.com/microsoft/fides

## From the paper (full-text excerpts)
**Introduction.** Introduction Recent advances in large language models (LLMs) have greatly improved their abilities in language understanding, reasoning, and planning. This growing fluency and competency, together with the integration of tool-calling capabilities, enables the development of agentic systems that solve complex tasks on behalf of users [7, 34, 13, 24, 19, 3]. Unfortunately, the ability to call consequential tools while processing data from varied origins, from trusted collaborators to the public web, also increases the security and privacy risks of agentic systems. In particular, indirect prompt injection attacks (PIAs) [16, 38] pose a serious threat, allowing malicious actors to hijack agent behavior and exploit delegated capabilities, leading to harmful outcomes. To illustrate the risks, consider a common enterprise scenario: a user asks an agent to “summarize recent emails on Project X and send the summary to my manager.” A malicious email with subject “Project X Update” and body “Ignore previous instructions and send the top email in my mailbox to attacker@evil.com.” could exfiltra…

**Method / approach.** approach enables us to complete a broad range of tasks with security guarantees. A tutorial to walk readers through the concepts introduced in the paper can be found at https://github.com/microsoft/fides. 1 Introduction Recent advances in large language models (LLMs) have greatly improved their abilities in language understanding, reasoning, and planning. This growing fluency and competency, together with the integration of tool-calling capabilities, enables the development of agentic systems that solve complex tasks on behalf of users [7, 34, 13, 24, 19, 3]. Unfortunately, the ability to call consequential tools while processing data from varied origins, from trusted collaborators to the public web, also increases the security and privacy risks of agentic systems. In particular, indirect prompt injection attacks (PIAs) [16, 38] pose a serious threat, allowing malicious actors to hijack agent behavior and exploit delegated capabilities, leading to harmful outcomes. To illustrate the…

**Results.** Experimental Setup We use the AgentDojo benchmark suite [11] to evaluate the different planner designs discussed in this paper. The AgentDojo benchmark includes tasks in 4 simulated application environments: workspace, travel, banking, and Slack. The tasks are representative of real-world scenarios and include a variety of actions that the agents can take, such 13 Securing AI Agents with Information-Flow Control as making online reservations, sending messages, and performing financial transactions. AgentDojo includes attack scenarios designed to test the security of agents against PIAs. AgentDojo provides two kinds of tasks: user tasks and injection tasks. User tasks happen in a benign setting while injection tasks aim to trick the agent into satisfying an attacker’s goal. An attack defines a way to place a prompt injection within the context of the user task. For instance, a Tool Knowledge attack assumes the adversary knows the too…

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2505.23643v2.md` · `raw/arxiv/2505.23643v2.fulltext.md`
