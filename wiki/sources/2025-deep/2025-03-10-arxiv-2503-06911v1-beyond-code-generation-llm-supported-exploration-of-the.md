---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Beyond Code Generation: LLM-supported Exploration of the Program Design Space"
authors: J. D. Zamfirescu-Pereira, Eunice Jun, Michael Terry, Qian Yang et al.
url: https://arxiv.org/abs/2503.06911v1
date: 2025-03-10
citationCount: 53
influentialCitationCount: 3
velocity: 3.44
ingested: 2026-06-22
tags: [coding-agents, arxiv, 2025, cited]
---

# Beyond Code Generation: LLM-supported Exploration of the Program Design Space

**arXiv [2503.06911v1](https://arxiv.org/abs/2503.06911v1)** · 2025-03-10 · **53 citations** (3 influential · 3.44/mo) · J. D. Zamfirescu-Pereira, Eunice Jun, Michael Terry, Qian Yang et al.

## Abstract
In this work, we explore explicit Large Language Model (LLM)-powered support for the iterative design of computer programs. Program design, like other design activity, is characterized by navigating a space of alternative problem formulations and associated solutions in an iterative fashion. LLMs are potentially powerful tools in helping this exploration; however, by default, code-generation LLMs deliver code that represents a particular point solution. This obscures the larger space of possible alternatives, many of which might be preferable to the LLM's default interpretation and its generated code. We contribute an IDE that supports program design through generating and showing new ways to frame problems alongside alternative solutions, tracking design decisions, and identifying implicit decisions made by either the programmer or the LLM. In a user study, we find that with our IDE, users combine and parallelize design phases to explore a broader design space -- but also struggle to keep up with LLM-originated changes to code and other information overload. These findings suggest a core challenge for future IDEs that support program design through higher-level instructions given to LLM-based agents: carefully managing attention and deciding what information agents should surface to program designers and when.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Program Design Processes; Sketching and Comparing Alternatives 2.2 AI Assistance for Programming and Design 2.3 Workflows Integrating LLMs in Complex Tasks 3 Designing Pail 3.1 Design Process 3.2 Formative Study 3.3 Design Goals 3.4 System Design 3.4.1 System Design Non-Goals 3.5 Pail Implementation 3.5.1 Speculative Assessment 3.5.2 Differential Updates to Code 3.5.3 Differential Updates to Design Artifacts 4 Pail Usage: An Example 5 User Study Procedure 5.1 Interview Protocol 5.2 Tasks 5.3 Participants 5.4 Analysis Evaluation 6 Findings 6.1 Use of Pail ’s Design Support 6.1.1 Abstracting Up Problem Exploration Reflection 6.1.2 A Working Sketch: First Contact Rapid Iteration Reflection 6.1.3 The Design Panel, Alternatives, and Rationales Reflection 6.2 Stumbles, Mismatches in Participants’ Design Processes 6.2.1 Re-considering Design Problems 6.2.2 Content Generation and Overwhelming Information 6.2.3 Application of Reflection and Design Agents 6.2.4 Att…

**Method / approach.** methodologies Artificial intelligence Figure 1 . Today, LLM-powered programming assistance resembles a repeating cycle of “prompt”-to-“code” (left) by re-running generation with every prompt change. Pail , our IDE (right), instead encourages developers to abstract up, pulling them towards a deeper understanding of the problem space through an exploration of alternative problem formulations and solutions. Throughout this exploration, Pail tracks design goals, changing requirements, and surfaces implicit decisions—but the breadth and depth of information Pail generates can be overwhelming. \Description 1. Introduction A common vision of future computer programming relies on Large Language Models (LLMs) to do it all: identify requirements, write code and tests, perform simulated QA testing, deploy, etc. We are making rapid progress towards this vision on many fronts (Hong et al . , 2023 ; Di Fede et al . , 2022 ; noa, 2024a ; Chen et al . , 2021 ; Si et al . , 2024 ) . Yet t…

**Results.** experiments or revert to the code used for them. Participants also reported feeling unsure about the code the LLMs generated, looking at it relatively rarely—the common iterative loop consisted of running the generated code and asking the LLM directly to fix any observed errors, rather than reviewing the code directly for errors. Conspicuously lacking was support for an understanding of the generated code, beyond the high-level overviews produced by the LLMs—overviews which lacked mention or explanation of critical decisions or assumptions made by the LLM. Even when these were provided, they were typically buried within paragraphs of overview, requiring a close read to find, and participants almost never read these explanations closely because of a low signal-to-noise ratio. Lastly, those participants who mediated a program generation exercise for someone else reported spending substantial time identifying what needs that user had, a…

**Conclusion.** Conclusion 10 Disclosure Beyond Code Generation: LLM-supported Exploration of the Program Design Space J.D. Zamfirescu-Pereira zamfi@berkeley.edu UC Berkeley Berkeley CA USA , Eunice Jun emjun@cs.ucla.edu UCLA Los Angeles CA USA , Michael Terry michaelterry@google.com Google DeepMind Cambridge MA USA , Qian Yang qianyang@cornell.edu Cornell University Ithaca NY USA and Björn Hartmann bjoern@eecs.berkeley.edu UC Berkeley Berkeley CA USA (2025) Abstract. In this work, we explore explicit Large Language Model (LLM)-powered support for the iterative design of computer programs. Program design, like other design activity, is characterized by navigating a space of a…

## Graph
- **Concepts:** [[coding-agents|Coding agents]]
- **Raw:** `raw/arxiv/2503.06911v1.md` · `raw/arxiv/2503.06911v1.fulltext.md`
