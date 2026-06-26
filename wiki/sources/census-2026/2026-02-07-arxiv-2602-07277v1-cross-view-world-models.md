---
type: source
source_type: arxiv
title: "Cross-View World Models"
authors: Rishabh Sharma, Gijs Hogervorst, Wayne E. Mackey, David J. Heeger et al.
url: https://arxiv.org/abs/2602.07277v1
date: 2026-02-07
ingested: 2026-06-21
depth: abstract
auto: true
score: 7
primary: cs.CV
tags: [embodied-agents, multi-agent-systems, arxiv, auto-ingested]
---

# Cross-View World Models

**arXiv:** [2602.07277v1](https://arxiv.org/abs/2602.07277v1) · 2026-02-07 · cs.CV
**Authors:** Rishabh Sharma, Gijs Hogervorst, Wayne E. Mackey, David J. Heeger et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
World models enable agents to plan by imagining future states, but existing approaches operate from a single viewpoint, typically egocentric, even when other perspectives would make planning easier; navigation, for instance, benefits from a bird's-eye view. We introduce Cross-View World Models (XVWM), trained with a cross-view prediction objective: given a sequence of frames from one viewpoint, predict the future state from the same or a different viewpoint after an action is taken. Enforcing cross-view consistency acts as geometric regularization: because the input and output views may share little or no visual overlap, to predict across viewpoints, the model must learn view-invariant representations of the environment's 3D structure. We train on synchronized multi-view gameplay data from Aimlabs, an aim-training platform providing precisely aligned multi-camera recordings with high-frequency action labels. The resulting model gives agents parallel imagination streams across viewpoints, enabling planning in whichever frame of reference best suits the task while executing from the egocentric view. Our results show that multi-view consistency provides a strong learning signal for spatially grounded representations. Finally, predicting the consequences of one's actions from another viewpoint may offer a foundation for perspective-taking in multi-agent settings.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[bird-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.07277v1)
