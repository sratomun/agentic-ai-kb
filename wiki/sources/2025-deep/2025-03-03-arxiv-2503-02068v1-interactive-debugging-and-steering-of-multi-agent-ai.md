---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Interactive Debugging and Steering of Multi-Agent AI Systems"
authors: Will Epperson, Gagan Bansal, Victor Dibia, Adam Fourney et al.
url: https://arxiv.org/abs/2503.02068v1
date: 2025-03-03
citationCount: 69
influentialCitationCount: 6
velocity: 4.41
ingested: 2026-06-22
tags: [computer-use-agents, multi-agent-systems, agentic-ai, arxiv, 2025, cited]
---

# Interactive Debugging and Steering of Multi-Agent AI Systems

**arXiv [2503.02068v1](https://arxiv.org/abs/2503.02068v1)** · 2025-03-03 · **69 citations** (6 influential · 4.41/mo) · Will Epperson, Gagan Bansal, Victor Dibia, Adam Fourney et al.

## Abstract
Fully autonomous teams of LLM-powered AI agents are emerging that collaborate to perform complex tasks for users. What challenges do developers face when trying to build and debug these AI agent teams? In formative interviews with five AI agent developers, we identify core challenges: difficulty reviewing long agent conversations to localize errors, lack of support in current tools for interactive debugging, and the need for tool support to iterate on agent configuration. Based on these needs, we developed an interactive multi-agent debugging tool, AGDebugger, with a UI for browsing and sending messages, the ability to edit and reset prior agent messages, and an overview visualization for navigating complex message histories. In a two-part user study with 14 participants, we identify common user strategies for steering agents and highlight the importance of interactive message resets for debugging. Our studies deepen understanding of interfaces for debugging increasingly important agentic workflows.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Multi-Agent AI Systems 2.2 LLM and Agent Debugging 3 Background: Agent Framework and Tasks 3.1 Agent Implementation Framework 3.2 GAIA Benchmark Tasks 3.3 Agent Team for GAIA Tasks 4 Formative Interviews on Agent Debugging 4.1 Understanding Long Agent Conversations is Cumbersome 4.2 Lack of Support for Interactive Debugging 4.3 Iterating on Agent Configuration 4.4 Design Goals 5 AGDebugger : Interactive Agent Debugging 5.1 Message Sending and History 5.2 Message Resetting and Edits 5.2.1 Technical details: checkpoints and sessions 5.3 Conversation Overview Visualization 5.4 Agent Configuration 6 User Study 6.1 Study Design 6.2 Part 1 Findings: Error Identification 6.3 Part 2 Findings: AGDebugger Facilitates Interactive Steering and Debugging 6.4 Three User Approaches to Steer Agents 6.5 User Study Limitations 7 Discussion 7.1 Open Challenges for AI Agent Steering 7.2 Future Directions for Multi-Agent Debugging 8 Conclusion A Formative interview details B User study par…

**Method / approach.** methodologies Multi-agent systems Figure 1. Debugging multi-agent AI systems involves reasoning over long multi-turn conversations where specialized agents use tools like web browsing and writing code with LLMs. AGDebugger allows users to interactively debug and steer multi-agent teams by resetting the agents to earlier points in the workflow then editing messages to interactively test hypotheses about their behavior. \Description This figure shows an agent conversation with represented as boxes on the lefthand side. Several of these boxes are connected to screenshots of the tool used in that box such as a web browsing page or code writing. One of the messages is annotated with an annotation that reads What would have happened with a different plan at message 5?. This leads to a second conversation that is a fork of the first where the messages above the fork are greyed out and the new messages are different. At the bottom, an annotation shows that the original agent conver…

**Results.** experiment with fixes for errors in agent workflows. We identify common patterns of steering across users around adding instructions to agent messages, simplifying messages, and modifying the agents’ plan. 2. Related Work 2.1. Multi-Agent AI Systems In recent years, general purpose Large Language Models (LLMs) leveraging in-context learning (e.g., few-shot prompting), have been applied to various domains that previously required training specialized models (Brown et al . , 2020 ) . When combined with the ability to use tools and store state, these models can function as agents that interact with the world to accomplish more complex tasks. AI agents have been developed for tasks ranging from browsing the web (Zhou et al . , 2024 ; He et al . , 2024 ) to advanced coding tasks that involve looking up documentation and combining code authoring with execution (Jimenez et al . , 2024 ; Wang et al . , 2024 ) . For more intricat…

**Conclusion.** Conclusion A Formative interview details B User study part 2 questions \setcctype by Interactive Debugging and Steering of Multi-Agent AI Systems Will Epperson willepp@cmu.edu 0000-0002-2745-4315 Human-Computer Interaction Institute Carnegie Mellon University Pittsburgh PA USA , Gagan Bansal gaganbansal@microsoft.com 0000-0002-7741-3861 Microsoft Research Redmond WA USA , Victor Dibia victordibia@microsoft.com 0000-0002-1839-5632 Microsoft Research Redmond WA USA , Adam Fourney adam.fourney@microsoft.com 0000-0002-4986-7794 Microsoft Research Redmond WA USA , Jack Gerrits jagerrit@microsoft.com 0009-0003-1966-2434 Microsoft Research Redmond WA USA ,…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2503.02068v1.md` · `raw/arxiv/2503.02068v1.fulltext.md`
