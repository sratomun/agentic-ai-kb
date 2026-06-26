---
type: source
source_type: arxiv
title: "ATP-Bench: Towards Agentic Tool Planning for MLLM Interleaved Generation"
authors: Yinuo Liu, Zi Qian, Heng Zhou, Jiahao Zhang et al.
url: https://arxiv.org/abs/2603.29902v1
date: 2026-03-31
ingested: 2026-06-21
depth: abstract
auto: true
score: 23
primary: cs.AI
tags: [tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# ATP-Bench: Towards Agentic Tool Planning for MLLM Interleaved Generation

**arXiv:** [2603.29902v1](https://arxiv.org/abs/2603.29902v1) · 2026-03-31 · cs.AI
**Authors:** Yinuo Liu, Zi Qian, Heng Zhou, Jiahao Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Interleaved text-and-image generation represents a significant frontier for Multimodal Large Language Models (MLLMs), offering a more intuitive way to convey complex information. Current paradigms rely on either image generation or retrieval augmentation, yet they typically treat the two as mutually exclusive paths, failing to unify factuality with creativity. We argue that the next milestone in this field is Agentic Tool Planning, where the model serves as a central controller that autonomously determines when, where, and which tools to invoke to produce interleaved responses for visual-critical queries. To systematically evaluate this paradigm, we introduce ATP-Bench, a novel benchmark comprising 7,702 QA pairs (including 1,592 VQA pairs) across eight categories and 25 visual-critical intents, featuring human-verified queries and ground truths. Furthermore, to evaluate agentic planning independent of end-to-end execution and changing tool backends, we propose a Multi-Agent MLLM-as-a-Judge (MAM) system. MAM evaluates tool-call precision, identifies missed opportunities for tool use, and assesses overall response quality without requiring ground-truth references. Our extensive experiments on 10 state-of-the-art MLLMs reveal that models struggle with coherent interleaved planning and exhibit significant variations in tool-use behavior, highlighting substantial room for improvement and providing actionable guidance for advancing interleaved generation. Dataset and code are available at https://github.com/Qwen-Applications/ATP-Bench.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.29902v1)
