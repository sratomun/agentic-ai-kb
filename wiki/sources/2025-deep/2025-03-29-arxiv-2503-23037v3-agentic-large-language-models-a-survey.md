---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Agentic Large Language Models, a survey"
authors: Aske Plaat, Max van Duijn, Niki van Stein, Mike Preuss et al.
url: https://arxiv.org/abs/2503.23037v3
date: 2025-03-29
citationCount: 128
influentialCitationCount: 3
velocity: 8.66
ingested: 2026-06-22
tags: [clinical-agents, embodied-agents, finance-agents, agent-security, tool-use, arxiv, 2025, cited]
---

# Agentic Large Language Models, a survey

**arXiv [2503.23037v3](https://arxiv.org/abs/2503.23037v3)** · 2025-03-29 · **128 citations** (3 influential · 8.66/mo) · Aske Plaat, Max van Duijn, Niki van Stein, Mike Preuss et al.

## Abstract
Background: There is great interest in agentic LLMs, large language models that act as agents. Objectives: We review the growing body of work in this area and provide a research agenda. Methods: Agentic LLMs are LLMs that (1) reason, (2) act, and (3) interact. We organize the literature according to these three categories. Results: The research in the first category focuses on reasoning, reflection, and retrieval, aiming to improve decision making; the second category focuses on action models, robots, and tools, aiming for agents that act as useful assistants; the third category focuses on multi-agent systems, aiming for collaborative task solving and simulating interaction to study emergent social behavior. We find that works mutually benefit from results in other categories: retrieval enables tool use, reflection improves multi-agent collaboration, and reasoning benefits all categories. Conclusions: We discuss applications of agentic LLMs and provide an agenda for further research. Important applications are in medical diagnosis, logistics and financial market analysis. Meanwhile, self-reflective agents playing roles and interacting with one another augment the process of scientific research itself. Further, agentic LLMs provide a solution for the problem of LLMs running out of training data: inference-time behavior generates new training states, such that LLMs can keep learning without needing ever larger datasets. We note that there is risk associated with LLM assistants taking action in the real world-safety, liability and security are open problems-while agentic LLMs are also likely to benefit society.

## From the paper (full-text excerpts)
**Introduction.** Introduction 1.1 Agentic LLMs: Reasoning–Acting–Interacting 1.2 Literature Selection 1.3 LLM Training Pipeline Data, Benchmarks, and Performance Models Training Pipeline 1.4 The Need for Agentic LLMs 1.5 Taxonomy Reasoning (Table 1 ) Acting (Table 2 ) Interacting (Table 3 ) Taxonomy 2 Reasoning 2.1 Multi Step Reasoning 2.1.1 Chain of Thought Step-by-Step 2.1.2 Interpreter and Debugger 2.1.3 Search Tree 2.2 Self Reflection 2.2.1 Prompt-Improvement 2.2.2 Using LLMs for Self Reflection Transformers as Memory Memory, Experience, Personality Implicit Reasoning 2.3 Retrieval Augmentation 2.4 Discussion 2.4.1 In Depth: Chain of Thought and Self Reflection Chain of Thought Self Reflection 2.4.2 Thinking, Fast and Slow 2.4.3 Causal and Common Sense Reasoning 2.4.4 Artificial General Intelligence 2.4.5 Interpretability 2.4.6 Use Case: Benchmarks 3 Acting 3.1 Action Models 3.1.1 World Models 3.1.2 Vision-Language-Action Models 3.2 Robots and Tools 3.2.1 Robot Planning 3.2.2 Act…

**Method / approach.** Methods: Agentic LLMs are LLMs that (1) reason, (2) act, and (3) interact. We organize the literature according to these three categories. Results: The research in the first category focuses on reasoning, reflection, and retrieval, aiming to improve decision making; the second category focuses on action models, robots, and tools, aiming for agents that act as useful assistants; the third category focuses on multi-agent systems, aiming for collaborative task solving and simulating interaction to study emergent social behavior. We find that works mutually benefit from results in other categories: retrieval enables tool use, reflection improves multi-agent collaboration, and reasoning benefits all categories. Conclusions: We discuss applications of agentic LLMs and provide an agenda for further research. Important applications are in medical diagnosis, logistics and financial market analysis. Meanwhile, self-reflective agents playing roles and interacting with one another augment…

**Results.** experiments. The outcome of assistant actions (category 2) and of these social experiments (category 3) can be used for data augmentation (category 1), to finetune LLMs (which can improve the accuracy of reasoning LLMs, etc.). This virtuous circle is depicted in Figure 1 , and attracts interest from LLM researchers to agentic LLM methods ( sutskever2024 ; guo2025deepseek ; team2025kimi ; lambert2024tulu ) . The categories also correspond to fields in artificial intelligence that have a long research tradition across symbolic AI, robotics/autonomous systems, and connectionism/multi-agent modeling, respectively. Agentic LLMs are thus both a recent development and build on decades of research. This is reflected in our discussion below. 1.2. Literature Selection The field of agentic LLM is rich and active. This survey can only cover the current status of the field. We hope to provide clarity about the main approaches, to ease the en…

**Conclusion.** Conclusion 6 Reproducibility Checklist for JAIR \JAIRAE Kai-Wei Chang \JAIRTrack Agentic Large Language Models, a survey Aske Plaat 0000-0001-7202-3322 aske.plaat@gmail.com Leiden University Leiden Netherlands , Max van Duijn Leiden University Leiden Netherlands , Niki van Stein Leiden University Leiden Netherlands , Mike Preuss Leiden University Leiden Netherlands , Peter van der Putten Leiden University AI Lab, Pegasystems Leiden Netherlands and Kees Joost Batenburg Leiden University Leiden Netherlands (6 October 2025) Abstract. Background: There is great interest in agentic LLMs , large language models that act as agents. Objectives: We review the growing b…

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[embodied-agents|Embodied agents]] · [[finance-agents|Finance agents]] · [[agent-security|Agent security]] · [[tool-use|Tool use]]
- **Raw:** `raw/arxiv/2503.23037v3.md` · `raw/arxiv/2503.23037v3.fulltext.md`
