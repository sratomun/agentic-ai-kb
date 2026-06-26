---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "$τ^2$-Bench: Evaluating Conversational Agents in a Dual-Control Environment"
authors: Victor Barres, Honghua Dong, Soham Ray, Xujie Si et al.
url: https://arxiv.org/abs/2506.07982v1
date: 2025-06-09
citationCount: 275
influentialCitationCount: 43
velocity: 22.15
ingested: 2026-06-22
tags: [agent-reliability, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# $τ^2$-Bench: Evaluating Conversational Agents in a Dual-Control Environment

**arXiv [2506.07982v1](https://arxiv.org/abs/2506.07982v1)** · 2025-06-09 · **275 citations** (43 influential · 22.15/mo) · Victor Barres, Honghua Dong, Soham Ray, Xujie Si et al.

## Abstract
Existing benchmarks for conversational AI agents simulate single-control environments, where only the AI agent can use tools to interact with the world, while the user remains a passive information provider. This differs from real-world scenarios like technical support, where users need to actively participate in modifying the state of the (shared) world. In order to address this gap, we introduce $τ^2$-bench, with four key contributions: 1) A novel Telecom dual-control domain modeled as a Dec-POMDP, where both agent and user make use of tools to act in a shared, dynamic environment that tests both agent coordination and communication, 2) A compositional task generator that programmatically creates diverse, verifiable tasks from atomic components, ensuring domain coverage and controlled complexity, 3) A reliable user simulator tightly coupled with the environment, whose behavior is constrained by tools and observable states, improving simulation fidelity, 4) Fine-grained analysis of agent performance through multiple ablations including separating errors arising from reasoning vs communication/coordination. In particular, our experiments show significant performance drops when agents shift from no-user to dual-control, highlighting the challenges of guiding users. Overall, $τ^2$-bench provides a controlled testbed for agents that must both reason effectively and guide user actions.

## From the paper (full-text excerpts)
**Introduction.** Introduction Existing benchmarks for conversational AI agents are designed to test their abilities to communicate effectively with a user and perform the right sequence of actions to solve tasks [26, 14, 23, 19]. These benchmarks are inherently single-control environments, where the AI agent is able to interact with the world but the (simulated) user is limited to providing information about preferences and goals. In τ -bench [26] for example, the retail and airline domains test the agent’s ability to solve constraint satisfaction tasks, where constraints stem from a combination of a domain policy that the agent must follow and the user’s cognitive state including beliefs, goals and preferences. In such settings, the user’s understanding of the agent’s environment (including the set of actions the agent can take) is provided through carefully crafted natural language instructions that help ensure a single, solvable path for the constraint satisfaction problem. While this enables easier task * Equal contribution. † 1 Work done during internship. Code and data are available at: https…

**Method / approach.** method ensures provable correctness of tasks, provides complete domain coverage, allows for explicit control over task complexity (e.g., by number of solution steps or issue type), and removes the manual effort and potential brittleness associated with hand-crafted task suites. 2 Reliable user simulator. We enhance the reliability of the user simulation by tightly coupling the user simulator to the environment. User behavior is constrained by the available tools and the observable state of the environment, leading to more predictable and consistent interactions. This approach significantly alleviates the need for complex natural language prompting to guide the user simulator and results in substantially higher reliability (e.g., the telecom domain’s user simulator shows a 16% error rate with 6% critical errors, compared to 40% error rate with 12% critical errors in the retail domain from τ -bench). Fine-grained diagnosis of agent failures. τ 2 -bench enables a decomposed diagnosis o…

**Results.** experiments show significant performance drops when agents shift from no-user to dual-control, highlighting the challenges of guiding users. Overall, τ 2 -bench provides a controlled testbed for agents that must both reason effectively and guide user actions.1 1 Introduction Existing benchmarks for conversational AI agents are designed to test their abilities to communicate effectively with a user and perform the right sequence of actions to solve tasks [26, 14, 23, 19]. These benchmarks are inherently single-control environments, where the AI agent is able to interact with the world but the (simulated) user is limited to providing information about preferences and goals. In τ -bench [26] for example, the retail and airline domains test the agent’s ability to solve constraint satisfaction tasks, where constraints stem from a combination of a domain policy that the agent must follow and the user’s cognitive state including beliefs, go…

**Conclusion.** Conclusion We present τ 2 -bench that generalizes τ -bench by introducing the dual-control setting and found a substantial performance drop in LLMs due to coordination and communication requirements, highlighting these as critical bottlenecks over pure reasoning capabilities for solving user requests. Works remains to be done to improve the user simulator. Although we have shown that augmenting users with curated tools can help avoid critical errors, we have not yet investigated how this method could be applied to the existing airline and retail domains. Doing so would pave the way towards a more generic solution to ensuring high quality user simulator. Extending domain coverage for the benchmark still heavily relies on human experts. For…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2506.07982v1.md` · `raw/arxiv/2506.07982v1.fulltext.md`
