---
type: source
source_type: arxiv
title: "Mobile-Agent-v3.5: Multi-platform Fundamental GUI Agents"
authors: Haiyang Xu, Xi Zhang, Haowei Liu, Junyang Wang et al.
url: https://arxiv.org/abs/2602.16855v1
date: 2026-02-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [computer-use-agents, agent-protocols, agent-memory, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# Mobile-Agent-v3.5: Multi-platform Fundamental GUI Agents

**arXiv:** [2602.16855v1](https://arxiv.org/abs/2602.16855v1) · 2026-02-15 · cs.AI
**Authors:** Haiyang Xu, Xi Zhang, Haowei Liu, Junyang Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The paper introduces GUI-Owl-1.5, the latest native GUI agent model that features instruct/thinking variants in multiple sizes (2B/4B/8B/32B/235B) and supports a range of platforms (desktop, mobile, browser, and more) to enable cloud-edge collaboration and real-time interaction. GUI-Owl-1.5 achieves state-of-the-art results on more than 20+ GUI benchmarks on open-source models: (1) on GUI automation tasks, it obtains 56.5 on OSWorld, 71.6 on AndroidWorld, and 48.4 on WebArena; (2) on grounding tasks, it obtains 80.3 on ScreenSpotPro; (3) on tool-calling tasks, it obtains 47.6 on OSWorld-MCP, and 46.8 on MobileWorld; (4) on memory and knowledge tasks, it obtains 75.5 on GUI-Knowledge Bench. GUI-Owl-1.5 incorporates several key innovations: (1) Hybird Data Flywheel: we construct the data pipeline for UI understanding and trajectory generation based on a combination of simulated environments and cloud-based sandbox environments, in order to improve the efficiency and quality of data collection. (2) Unified Enhancement of Agent Capabilities: we use a unified thought-synthesis pipeline to enhance the model's reasoning capabilities, while placing particular emphasis on improving key agent abilities, including Tool/MCP use, memory and multi-agent adaptation; (3) Multi-platform Environment RL Scaling: We propose a new environment RL algorithm, MRPO, to address the challenges of multi-platform conflicts and the low training efficiency of long-horizon tasks. The GUI-Owl-1.5 models are open-sourced, and an online cloud-sandbox demo is available at https://github.com/X-PLUG/MobileAgent.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[mcp]] · [[osworld]] · [[webarena]] · [[androidworld]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.16855v1)
