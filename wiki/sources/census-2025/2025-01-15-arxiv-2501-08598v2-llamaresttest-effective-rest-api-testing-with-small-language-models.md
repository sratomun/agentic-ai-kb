---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "LlamaRestTest: Effective REST API Testing with Small Language Models"
authors: Myeongsoo Kim et al.
url: https://arxiv.org/abs/2501.08598v2
date: 2025-01-15
score: 1
primary: cs.SE
tags: [arxiv, auto-ingested, small-language-models, llm-as-judge, post-training]
---

# LlamaRestTest: Effective REST API Testing with Small Language Models

**arXiv:** [2501.08598v2](https://arxiv.org/abs/2501.08598v2) · 2025-01-15 · cs.SE
**Authors:** Myeongsoo Kim et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Modern web services rely heavily on REST APIs, typically documented using the OpenAPI specification. The widespread adoption of this standard has resulted in the development of many black-box testing tools that generate tests based on OpenAPI specifications. Although Large Language Models (LLMs) have shown promising test-generation abilities, their application to REST API testing remains mostly unexplored. We present LlamaRestTest, a novel approach that employs two custom LLMs-created by fine-tuning and quantizing the Llama3-8B model using mined datasets of REST API example values and inter-parameter dependencies-to generate realistic test inputs and uncover inter-parameter dependencies during the testing process by analyzing server responses. We evaluated LlamaRestTest on 12 real-world services (including popular services such as Spotify), comparing it against RESTGPT, a GPT-powered specification-enhancement tool, as well as several state-of-the-art REST API testing tools, including RESTler, MoRest, EvoMaster, and ARAT-RL. Our results demonstrate that fine-tuning enables smaller models to outperform much larger models in detecting actionable parameter-dependency rules and generating valid inputs for REST API testing. We also evaluated different tool configurations, ranging from the base Llama3-8B model to fine-tuned versions, and explored multiple quantization techniques, including 2-bit, 4-bit, and 8-bit integer formats. Our study shows that small language models can perform as well as, or better than, large language models in REST API testing, balancing effectiveness and efficiency. Furthermore, LlamaRestTest outperforms state-of-the-art REST API testing tools in code coverage achieved and internal server errors identified, even when those tools use RESTGPT-enhanced specifications.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[llm-as-judge]] · [[post-training]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2501.08598v2)
