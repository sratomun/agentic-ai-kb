---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "WebShaper: Agentically Data Synthesizing via Information-Seeking Formalization"
authors: Zhengwei Tao, Jialong Wu, Wenbiao Yin, Junkai Zhang et al.
url: https://arxiv.org/abs/2507.15061v1
date: 2025-07-20
citationCount: 97
influentialCitationCount: 16
velocity: 8.76
ingested: 2026-06-22
tags: [agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# WebShaper: Agentically Data Synthesizing via Information-Seeking Formalization

**arXiv [2507.15061v1](https://arxiv.org/abs/2507.15061v1)** · 2025-07-20 · **97 citations** (16 influential · 8.76/mo) · Zhengwei Tao, Jialong Wu, Wenbiao Yin, Junkai Zhang et al.

## Abstract
The advent of Large Language Model (LLM)-powered agents has revolutionized artificial intelligence by enabling solutions to complex, open-ended tasks through web-based information-seeking (IS) capabilities. The scarcity of high-quality training data has limited the development of IS agents. Existing approaches typically adopt an information-driven paradigm that first collects web data and then generates questions based on the retrieval. However, this may lead to inconsistency between information structure and reasoning structure, question and answer. To mitigate, we propose a formalization-driven IS data synthesis framework WebShaper to construct a dataset. WebShaper systematically formalizes IS tasks through set theory. Central to the formalization is the concept of Knowledge Projections (KP), which enables precise control over reasoning structure by KP operation compositions. During synthesis, we begin by creating seed tasks, then use a multi-step expansion process. At each step, an agentic Expander expands the current formal question more complex with retrieval and validation tools based on our formalization. We train our model on the synthesized dataset. Experiment results demonstrate that WebShaper achieves state-of-the-art performance among open-sourced IS agents on GAIA and WebWalkerQA benchmarks.

## From the paper (full-text excerpts)
**Introduction.** Introduction The emergence of Large Language Model (LLM)-powered language agents has marked a paradigmshifting advance in artificial intelligence, enabling transformative solutions to previously intractable challenges across domains (Guo et al., 2024; Wang et al., 2024; AutoGPT, 2023; Wu et al., 2023; Ye et al., 2023). Information-seeking (IS) represents a core component of the cognitive autonomy of language agents. This capability not only underpins their adaptability in open-ended tasks but also powers a range of powerful commercial systems such as Deep Research of OpenAI (OpenAI, 2025), Gemini (Gemini, 2025), and Perplexity (Perplexity, 2025). Current agentic systems for unlocking this capability typically follow a well-established pipeline in agent development: (1) First, construct task-specific trajectories of question-answer pairs; (2) Employ supervised fine-tuning (SFT) to acquire foundational skills (Sun et al., 2025). (3) Generalize strategic decision-making through on-policy reinforcement learning (RL) (Jin et al., 2025). The entire development of the IS agent originates f…

**Method / approach.** methods retrieve and organize collected information in advance, then synthesize data according to the information structures. (b) Our method establishes the task formalization first, then collects information, and synthesizes QA data based on the formalization. Existing IS dataset synthesis methods typically involve freely pre-searching for information online and employing LLMs to generate questions from the collected content (Figure 2(a)). These approaches first organize the collected information into structured formats, then prompt the LLM with the structured data to produce natural language (NL) questions. Their core objective is to map information structures into reasoning structures within the resulting NL questions. Representative methods like WebDancer (Wu et al., 2025a) and TaskCraft (Shi et al., 2025a) generate linear information chains, while others construct graphs connected via web links (Wu et al., 2025b) or entity coreference networks (Li et al., 2025a). However, these i…

**Results.** Experiment results demonstrate that WebShaper achieves state-of-the-art performance among open-sourced IS agents on GAIA and WebWalkerQA benchmarks. GAIA 60 60.19 58.25 50 55.4 55.33 52.43 51.5 50.5 48.5 40.77 40 30 39.8 37.86 20.4 20 G PT -4 .1 * Se ar ch -o 1 G em in i2 .0 * R 1Se ar ch er 70 W eb Sh ap er -7 C 2B la ud eSo nn et * W eb Sa ilo G r em im i2 .5 pr W o* eb Sh ap er -3 2B W eb D an ce r Si m pl eD R W eb Th in ke r arXiv:2507.15061v1 [cs.CL] 20 Jul 2025 https://github.com/Alibaba-NLP/WebAgent https://huggingface.co/datasets/Alibaba-NLP/WebShaper https://modelscope.cn/datasets/iic/WebShaper Figure 1: Results on GAIA information-seeking subset among the cutting-edge Deep Research models or systems. ∗ denotes the results using our two browsing tools via function calling APIs. * denotes equal contribution. denotes the correspondence. {yinwenbiao.ywb, yongjiang.yj}@alibaba-inc.com 1 1 Introduction The…

**Conclusion.** Conclusion This work presents a paradigm-shifting framework for synthesizing training data WebShaper for information-seeking (IS) agents through formalization-driven design. By establishing a set theory-based mathematical formalization of IS tasks, we address critical limitations in existing information-driven approaches that suffer from structural inconsistencies, task controllability, diversity, and coverage. The composition of proposed Knowledge Projections enables precise engineering of reasoning structures and complexity. Our agentic Expander module further ensures systematic expansion of formalized tasks with a layer-wise expansion paradigm, combining autonomous knowledge retrieval and rigorous validation to minimize redundancy and p…

## Graph
- **Concepts:** [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[gaia-benchmark]]
- **Raw:** `raw/arxiv/2507.15061v1.md` · `raw/arxiv/2507.15061v1.fulltext.md`
