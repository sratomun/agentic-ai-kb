---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MiroThinker: Pushing the Performance Boundaries of Open-Source Research Agents via Model, Context, and Interactive Scaling"
authors: MiroMind Team, Song Bai, Lidong Bing, Carson Chen et al.
url: https://arxiv.org/abs/2511.11793v3
date: 2025-11-14
citationCount: 52
influentialCitationCount: 9
velocity: 7.19
ingested: 2026-06-22
tags: [science-agents, agentic-rl, tool-use, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# MiroThinker: Pushing the Performance Boundaries of Open-Source Research Agents via Model, Context, and Interactive Scaling

**arXiv [2511.11793v3](https://arxiv.org/abs/2511.11793v3)** · 2025-11-14 · **52 citations** (9 influential · 7.19/mo) · MiroMind Team, Song Bai, Lidong Bing, Carson Chen et al.

## Abstract
We present MiroThinker v1.0, an open-source research agent designed to advance tool-augmented reasoning and information-seeking capabilities. Unlike previous agents that only scale up model size or context length, MiroThinker explores interaction scaling at the model level, systematically training the model to handle deeper and more frequent agent-environment interactions as a third dimension of performance improvement. Unlike LLM test-time scaling, which operates in isolation and risks degradation with longer reasoning chains, interactive scaling leverages environment feedback and external information acquisition to correct errors and refine trajectories. Through reinforcement learning, the model achieves efficient interaction scaling: with a 256K context window, it can perform up to 600 tool calls per task, enabling sustained multi-turn reasoning and complex real-world research workflows. Across four representative benchmarks-GAIA, HLE, BrowseComp, and BrowseComp-ZH-the 72B variant achieves up to 81.9%, 37.7%, 47.1%, and 55.6% accuracy respectively, surpassing previous open-source agents and approaching commercial counterparts such as GPT-5-high. Our analysis reveals that MiroThinker benefits from interactive scaling consistently: research performance improves predictably as the model engages in deeper and more frequent agent-environment interactions, demonstrating that interaction depth exhibits scaling behaviors analogous to model size and context length. These findings establish interaction scaling as a third critical dimension for building next-generation open research agents, complementing model capacity and context windows.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works Agent Foundation Models Deep Research Models 3 Agentic Workflow 3.1 Formulation 3.2 Tool Interface Execution Environment File Management Information Retrieval 3.3 Context Management Recency-Based Context Retention Result Truncation 4 Data Construction 4.1 MultiDocQA Synthesis Document Corpus Construction Document Sampling and Graph Construction Document Consolidation Fact Extraction Constraint Obfuscation Question Generation 4.2 Agentic Trajectory Synthesis Agent Paradigms Tool Invocation Mechanisms Diverse Data Synthesis 4.3 Open-Source Data Collection 5 Training Pipeline 5.1 Agentic Supervised Fine-tuning Data Construction Training Objective 5.2 Agentic Preference Optimization Data Collection Training Objective 5.3 Agentic Reinforcement Learning Environment Setup Streaming Rollout Acceleration Reward Design Trajectory Curation Training Objective 6 Experiments 6.1 Experimental Setup Evaluation Benchmarks. Evaluation Protocol. 6.2 Ove…

**Method / approach.** method combining metadata extraction and topic modeling, enabling category-aware sampling in later stages. Document Sampling and Graph Construction We begin by sampling document nodes from our corpus while maintaining balanced representation across different categories. This category-balanced sampling ensures comprehensive coverage across diverse knowledge domains and prevents bias toward over-represented topics. For each sampled seed document, we construct a knowledge graph by following its internal hyperlinks. Specifically, we randomly select one internal link from each document and recursively repeat this process multiple times to build a connected subgraph of related documents. Document Consolidation After constructing the document graph, we convert each document into markdown format and perform link pruning. We remove all hyperlinks that point to documents outside our selected subgraph, ensuring that the consolidated article maintains coherent references only within t…

**Results.** Experiments 6.1 Experimental Setup Evaluation Benchmarks. Evaluation Protocol. 6.2 Overall Performance 6.3 Interactive Scaling 6.4 Limitations Tool-Use Quality under Interactive Scaling Overlong Chain-of-Thought Language Mixing Limited Sandbox Capability 7 Conclusions References License: arXiv.org perpetual non-exclusive license arXiv:2511.11793v3 [cs.CL] 21 Apr 2026 MiroThinker: Pushing the Performance Boundaries of Open-Source Research Agents via Model, Context, and Interactive Scaling MiroMind Team Abstract We present MiroThinker v1.0, an open-source research agent designed to advance tool-augmented reasoning and information-seeking capabilities. Unlike previous agents that only scale up model size or context length, MiroThinker explores interaction scaling at the model level—systematically training the model to handle deeper and more frequent agent–environment interactions as a third di…

**Conclusion.** Conclusions References License: arXiv.org perpetual non-exclusive license arXiv:2511.11793v3 [cs.CL] 21 Apr 2026 MiroThinker: Pushing the Performance Boundaries of Open-Source Research Agents via Model, Context, and Interactive Scaling MiroMind Team Abstract We present MiroThinker v1.0, an open-source research agent designed to advance tool-augmented reasoning and information-seeking capabilities. Unlike previous agents that only scale up model size or context length, MiroThinker explores interaction scaling at the model level—systematically training the model to handle deeper and more frequent agent–environment interactions as a third dimension of performance improvement. Unlike LLM test-time scaling, which operates in isol…

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[gaia-benchmark]] · [[gpt-5]]
- **Raw:** `raw/arxiv/2511.11793v3.md` · `raw/arxiv/2511.11793v3.fulltext.md`
