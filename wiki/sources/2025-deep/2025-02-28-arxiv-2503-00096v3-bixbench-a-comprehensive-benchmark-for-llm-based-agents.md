---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "BixBench: a Comprehensive Benchmark for LLM-based Agents in Computational Biology"
authors: Ludovico Mitchener, Jon M Laurent, Alex Andonian, Benjamin Tenmann et al.
url: https://arxiv.org/abs/2503.00096v3
date: 2025-02-28
citationCount: 73
influentialCitationCount: 6
velocity: 4.64
ingested: 2026-06-22
tags: [science-agents, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# BixBench: a Comprehensive Benchmark for LLM-based Agents in Computational Biology

**arXiv [2503.00096v3](https://arxiv.org/abs/2503.00096v3)** · 2025-02-28 · **73 citations** (6 influential · 4.64/mo) · Ludovico Mitchener, Jon M Laurent, Alex Andonian, Benjamin Tenmann et al.

## Abstract
Large Language Models (LLMs) and LLM-based agents show great promise in accelerating scientific research. Existing benchmarks for measuring this potential and guiding future development continue to evolve from pure recall and rote knowledge tasks, towards more practical work such as literature review and experimental planning. Bioinformatics is a domain where fully autonomous AI-driven discovery may be near, but no extensive benchmarks for measuring progress have been introduced to date. We therefore present the Bioinformatics Benchmark (BixBench), a dataset comprising over 50 real-world scenarios of practical biological data analysis with nearly 300 associated open-answer questions designed to measure the ability of LLM-based agents to explore biological datasets, perform long, multi-step analytical trajectories, and interpret the nuanced results of those analyses. We evaluate the performance of two frontier LLMs (GPT-4o and Claude 3.5 Sonnet) using a custom agent framework we open source. We find that even the latest frontier models only achieve 17% accuracy in the open-answer regime, and no better than random in a multiple-choice setting. By exposing the current limitations of frontier models, we hope BixBench can spur the development of agents capable of conducting rigorous bioinformatic analysis and accelerate scientific discovery.

## From the paper (full-text excerpts)
**Introduction.** Introduction Accelerating scientific discovery across domains is a core aspiration for modern AI models and agents, driven by the ability of these systems to synthesize information and identify novel connections across disparate fields (Skarlinski et al., 2024). While significant progress has been made in developing systems for automating certain aspects of the scientific research process (Lu et al., 2024; Gao et al., 2024; Swanson et al., 2024; Schmidgall et al., 2025; Narayanan et al., 2024), the ultimate realization of fully automated scientific systems remains elusive. Large Language Models (LLMs) and LLM-based agents show great promise in accelerating scientific research. Existing benchmarks for measuring this potential and guiding future development continue to evolve from pure recall and rote knowledge tasks, towards more practical work such as literature review and experimental planning. Bioinformatics is a domain where fully autonomous AI-driven discovery may be near, but no extensive benchmarks for measuring progress have been introduced to date. We therefore present the…

**Method / approach.** method. However, we are also able to perform multiple-choice evaluations with options to determine how that may influence performance in answering the questions. 3.2.2 • list workdir: Enables the model to inspect its own workspace directory recursively to ascertain the structure and format of the dataset. • submit answer: Used by the model to finalize and submit an open-answer. At each timestep, the model must decide which tool to invoke. The agent then receives observations from the tool’s execution. Each code modification triggers a full rerun of the notebook, allowing the model to view results in tabular or plot formats as well as debug tracebacks. Prompt engineering was explored extensively as a means to improve performance. An example of the final prompt used to initiate an agent trajectory is shared in the Appendix A. AGENT I NFRASTRUCTURE We implemented our agent framework using Aviary, an extensible gymnasium for language agents (Narayanan et al., 2024). Aviary was selected…

**Results.** experimental planning. Bioinformatics is a domain where fully autonomous AI-driven discovery may be near, but no extensive benchmarks for measuring progress have been introduced to date. We therefore present the Bioinformatics Benchmark (BixBench), a dataset comprising over 60 realworld scenarios of practical biological data analysis with over 200 associated open-answer questions designed to measure the ability of LLMbased agents to explore biological datasets, perform long, multi-step analytical trajectories, and interpret the nuanced results of those analyses. We evaluate the performance of two frontier LLMs (GPT-4o and Claude 3.5 Sonnet) using a custom agent framework we open source. We find that even the latest frontier models achieve only 21% accuracy in the open-answer regime, and marginally better than random in a multiplechoice setting. By exposing the current limitations of frontier models, we hope BixBench can spur the develop…

**Conclusion.** Discussion Biological data analysis and associated domains offer an opportunity to build the first agents for scientific discovery, and thus assessing the state of progress is critical. We’ve introduced here BixBench, a benchmark and evaluation framework for measuring agent performance on real-world bioinformatics tasks. BixBench presents 61 real-world analytical scenarios, along with a set of 205 associated questions, supporting both open-answer or multiple-choice evaluation regimes. 5.1.3 Reasoning models, introduced recently in (OpenAI et al., 2024; DeepSeek-AI et al., 2025) and others have rapidly topped many benchmarks, including MLE-bench. It is still early to incorporate them into environments, with few details or results on tool…

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[claude]] · [[gpt-5]]
- **Raw:** `raw/arxiv/2503.00096v3.md` · `raw/arxiv/2503.00096v3.fulltext.md`
