---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Joint Knowledge Base Completion and Question Answering by Combining Large Language Models and Small Language Models"
authors: Yinan Liu et al.
url: https://arxiv.org/abs/2604.05875v1
date: 2026-04-07
score: 7
primary: cs.AI
tags: [arxiv, auto-ingested, small-language-models, llm-as-judge, post-training, reasoning-models, coding-agents]
---

# Joint Knowledge Base Completion and Question Answering by Combining Large Language Models and Small Language Models

**arXiv:** [2604.05875v1](https://arxiv.org/abs/2604.05875v1) · 2026-04-07 · cs.AI
**Authors:** Yinan Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Knowledge Bases (KBs) play a key role in various applications. As two representative KB-related tasks, knowledge base completion (KBC) and knowledge base question answering (KBQA) are closely related and inherently complementary with each other. Thus, it will be beneficial to solve the task of joint KBC and KBQA to make them reinforce each other. However, existing studies usually rely on the small language model (SLM) to enhance them jointly, and the large language model (LLM)'s strong reasoning ability is ignored. In this paper, by combining the strengths of the LLM with the SLM, we propose a novel framework JCQL, which can make these two tasks enhance each other in an iterative manner. To make KBC enhance KBQA, we augment the LLM agent-based KBQA model's reasoning paths by incorporating an SLM-trained KBC model as an action of the agent, alleviating the LLM's hallucination and high computational costs issue in KBQA. To make KBQA enhance KBC, we incrementally fine-tune the KBC model by leveraging KBQA's reasoning paths as its supplementary training data, improving the ability of the SLM in KBC. Extensive experiments over two public benchmark data sets demonstrate that JCQL surpasses all baselines for both KBC and KBQA tasks.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[llm-as-judge]] · [[post-training]] · [[reasoning-models]] · [[coding-agents]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.05875v1)
