---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "WebSailor-V2: Bridging the Chasm to Proprietary Agents via Synthetic Data and Scalable Reinforcement Learning"
authors: Kuan Li, Zhongwang Zhang, Huifeng Yin, Rui Ye et al.
url: https://arxiv.org/abs/2509.13305v1
date: 2025-09-16
citationCount: 50
influentialCitationCount: 6
velocity: 5.46
ingested: 2026-06-22
tags: [agentic-rl, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# WebSailor-V2: Bridging the Chasm to Proprietary Agents via Synthetic Data and Scalable Reinforcement Learning

**arXiv [2509.13305v1](https://arxiv.org/abs/2509.13305v1)** · 2025-09-16 · **50 citations** (6 influential · 5.46/mo) · Kuan Li, Zhongwang Zhang, Huifeng Yin, Rui Ye et al.

## Abstract
Transcending human cognitive limitations represents a critical frontier in LLM training. Proprietary agentic systems like DeepResearch have demonstrated superhuman capabilities on extremely complex information-seeking benchmarks such as BrowseComp, a feat previously unattainable. We posit that their success hinges on a sophisticated reasoning pattern absent in open-source models: the ability to systematically reduce extreme uncertainty when navigating vast information landscapes. Based on this insight, we introduce WebSailor, a complete post-training methodology designed to instill this crucial capability. Our approach involves generating novel, high-uncertainty tasks through structured sampling and information obfuscation, RFT cold start, and an efficient agentic RL training algorithm, Duplicating Sampling Policy Optimization (DUPO). With this integrated pipeline, WebSailor significantly outperforms all open-source agents in complex information-seeking tasks, matching proprietary agents' performance and closing the capability gap.

## From the paper (full-text excerpts)
**Introduction.** Introduction In the pursuit of Artificial General Intelligence (AGI), autonomous AI agents represent a critical milestone, with "Deep Research" emerging as a core paradigm for achieving more generalized capabilities. By leveraging external tools like search engines and web browsers, these agents can autonomously conduct systematic and in-depth analyses to tackle complex, multi-step research tasks through dynamic reasoning and iterative information retrieval (OpenAI, 2025a; AI, 2025). Despite recent advancements across the research community, spanning improvements from both perspectives of data and training (Wu et al., 2025b; Li et al., 2025b; Liu et al., 2025a; Nguyen et al., 2025; Li et al., 2025c; Wu et al., 2025a; Tao et al., 2025), a considerable performance gap still persists between open-source solutions and proprietary systems (e.g., OpenAI DeepResearch (OpenAI, 2025a)), leading to a bottleneck in democratizing powerful research capabilities. This performance disparity primarily stems from fundamental challenges in two of the most critical stages for developing powerful agent…

**Method / approach.** methodologies often rely on a narrow set of uncertainty definitions, such as obfuscation (Li et al., 2025b; Gao et al.; Shi et al., 2025). A wider variety of uncertainty types is needed to elicit more diverse and sophisticated reasoning behaviors from the base model, better preparing it for the ambiguity inherent in real-world research. (2) Training: lack of scalable reinforcement learning (RL) training environment. Creating a scalable and robust RL training environment for agentic systems poses a significant challenge, which typically demands massive rollouts, each potentially involving numerous tool calls. The high cost and engineering complexity of high-concurrency requests to external APIs can lead to practical issues like tool latency, API failures, and inconsistent outputs. These issues would contaminate the training data, degrade the model’s learned policies, and severely hinder our rapid iteration of RL training algorithms (Qin et al., 2025; Wang et al., 2025). In this paper,…

**Results.** experimentation and data curation, providing a low-cost, exceptionally fast, and fully controllable platform. Through meticulous design, it achieves high fidelity, ensuring that the agent’s interaction dynamics, state transitions, and reward mechanisms closely mirror those of a real-world setting. Second, recognizing that RL training in a real environment is a complex engineering problem—especially concerning the consistency of tool returns after toolset expansion, the reproducibility of trajectory sampling, and the need for high concurrency and fault tolerance—we manage our toolkit in a systematic way to ensure robustness and reliability. Finally, our data construction and RL training pipelines are integrated into a symbiotic feedback loop. This dynamic mechanism allows the system to synthesize and filter high-quality data based on training dynamics, enabling the model to continually refine its policies and learn from a stream of relev…

**Conclusion.** conclusions from ablation studies. To address this, we build a simulated environment using an offline Wikipedia database and a corresponding suite of web tools. To populate this environment with high-quality, structurally complex tasks, we adapted our SailorFog-QA-V2 generation pipeline to operate on this offline corpus, thereby creating a dedicated set of training and testing data tailored to the simulation. This has enabled us to conduct high-frequency algorithmic experiments on a highly cost-efficient, fast, and fully controllable platform, thereby significantly accelerating our development and iteration process. Real environment. While the simulated environment is invaluable for rapid prototyping and algorithm validation, the ultimate g…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2509.13305v1.md` · `raw/arxiv/2509.13305v1.fulltext.md`
