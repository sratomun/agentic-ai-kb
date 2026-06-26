---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Training Agents Inside of Scalable World Models"
authors: Danijar Hafner, Wilson Yan, Timothy Lillicrap
url: https://arxiv.org/abs/2509.24527v1
date: 2025-09-29
citationCount: 95
influentialCitationCount: 6
velocity: 10.87
ingested: 2026-06-22
tags: [embodied-agents, agentic-rl, agentic-ai, arxiv, 2025, cited]
---

# Training Agents Inside of Scalable World Models

**arXiv [2509.24527v1](https://arxiv.org/abs/2509.24527v1)** · 2025-09-29 · **95 citations** (6 influential · 10.87/mo) · Danijar Hafner, Wilson Yan, Timothy Lillicrap

## Abstract
World models learn general knowledge from videos and simulate experience for training behaviors in imagination, offering a path towards intelligent agents. However, previous world models have been unable to accurately predict object interactions in complex environments. We introduce Dreamer 4, a scalable agent that learns to solve control tasks by reinforcement learning inside of a fast and accurate world model. In the complex video game Minecraft, the world model accurately predicts object interactions and game mechanics, outperforming previous world models by a large margin. The world model achieves real-time interactive inference on a single GPU through a shortcut forcing objective and an efficient transformer architecture. Moreover, the world model learns general action conditioning from only a small amount of data, allowing it to extract the majority of its knowledge from diverse unlabeled videos. We propose the challenge of obtaining diamonds in Minecraft from only offline data, aligning with practical applications such as robotics where learning from environment interaction can be unsafe and slow. This task requires choosing sequences of over 20,000 mouse and keyboard actions from raw pixels. By learning behaviors in imagination, Dreamer 4 is the first agent to obtain diamonds in Minecraft purely from offline data, without environment interaction. Our work provides a scalable recipe for imagination training, marking a step towards intelligent agents.

## From the paper (full-text excerpts)
**Introduction.** Introduction To solve complex tasks in embodied environments, intelligent agents need to deeply understand the world and choose successful actions. World models offer a promising approach towards this goal by learning to predict the future outcomes of potential actions from the perspective of an agent, such as a robot or a video game player. This way, world models equip agents with a deep understanding of the world and the ability to choose actions by planning or reinforcement learning in imagination. Moreover, world models can in principle learn from fixed datasets, allowing to train agents purely in imagination without the need for online interaction. Optimizing behaviors offline is valuable for many practical applications, such as robots in the physical world, where online interaction with a partially trained agent is often unsafe. World model agents, such as Dreamer 3, are among the best-performing and most robust reinforcement learning algorithms for games and robotics to date 1–6 . While these models are fast and accurate for their narrow environments, their architecture lacks…

**Method / approach.** methods have access to the same contractor dataset 15 with image inputs and low-level mouse and keyboard actions. We report the success rates of important items obtained during 60-minute episodes that start in random worlds and from empty inventory, computed over 1000 episodes. Leveraging imagination training, Dreamer 4 is the first agent to obtain diamonds in Minecraft purely from offline experience. Dreamer 4 substantially outperforms OpenAI’s VPT offline agent 15 while using 100× less data. It also outperforms our VLA agent 41,42 , which leverages the general knowledge of the Gemma 3 visionlanguage model 43 , nearly tripling its success rate for crafting iron pickaxes. 4. Experiments We perform a wide range of experiments to evaluate and explore the capabilities of Dreamer 4. The majority of our experiments focus on Minecraft, a complex video game that features infinite open worlds including monsters and hundreds of items that can be mined or crafted, with raw pixel observations a…

**Results.** Experiments We perform a wide range of experiments to evaluate and explore the capabilities of Dreamer 4. The majority of our experiments focus on Minecraft, a complex video game that features infinite open worlds including monsters and hundreds of items that can be mined or crafted, with raw pixel observations and low-level mouse and keyboard actions. We primarily use the VPT dataset 15 that contains 2541 hours of contractor gameplay with 360p video and mouse and keyboard actions at 20 FPS. The experiments are designed to answer the following questions: • Does Dreamer 4 learn to solve challenging control tasks purely by imagination training inside the world model, without online environment interaction? (Section 4.1) • How well does Dreamer 4 learn to predict accurate object interactions and game mechanics in Minecraft compared to previous world models? (Section 4.2) • How much action data does Dreamer 4 need for learning action condit…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agentic-rl|Agentic RL]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2509.24527v1.md` · `raw/arxiv/2509.24527v1.fulltext.md`
