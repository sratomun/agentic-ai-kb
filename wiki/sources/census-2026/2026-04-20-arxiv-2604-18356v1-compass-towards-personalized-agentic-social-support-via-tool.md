---
type: source
source_type: arxiv
title: "ComPASS: Towards Personalized Agentic Social Support via Tool-Augmented Companionship"
authors: Zhaopei Huang, Yanfeng Jia, Jiayi Zhao, Xinjie Zhang et al.
url: https://arxiv.org/abs/2604.18356v1
date: 2026-04-20
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CL
tags: [human-agent-interaction, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# ComPASS: Towards Personalized Agentic Social Support via Tool-Augmented Companionship

**arXiv:** [2604.18356v1](https://arxiv.org/abs/2604.18356v1) · 2026-04-20 · cs.CL
**Authors:** Zhaopei Huang, Yanfeng Jia, Jiayi Zhao, Xinjie Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Developing compassionate interactive systems requires agents to not only understand user emotions but also provide diverse, substantive support. While recent works explore empathetic dialogue generation, they remain limited in response form and content, struggling to satisfy diverse needs across users and contexts. To address this, we explore empowering agents with external tools to execute diverse actions. Grounded in the psychological concept of "social support", this paradigm delivers substantive, human-like companionship. Specifically, we first design a dozen user-centric tools simulating various multimedia applications, which can cover different types of social support behaviors in human-agent interaction scenarios. We then construct ComPASS-Bench, the first personalized social support benchmark for LLM-based agents, via multi-step automated synthesis and manual refinement. Based on ComPASS-Bench, we further synthesize tool use records to fine-tune the Qwen3-8B model, yielding a task-specific ComPASS-Qwen. Comprehensive evaluations across two settings reveal that while the evaluated LLMs can generate valid tool-calling requests with high success rates, significant gaps remain in final response quality. Moreover, tool-augmented responses achieve better overall performance than directly producing conversational empathy. Notably, our trained ComPASS-Qwen demonstrates substantial improvements over its base model, achieving comparable performance to several large-scale models. Our code and data are available at https://github.com/hzp3517/ComPASS.

## Graph
- **Concepts:** [[human-agent-interaction|Human-agent interaction]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.18356v1)
