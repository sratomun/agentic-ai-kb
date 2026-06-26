---
type: source
source_type: arxiv
title: "SpotAgent: Grounding Visual Geo-localization in Large Vision-Language Models through Agentic Reasoning"
authors: Furong Jia, Ling Dai, Wenjin Deng, Fan Zhang et al.
url: https://arxiv.org/abs/2602.09463v3
date: 2026-02-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 25
primary: cs.AI
tags: [agentic-rl, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# SpotAgent: Grounding Visual Geo-localization in Large Vision-Language Models through Agentic Reasoning

**arXiv:** [2602.09463v3](https://arxiv.org/abs/2602.09463v3) · 2026-02-10 · cs.AI
**Authors:** Furong Jia, Ling Dai, Wenjin Deng, Fan Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Vision-Language Models (LVLMs) have demonstrated strong reasoning capabilities in geo-localization, yet they often struggle in real-world scenarios where visual cues are sparse, long-tailed, and highly ambiguous. Previous approaches, bound by internal knowledge, often fail to provide verifiable results, yielding confident but ungrounded predictions when faced with confounded evidence. To address these challenges, we propose SpotAgent, a framework that formalizes geo-localization into an agentic reasoning process that leverages expert-level reasoning to synergize visual interpretation with tool-assisted verification. SpotAgent actively explores and verifies visual cues by leveraging external tools (e.g., web search, maps) through a ReAct diagram. We introduce a 3-stage post-training pipeline starting with a Supervised Fine-Tuning (SFT) stage for basic alignment, followed by an Agentic Cold Start phase utilizing high-quality trajectories synthesized via a Multi-Agent framework, aiming to instill tool-calling expertise. Subsequently, the model's reasoning capabilities are refined through Reinforcement Learning. We propose a Spatially-Aware Dynamic Filtering strategy to enhance the efficiency of the RL stage by prioritizing learnable samples based on spatial difficulty. Extensive experiments on standard benchmarks demonstrate that SpotAgent achieves state-of-the-art performance, effectively mitigating hallucinations while delivering precise and verifiable geo-localization.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.09463v3)
