---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "AgenTracer: Who Is Inducing Failure in the LLM Agentic Systems?"
authors: Guibin Zhang, Junhao Wang, Junjie Chen, Wangchunshu Zhou et al.
url: https://arxiv.org/abs/2509.03312v2
date: 2025-09-03
citationCount: 51
influentialCitationCount: 5
velocity: 5.32
ingested: 2026-06-22
tags: [clinical-agents, agent-reliability, self-evolving-agents, agentic-rl, tool-use, arxiv, 2025, cited]
---

# AgenTracer: Who Is Inducing Failure in the LLM Agentic Systems?

**arXiv [2509.03312v2](https://arxiv.org/abs/2509.03312v2)** · 2025-09-03 · **51 citations** (5 influential · 5.32/mo) · Guibin Zhang, Junhao Wang, Junjie Chen, Wangchunshu Zhou et al.

## Abstract
Large Language Model (LLM)-based agentic systems, often comprising multiple models, complex tool invocations, and orchestration protocols, substantially outperform monolithic agents. Yet this very sophistication amplifies their fragility, making them more prone to system failure. Pinpointing the specific agent or step responsible for an error within long execution traces defines the task of agentic system failure attribution. Current state-of-the-art reasoning LLMs, however, remain strikingly inadequate for this challenge, with accuracy generally below 10%. To address this gap, we propose AgenTracer, the first automated framework for annotating failed multi-agent trajectories via counterfactual replay and programmed fault injection, producing the curated dataset TracerTraj. Leveraging this resource, we develop AgenTracer-8B, a lightweight failure tracer trained with multi-granular reinforcement learning, capable of efficiently diagnosing errors in verbose multi-agent interactions. On the Who&When benchmark, AgenTracer-8B outperforms giant proprietary LLMs like Gemini-2.5-Pro and Claude-4-Sonnet by up to 18.18%, setting a new standard in LLM agentic failure attribution. More importantly, AgenTracer-8B delivers actionable feedback to off-the-shelf multi-agent systems like MetaGPT and MaAS with 4.8-14.2% performance gains, empowering self-correcting and self-evolving agentic AI.

## From the paper (full-text excerpts)
**Method / approach.** methodology, on developing swift and accurate multi-agent failure localizer, which we also refer to as a tracer. Present Framework. To address the aforementioned research gap, we present (1) AgenTracer, a fully automated pipeline for constructing well-annotated multi-agent failure trajectories, and (2) AgenTracer-8B, a lightweight failure attributor for multi-agent systems. Methodologically, AgenTracer leverages ♣ counterfactual replay, systematically replacing agent actions with oracle guidance to identify the decisive error step responsible for system failure. To enhance data diversity and ensure annotation precision, it further adopts ♠ programmatic fault injection, synthetically generating failure instances by perturbing successful trajectories through targeted corruption. Further, we fine-tune Q WEN 3-8B on the curated dataset to obtain AgenTracer-8B via reinforcement learning (RL), enabling it to analyze long-horizon multi-agent collaboration traces. AgenTracer-8B takes as input…

**Results.** Experiments show that AgenTracer-8B facilitates (I) accurate attribution, outperforming giant LLMs like D EEP S EEK -R1 by ∼ 12.21% and G EMINI -2.5-P RO 2 AgenTracer by ∼ 18.18% on Who&When benchmark; and (II) self-evolution, enabling off-the-shelf agentic systems to improve performance by 4.8 ∼ 14.2%. 2 R ELATED W ORKS LLM-based Multi-Agent System. Contemporary multi-agent systems can be broadly categorized by their level of automation into three classes: ■ Handcrafted, where the entire system configuration (e.g., LLM backbone, prompting strategies, and communication protocols) is manually specified represented by AutoGen (Wu et al., 2023), AutoGPT (Richards & et al., 2023), Camel (Li et al., 2023), and ChatDev (Qian et al., 2023); ■ Partially Automated, which automate specific system components: for example, AutoAgent (Chen et al., 2023a), LLMSelector (Chen et al., 2025), and MasRouter (Yue et al., 2025) automate agent role ass…

**Conclusion.** limitations of relying on a single monolithic model have become increasingly conspicuous. 1 AgenTracer Consequently, numerous multi-agent frameworks, motivated by collective intelligence (Wang et al., 2025a; Zhang et al., 2024a;b) and the society of mind theory (Minsky, 1988; Li et al., 2023), have emerged, ensembling multiple LLM agents to achieve refined subtask orchestration (Zhang et al., 2025d; Hu et al., 2025), ultra-long context handling (Zhang et al., 2024d), and broader environmental perception (Jiang et al., 2024). These systems have demonstrated superior performance over single-agent counterparts across a range of complex real-world domains, including data science engineering (Hong et al., 2024), scientific discovery (Ghareeb…

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]]
- **Entities:** [[claude]]
- **Raw:** `raw/arxiv/2509.03312v2.md` · `raw/arxiv/2509.03312v2.fulltext.md`
