---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Assistance or Disruption? Exploring and Evaluating the Design and Trade-offs of Proactive AI Programming Support"
authors: Kevin Pu, Daniel Lazaro, Ian Arawjo, Haijun Xia et al.
url: https://arxiv.org/abs/2502.18658v4
date: 2025-02-25
citationCount: 63
influentialCitationCount: 4
velocity: 3.98
ingested: 2026-06-22
tags: [coding-agents, agentic-ai, arxiv, 2025, cited]
---

# Assistance or Disruption? Exploring and Evaluating the Design and Trade-offs of Proactive AI Programming Support

**arXiv [2502.18658v4](https://arxiv.org/abs/2502.18658v4)** · 2025-02-25 · **63 citations** (4 influential · 3.98/mo) · Kevin Pu, Daniel Lazaro, Ian Arawjo, Haijun Xia et al.

## Abstract
AI programming tools enable powerful code generation, and recent prototypes attempt to reduce user effort with proactive AI agents, but their impact on programming workflows remains unexplored. We introduce and evaluate Codellaborator, a design probe LLM agent that initiates programming assistance based on editor activities and task context. We explored three interface variants to assess trade-offs between increasingly salient AI support: prompt-only, proactive agent, and proactive agent with presence and context (Codellaborator). In a within-subject study (N=18), we find that proactive agents increase efficiency compared to prompt-only paradigm, but also incur workflow disruptions. However, presence indicators and interaction context support alleviated disruptions and improved users' awareness of AI processes. We underscore trade-offs of Codellaborator on user control, ownership, and code understanding, emphasizing the need to adapt proactivity to programming processes. Our research contributes to the design exploration and evaluation of proactive AI systems, presenting design implications on AI-integrated programming workflow.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 AI Programming Tools 2.2 Proactive Assistance and Interruption 2.3 Help-Seeking and Collaboration in Programming 2.3.1 Help-Seeking in Programming 2.3.2 Pair Programming 3 Design Goals 4 The Codellaborator Probe 4.1 Timely Proactive Programming Assistance 4.2 AI Agent’s Visual Representation in the Code Editor 4.3 Different Scopes of Interaction 4.4 Probe System Implementation 5 Evaluation 5.1 Participants 5.2 Study Design 5.3 Tasks 5.4 Procedure 5.5 Data Analysis 6 Results 6.1 Codellaborator Reduces Expression Effort and Alleviates Disruptions 6.2 Measuring Programming Sub-Task Boundary Is Effective to Time Proactive AI Assistance 6.3 Users Adapted to AI Proactivity and Established New Collaboration Patterns 6.4 Users Desired Varying Proactivity at Different Programming Processes 6.5 Codellaborator and CodeGhost Feel More Like Programming with a Partner than a Tool 6.6 Presence and Local Scope of Interaction Increase User Awareness on AI Action and Process 6.7 Over-Reliance on Proa…

**Method / approach.** approaches involve advancing on the timing of auto-completion feature to proactively make intelligent file changes with an AI caret in the code editor (cur, 2024 ) , representing the AI’s presence in the editor with an automated AI cursor (gen, 2024 ) , or grounding interactions context in different scopes, such as conversational dialogue (cop, 2023 ; Ross et al., 2023 ; Rep, 2024 ) , specific code lines (Jiang et al., 2022 ; git, 2023 ) , or an agent-managed workspace to tackle software engineering tasks autonomously (dev, 2024 ; Yang et al., 2024 ; Wang et al., 2024 ) . However, the effects of these new designs of system-driven programming assistance on the human workflows, compared to the existing user-initiated paradigm, remain to be explored. Visions of more “ proactive 1 1 1 In this paper, we refer to system-initiated assistance in the programming environment as “proactive” programming support. ” AI programmers additionally raise questions about the potential for harm. Researcher…

**Results.** experiment using three versions of Codellaborator with 18 participants. In the PromptOnly condition, the ablated system only responds to user prompts and in-line code comments, similar to ChatGPT (cha, 2023 ) and Github Copilot (git, 2023 ) with low to no proactive features. In the CodeGhost condition, the system proactively initiates interactions and assistance, but the interactions are constrained in the global context of chat messages and direct code changes, with no visual representation of the agent. In the Codellaborator condition, all of the agent’s visual representation, scopes of interaction , and proactive timing features are utilized. Our study showed that, through the heuristic-based timing to provide contextualized assistance at task boundaries, the CodeGhost condition reduced the time users took to comprehend system responses compared to the PromptOnly condition. But it also caused workflow disruptions and diminished u…

**Conclusion.** Conclusion A Codellaborator LLM Prompt A.1 System Prompt A.2 Action Prompt B Task Descriptions B.1 Task 1: Scheduling API B.1.1 Subtasks B.2 Task 2: Word Guessing Game B.2.1 Subtasks B.3 Task 3: Budget Tracker B.3.1 Subtasks \setlistdepth 9 Assistance or Disruption? Exploring and Evaluating the Design and Trade-offs of Proactive AI Programming Support Kevin Pu jpu@dgp.toronto.edu University of Toronto Canada , Daniel Lazaro d.lazaro@mail.utoronto.ca University of Toronto Canada , Ian Arawjo ian.arawjo@umontreal.ca Université de Montréal Canada , Haijun Xia haijunxia@ucsd.edu University of California San Diego USA , Ziang Xiao ziang.xiao@jh…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2502.18658v4.md` · `raw/arxiv/2502.18658v4.fulltext.md`
