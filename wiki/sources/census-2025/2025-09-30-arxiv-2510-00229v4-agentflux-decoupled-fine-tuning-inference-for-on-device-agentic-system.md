---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "AgentFlux: Decoupled Fine-Tuning & Inference for On-Device Agentic Systems"
authors: Rohan Kadekodi et al.
url: https://arxiv.org/abs/2510.00229v4
date: 2025-09-30
score: 23
primary: cs.AI
tags: [arxiv, auto-ingested, small-language-models, tool-use, llm-as-judge, post-training, reasoning-models]
---

# AgentFlux: Decoupled Fine-Tuning & Inference for On-Device Agentic Systems

**arXiv:** [2510.00229v4](https://arxiv.org/abs/2510.00229v4) · 2025-09-30 · cs.AI
**Authors:** Rohan Kadekodi et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The deployment of Large Language Models (LLMs) as agentic orchestrators has revolutionized task automation, but the need for privacy-preserving, cost-effective solutions demands on-device inference capabilities. However, local LLMs consistently underperform compared to frontier models in tool calling scenarios, struggling with both tool selection from large tool sets and accurate argument generation for complex parameter structures. We introduce a methodology that disaggregates a tool-calling task into two distinct subtasks: tool selection and argument generation. We propose "decoupled fine-tuning", a novel post-training approach that employs LoRA fine-tuning to create dedicated LoRA adapters for tool selection and tool-specific argument generation using separate loss masking for each of the subtasks. Furthermore, we present AgentFlux, an inference framework that leverages the LoRA adapters created using decoupled fine-tuning to perform efficient agent orchestration with the help of local models on end-user devices. AgentFlux decomposes the tool-call generation step into tool selection and argument generation, and dynamically loads the corresponding LoRA adapters to generate tool calls. Additionally, AgentFlux implements hierarchical orchestration to restrict the number of tools required for tool selection. Our experiments on the MCP-Bench benchmark demonstrate that the Qwen-2.5-7B model trained using decoupled fine-tuning improves the tool calling accuracy of the base model by 46%, and outperforms other local reasoning, non-reasoning and fine-tuned models of similar size in all cases, and models that are 2x larger, in most cases.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[tool-use]] · [[llm-as-judge]] · [[post-training]] · [[reasoning-models]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2510.00229v4)
