---
type: source
source_type: arxiv
title: "AdaReasoner: Dynamic Tool Orchestration for Iterative Visual Reasoning"
authors: Mingyang Song, Haoyu Sun, Jiawei Gu, Linjie Li et al.
url: https://arxiv.org/abs/2601.18631v2
date: 2026-01-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [agentic-rl, agent-skills, agent-memory, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# AdaReasoner: Dynamic Tool Orchestration for Iterative Visual Reasoning

**arXiv:** [2601.18631v2](https://arxiv.org/abs/2601.18631v2) · 2026-01-26 · cs.AI
**Authors:** Mingyang Song, Haoyu Sun, Jiawei Gu, Linjie Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
When humans face problems beyond their immediate capabilities, they rely on tools, providing a promising paradigm for improving visual reasoning in multimodal large language models (MLLMs). Effective reasoning, therefore, hinges on knowing which tools to use, when to invoke them, and how to compose them over multiple steps, even when faced with new tools or new tasks. We introduce \textbf{AdaReasoner}, a family of multimodal models that learn tool use as a general reasoning skill rather than as tool-specific or explicitly supervised behavior. AdaReasoner is enabled by (i) a scalable data curation pipeline exposing models to long-horizon, multi-step tool interactions; (ii) Tool-GRPO, a reinforcement learning algorithm that optimizes tool selection and sequencing based on end-task success; and (iii) an adaptive learning mechanism that dynamically regulates tool usage. Together, these components allow models to infer tool utility from task context and intermediate outcomes, enabling coordination of multiple tools and generalization to unseen tools. Empirically, AdaReasoner exhibits strong tool-adaptive and generalization behaviors: it autonomously adopts beneficial tools, suppresses irrelevant ones, and adjusts tool usage frequency based on task demands, despite never being explicitly trained to do so. These capabilities translate into state-of-the-art performance across challenging benchmarks, improving the 7B base model by +24.9\% on average and surpassing strong proprietary systems such as GPT-5 on multiple tasks, including VSP and Jigsaw.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[gpt-5]] · [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.18631v2)
