---
type: source
source_type: arxiv
title: "HTAA: Enhancing LLM Planning via Hybrid Toolset Agentization & Adaptation"
authors: Chengrui Huang, Junshuo Zhang, Zhiyuan Ma, Xikun Wang et al.
url: https://arxiv.org/abs/2604.10917v1
date: 2026-04-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.CL
tags: [agent-reliability, agent-memory, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# HTAA: Enhancing LLM Planning via Hybrid Toolset Agentization & Adaptation

**arXiv:** [2604.10917v1](https://arxiv.org/abs/2604.10917v1) · 2026-04-13 · cs.CL
**Authors:** Chengrui Huang, Junshuo Zhang, Zhiyuan Ma, Xikun Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Enabling large language models to scale and reliably use hundreds of tools is critical for real-world applications, yet challenging due to the inefficiency and error accumulation inherent in flat tool-calling architectures. To address this, we propose Hybrid Toolset Agentization & Adaptation (HTAA), a hierarchical framework for scalable tool-use planning. We propose a novel toolset agentization paradigm, which encapsulates frequently co-used tools into specialized agent tools, thereby reducing the planner's action space and mitigating redundancy. To ensure effective coordination, we design Asymmetric Planner Adaptation, a trajectory-based training paradigm that aligns the high-level planner with agent tools via backward reconstruction and forward refinement. To validate the performance of HTAA, we conduct experiments on a real-world internal dataset, InfoVerify, based on the POI validation workflow of China's largest online large-scale ride-hailing platform, featuring long-horizon executable tool trajectories. Experiments on InfoVerify and widely-used benchmarks show that HTAA consistently achieves higher task success rates, requires short tool calling trajectories, and significantly reduces context overhead compared to strong baselines. Furthermore, in a production deployment, HTAA substantially reduces manual validation effort and operational cost, demonstrating its practical efficacy.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.10917v1)
