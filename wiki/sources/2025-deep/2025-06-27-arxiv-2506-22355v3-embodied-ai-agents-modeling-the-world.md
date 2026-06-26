---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Embodied AI Agents: Modeling the World"
authors: Pascale Fung, Yoram Bachrach, Asli Celikyilmaz, Kamalika Chaudhuri et al.
url: https://arxiv.org/abs/2506.22355v3
date: 2025-06-27
citationCount: 71
influentialCitationCount: 2
velocity: 6.0
ingested: 2026-06-22
tags: [embodied-agents, human-agent-interaction, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# Embodied AI Agents: Modeling the World

**arXiv [2506.22355v3](https://arxiv.org/abs/2506.22355v3)** · 2025-06-27 · **71 citations** (2 influential · 6.0/mo) · Pascale Fung, Yoram Bachrach, Asli Celikyilmaz, Kamalika Chaudhuri et al.

## Abstract
This paper describes our research on AI agents embodied in visual, virtual or physical forms, enabling them to interact with both users and their environments. These agents, which include virtual avatars, wearable devices, and robots, are designed to perceive, learn and act within their surroundings, which makes them more similar to how humans learn and interact with the environments as compared to disembodied agents. We propose that the development of world models is central to reasoning and planning of embodied AI agents, allowing these agents to understand and predict their environment, to understand user intentions and social contexts, thereby enhancing their ability to perform complex tasks autonomously. World modeling encompasses the integration of multimodal perception, planning through reasoning for action and control, and memory to create a comprehensive understanding of the physical world. Beyond the physical world, we also propose to learn the mental world model of users to enable better human-agent collaboration.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Embodied AI Agent Types and Applications 2.1 Virtual Embodied Agents 2.2 Wearable Agents 2.3 Robotic agents 3 World Models for Embodied Agents 3.1 Multimodal Perception 3.1.1 Image Video 3.1.2 Audio Speech Key Challenges Future Directions 3.1.3 Touch 3.2 Physical World Models 3.2.1 Low-level motion planning Visual world models. Planning with world models. Generative world models. Joint-Embedding predictive world models. 3.2.2 High-level action planning 3.3 Mental World Models 3.4 Actions and Control 3.5 Memory 3.5.1 Existing memories Fixed memory: The model weights. Working memory. External memory. 3.5.2 Challenge and objective of Memory for world models Limitations of current memories. Personalization. Life-long training. 3.6 World Model Benchmarks 3.6.1 Minimal Video Pairs 3.6.2 IntPhys2 3.6.3 CausalVQA 3.6.4 World Prediction Benchmark 4 Type I: Virtual Embodied Agents 4.1 Capability Taxonomy 4.2 Architecture and Models 4.3 Benchmarks Dataset. Subjecti…

**Method / approach.** method from Rubinstein ( 1997 ) . Planning (system 2) is more costly than calling a policy (system 1) but is more likely to generalize zero-shot outside the training distribution. Learned world models have been used for both use cases: 1) training a policy on trajectories imagined with the world model, 2) using the learned model for model-based planning. Figure 3 : Planning with a JEPA visual world model for a robotic manipulation task. The future is imagined by encoding the context frames with the encoder E θ subscript 𝐸 𝜃 E_{\theta} italic_E start_POSTSUBSCRIPT italic_θ end_POSTSUBSCRIPT and rolling out the predictor P ϕ subscript 𝑃 italic-ϕ P_{\phi} italic_P start_POSTSUBSCRIPT italic_ϕ end_POSTSUBSCRIPT from these context visual embeddings and actions. To plan, any cost function with respect to the goal can be used. In this figure, the L 1 subscript 𝐿 1 L_{1} italic_L start_POSTSUBSCRIPT 1 end_POSTSUBSCRIPT distance of the last imagined state to the goal state embedding is opti…

**Results.** experimental scientists in their laboratory work, and other scientists as research assistants. As research in this field continues to advance, we can expect to see more sophisticated and effective wearable agents that can provide personalized assistance, coaching, and tutoring to users. 2.3 Robotic agents Robotic agents are AI systems used to operate a robot in the physical environment either performing tasks independently or through collaboration and interaction with humans. As opposed to specialized “single-function”-robots we review more general purpose robotic agents. The embodiment can take on various forms, however we focus on agents that can execute a diverse set of tasks in new environments. Such robotics agents are observing their environment, much like humans, via a variety of senses (for instance RGB cameras, tactile sensors, IMUs, force/torque sensors, audio sensors to name a few), and can control their robotic body v…

**Conclusion.** Conclusion Embodied AI Agents: Modeling the World Pascale Fung Yoram Bachrach Asli Celikyilmaz Kamalika Chaudhuri Delong Chen Willy Chung Emmanuel Dupoux Hongyu Gong Hervé Jégou Alessandro Lazaric Arjun Majumdar Andrea Madotto Franziska Meier Florian Metze Louis-Philippe Morency Théo Moutakanni Juan Pino Basile Terver Joseph Tighe Paden Tomasello Jitendra Malik Meta AI Research pascalefung@meta.com (July 7, 2025) Abstract This paper describes our research on AI agents embodied in visual, virtual or physical forms, enabling them to interact more naturally with both users and their environments. These agents, which include virtual avatars, wearable devices, and robots, are designed…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[human-agent-interaction|Human-agent interaction]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2506.22355v3.md` · `raw/arxiv/2506.22355v3.fulltext.md`
