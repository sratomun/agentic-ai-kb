---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Agent KB: Leveraging Cross-Domain Experience for Agentic Problem Solving"
authors: Xiangru Tang, Tianrui Qin, Tianhao Peng, Ziyang Zhou et al.
url: https://arxiv.org/abs/2507.06229v5
date: 2025-07-08
citationCount: 60
influentialCitationCount: 3
velocity: 5.23
ingested: 2026-06-22
tags: [clinical-agents, coding-agents, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# Agent KB: Leveraging Cross-Domain Experience for Agentic Problem Solving

**arXiv [2507.06229v5](https://arxiv.org/abs/2507.06229v5)** · 2025-07-08 · **60 citations** (3 influential · 5.23/mo) · Xiangru Tang, Tianrui Qin, Tianhao Peng, Ziyang Zhou et al.

## Abstract
AI agent frameworks operate in isolation, forcing agents to rediscover solutions and repeat mistakes across different systems. Despite valuable problem-solving experiences accumulated by frameworks like smolagents, OpenHands, and OWL, this knowledge remains trapped within individual systems, preventing the emergence of collective intelligence. Current memory systems focus on individual agents or framework-specific demonstrations, failing to enable cross-architecture knowledge transfer. We introduce AGENT KB, a universal memory infrastructure enabling seamless experience sharing across heterogeneous agent frameworks without retraining. AGENT KB aggregates trajectories into a structured knowledge base and serves lightweight APIs. At inference time, hybrid retrieval operates through two stages: planning seeds agents with cross-domain workflows, while feedback applies targeted diagnostic fixes. A disagreement gate ensures retrieved knowledge enhances rather than disrupts reasoning, addressing knowledge interference in cross-framework transfer. We validate AGENT KB across major frameworks on GAIA, Humanity's Last Exam, GPQA, and SWE-bench. Results show substantial improvements across diverse model families: compared to baseline pass@1, smolagents with AGENT KB achieve up to 18.7pp gains at pass@3 (55.2% -> 73.9%), while OpenHands improves 4.0pp on SWE-bench pass@1 (24.3% -> 28.3%). Similar improvements are observed across all base model families. Ablations confirm that hybrid retrieval and feedback stages are essential, with automatically generated experiences matching manual curation. This establishes the foundation for collective agent intelligence through shared memory infrastructures.

## From the paper (full-text excerpts)
**Method / approach.** methods have also evolved to incorporate neuroscience inspiration or multi-agent variants (Ye, 2025; Wang et al., 2025; Squire et al., 2015; Wang et al., 2024d; Zhu et al., 2024; Qiao et al., 2024; Xu et al., 2024; Chen et al., 2025; Ganguli et al., 2025; Lv et al., 2024; Shuster et al., 2021; Niu et al., 2024; Mala et al., 2025). Despite improvements, existing approaches face significant limitations: they are primarily tailored for single agents, retain separate memory systems that prevent shared knowledge, and lack ways to reuse experiences across different areas, which makes them vulnerable in new or unfamiliar contexts. 2.2 AGENTIC K NOWLEDGE T RANSFER Alongside memory infrastructures, another research area condenses agent trajectories into workflow priors that guide future problem solving: retrieval-based systems (Zheng et al., 2023; Zhou et al., 2024a) stabilize tool use with exemplar traces, mined sub-workflows support reuse across tasks (Wang et al., 2024d), and templating p…

**Results.** experiments use smolagents (backed by GPT-4o, GPT-4.1, Claude-3.7, Qwen-3 32B, and DeepSeek-R1) and OWL (GPT-4o); SWEbench Lite is evaluated with SWE-Agent (GPT-4.1, o3-mini) and OpenHands (GPT-4o, GPT-4.1, Claude-3.7, Qwen-3 32B, DeepSeek-R1, o3-mini). Each benchmark instance is solved in three sequential passes: pass@1 retrieves cross-task experiences without exposure to held-out labels, pass@2 enriches AGENT KB with failure diagnoses from the first attempt, and pass@3 revisits unresolved cases using the expanded retrieval pool. Unless otherwise stated, we fix the base model to GPT-4.1, the temperature to 1.0, and the retrieval top-k to 3, mirroring the setting used for Figure 3. 2 We deliberately removed the biology & chemistry subset from Humanity’s Last Exam as a test set. 5 Table 1: Results on GAIA benchmark (val set). We report pass@1 for all standard baselines. For methods that build on top of a base framework (A-M EM (Xu et…

**Conclusion.** limitations: they are primarily tailored for single agents, retain separate memory systems that prevent shared knowledge, and lack ways to reuse experiences across different areas, which makes them vulnerable in new or unfamiliar contexts. 2.2 AGENTIC K NOWLEDGE T RANSFER Alongside memory infrastructures, another research area condenses agent trajectories into workflow priors that guide future problem solving: retrieval-based systems (Zheng et al., 2023; Zhou et al., 2024a) stabilize tool use with exemplar traces, mined sub-workflows support reuse across tasks (Wang et al., 2024d), and templating pipelines refine plans within narrow families (Tan et al., 2025; Liu et al., 2025e). Knowledge-augmented and collaborative planners extend these…

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[coding-agents|Coding agents]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]] · [[gaia-benchmark]]
- **Raw:** `raw/arxiv/2507.06229v5.md` · `raw/arxiv/2507.06229v5.fulltext.md`
