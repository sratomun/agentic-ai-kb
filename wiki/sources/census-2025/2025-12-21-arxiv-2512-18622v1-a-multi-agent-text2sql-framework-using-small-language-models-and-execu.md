---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "A Multi-agent Text2SQL Framework using Small Language Models and Execution Feedback"
authors: Thanh Dat Hoang et al.
url: https://arxiv.org/abs/2512.18622v1
date: 2025-12-21
score: 12
primary: cs.DB
tags: [arxiv, auto-ingested, small-language-models, llm-as-judge, post-training, multi-agent-systems, text-to-sql]
---

# A Multi-agent Text2SQL Framework using Small Language Models and Execution Feedback

**arXiv:** [2512.18622v1](https://arxiv.org/abs/2512.18622v1) · 2025-12-21 · cs.DB
**Authors:** Thanh Dat Hoang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Text2SQL, the task of generating SQL queries from natural language text, is a critical challenge in data engineering. Recently, Large Language Models (LLMs) have demonstrated superior performance for this task due to their advanced comprehension and generation capabilities. However, privacy and cost considerations prevent companies from using Text2SQL solutions based on external LLMs offered as a service. Rather, small LLMs (SLMs) that are openly available and can hosted in-house are adopted. These SLMs, in turn, lack the generalization capabilities of larger LLMs, which impairs their effectiveness for complex tasks such as Text2SQL. To address these limitations, we propose MATS, a novel Text2SQL framework designed specifically for SLMs. MATS uses a multi-agent mechanism that assigns specialized roles to auxiliary agents, reducing individual workloads and fostering interaction. A training scheme based on reinforcement learning aligns these agents using feedback obtained during execution, thereby maintaining competitive performance despite a limited LLM size. Evaluation results using on benchmark datasets show that MATS, deployed on a single- GPU server, yields accuracy that are on-par with large-scale LLMs when using significantly fewer parameters. Our source code and data are available at https://github.com/thanhdath/mats-sql.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[llm-as-judge]] · [[post-training]] · [[multi-agent-systems]] · [[text-to-sql]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2512.18622v1)
