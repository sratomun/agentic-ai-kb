---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Command A: An Enterprise-Ready Large Language Model"
authors: Team Cohere, :, Aakanksha, Arash Ahmadian et al.
url: https://arxiv.org/abs/2504.00698v2
date: 2025-04-01
citationCount: 55
influentialCitationCount: 5
velocity: 3.75
ingested: 2026-06-22
tags: [agentic-rag, tool-use, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Command A: An Enterprise-Ready Large Language Model

**arXiv [2504.00698v2](https://arxiv.org/abs/2504.00698v2)** · 2025-04-01 · **55 citations** (5 influential · 3.75/mo) · Team Cohere, :, Aakanksha, Arash Ahmadian et al.

## Abstract
In this report we describe the development of Command A, a powerful large language model purpose-built to excel at real-world enterprise use cases. Command A is an agent-optimised and multilingual-capable model, with support for 23 languages of global business, and a novel hybrid architecture balancing efficiency with top of the range performance. It offers best-in-class Retrieval Augmented Generation (RAG) capabilities with grounding and tool use to automate sophisticated business processes. These abilities are achieved through a decentralised training approach, including self-refinement algorithms and model merging techniques. We also include results for Command R7B which shares capability and architectural similarities to Command A. Weights for both models have been released for research purposes. This technical report details our original training pipeline and presents an extensive evaluation of our models across a suite of enterprise-relevant tasks and public benchmarks, demonstrating excellent performance and efficiency.

## From the paper (full-text excerpts)
**Introduction.** Introduction Large Language Models (LLMs) are Artificial Intelligence (AI) models designed to understand and generate human-like text conditioned on the input they receive. Recent advancements have led to remarkable breakthroughs in their ability to comprehend and produce human language with unparalleled accuracy and fluency. This progress has been instrumental in their widespread adoption across various real-world and enterprise environments, where they significantly boost operational efficiency and deepen understanding. This technical report describes the development of Command A and Command R7B, two LLMs designed to excel in real-world enterprise settings. Both the 111B parameter Command A and Command R7B perform best-in-class across a suite of established benchmarks for their respective model sizes. We also highlight key innovations and technical contributions including data and architectural optimisations, self-refinement algorithms, and a model merging-based approach optimised to bring out expert-level performance across capabilities within a single set of model weights, provi…

**Method / approach.** methods, offline preference, and online RL algorithms. Six expert models are created at each expert stage: Code, Safety, RAG, Math, Multilingual, and a General Long-Context expert. This approach allows us to adapt each expert’s training procedure, tailoring it to the specific capability or domain of interest. This allows fine-grained hyperparameter tuning, specialised data mixture optimisation, local optimisation (e.g., seed merging), and the capability-specific selection of the most appropriate algorithms. This becomes even more crucial during the RL stage, as different domains demand distinct RL techniques — for example, verifiable rewards for Math and Code, or preference pairs for Safety and Multilingual. Our late-merging procedure allows us to re-balance Soup model performance a posteriori without requiring additional training (§3.4). From an organisational perspective, merging allows contributors to collaborate closely in parallel, fostering a unique model development synergy. Ov…

**Results.** experiment with reward-based sample refinement approaches to obtain both SFT and preference pairs using the synthetically-generated prompts. Similar to Dubey et al. (2024), we use internal reward models trained on our most recent Command A checkpoints in conjunction with a collection of both humanwritten completions and completions generated from different checkpoints under different conditions (e.g., varying temperature values) during post-training This implies that the resulting dataset does not contain purely synthetic completions, and human-written completions are retained for inputs where the models fail to generate high-quality completions. We approach this in an iterative fashion, where we use the most recent checkpoints at a given point in time to generate completions, score those completions using our reward model, create preference pairs and SFT samples using the scores, re-train our models, and repeat. 3.3.1.3 Preambles A s…

## Graph
- **Concepts:** [[agentic-rag|Agentic RAG]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.00698v2.md` · `raw/arxiv/2504.00698v2.fulltext.md`
