---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "GTA1: GUI Test-time Scaling Agent"
authors: Yan Yang, Dongxu Li, Yutong Dai, Yuhao Yang et al.
url: https://arxiv.org/abs/2507.05791v5
date: 2025-07-08
citationCount: 82
influentialCitationCount: 15
velocity: 7.15
ingested: 2026-06-22
tags: [agentic-rl, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# GTA1: GUI Test-time Scaling Agent

**arXiv [2507.05791v5](https://arxiv.org/abs/2507.05791v5)** · 2025-07-08 · **82 citations** (15 influential · 7.15/mo) · Yan Yang, Dongxu Li, Yutong Dai, Yuhao Yang et al.

## Abstract
Graphical user interface (GUI) agents autonomously complete tasks across platforms (\eg, Linux) by sequentially decomposing user instructions into action proposals that iteratively interact with visual elements in the evolving environment. However, two main challenges arise: i) planning (\ie, the action proposal sequence) under expansive action space, where selecting an appropriate plan is non-trivial, as many valid ones may exist; ii) accurately grounding actions in complex and high-resolution interfaces, \ie, precisely interacting with visual targets. This paper investigates the aforementioned challenges with our \textbf{G}UI \textbf{T}est-time Scaling \textbf{A}gent, namely GTA1. First, we conduct test-time scaling to select the most appropriate action proposal: at each step, multiple candidate proposals are sampled and evaluated and selected by a judge model. It trades off computation for better decision quality by concurrent sampling. Second, we propose a model that improves grounding of the selected action proposals to its corresponding visual elements. Our key insight is that reinforcement learning (RL) facilitates grounding through inherent objective alignments, rewarding successful clicks on interface elements. Experimentally, GTA1 achieves state-of-the-art performance on both grounding and agent task execution benchmarks. The code and models are released here.

## From the paper (full-text excerpts)
**Introduction.** Introduction Automating task completions across diverse platforms through GUI agents represents a significant milestone toward general artificial intelligence, supporting activities from online orders to expert workflows [1]. To solve a task, a GUI agent translates user instructions into multi-step interactions such as action proposals consisting of clicks or keystrokes [2]. This introduces a planning challenge, as multiple valid action proposal sequences may exist for the same user task. The challenge is further amplified by the high-resolution (up to 4K), complex, and hierarchical layouts of GUI [3–6], requiring accurate coordinate identification of the target interface elements. This work aims to address both challenges (i. e., planning and grounding) towards a performant GUI agent. Formally, existing works [1, 6–9] often pair a GUI grounding model with a planner (e.g., o3 [10]). The planner determines an action proposal at each step, while the grounding model locates the target interface elements for interactions (e.g., click areas). However, due to the inherent flexibility of u…

**Method / approach.** methods. (a) Grounding accuracy (%) on the Verified [11] time. ShowUI-2B ScreenSpot-Pro benchmark [3] across CogAgent-18B model scales in billions (B) of parameters. (b) Success rate (%) on the OSWorldVerified benchmark [11] over time. “thinking” (i. e., CoT reasoning), before predicting interaction coordinates, training with a format reward to enforce reasoning(i.and clickreasoning), reward to before ensure predicting predictionsinteraction fall withincoordinates, the target element. furthertoextend this “thinking” e., aCoT training Some with amethods format reward enforce approach by predicting the bounding box of the target UI element [16, 17]. While improving over SFT, we ask: reasoning and a click reward to ensure predictions fall within the target element. Some methods further extend this is explicit “thinking” or auxiliary bounding effective GUI grounding? approach by predicting the bounding box ofbox thereward target necessary UI elementfor[16, 17]. While improving over SFT, w…

**Results.** Experimentally, GTA1 achieves state-of-the-art performance on both grounding and agent task execution benchmarks. The code and models are released here. 1 Introduction Automating task completions across diverse platforms through GUI agents represents a significant milestone toward general artificial intelligence, supporting activities from online orders to expert workflows [1]. To solve a task, a GUI agent translates user instructions into multi-step interactions such as action proposals consisting of clicks or keystrokes [2]. This introduces a planning challenge, as multiple valid action proposal sequences may exist for the same user task. The challenge is further amplified by the high-resolution (up to 4K), complex, and hierarchical layouts of GUI [3–6], requiring accurate coordinate identification of the target interface elements. This work aims to address both challenges (i. e., planning and grounding) towards a performant GUI ag…

**Conclusion.** Conclusion and Limitation This paper investigates two key challenges toward building intelligent GUI agents: selecting effective plans and precise grounding in complex interfaces. We address these challenges with two strategies. First, to improve task planning, we introduce a scalable test-time strategy that concurrent samples multiple action proposals at each step and use a multimodal large language model judge to select the most suitable one. Second, we propose a grounding model, which employs a simple RL-based optimization approach that directly rewards successful clicks on target elements, bypassing the explicit “thinking” required by prior methods. Overall, GTA1 achieves state-of-the-art performance on standard grounding benchmarks an…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2507.05791v5.md` · `raw/arxiv/2507.05791v5.fulltext.md`
