---
type: concept
tags: [agents, world-models, simulation, planning]
created: 2026-06-22
updated: 2026-06-22
census_count: 258
kind: domain
---

# World models

*Learned models of environment dynamics that let agents simulate, predict, and plan before acting.*

## What it is
Models that learn "what happens next" in an environment — increasingly video/latent-diffusion models — so an agent can roll out futures internally instead of acting by trial and error. The model-based counterweight to pure RL.

## Why it matters
The bet on **model-based agents**: planning against a learned simulator is more sample-efficient and safer than learning by failure, which matters most in physical and high-stakes settings. It's a longer-horizon research frontier, most relevant to [[embodied-agents]] and [[autonomous-driving-agents]].

## What the evidence shows
**2025 foundations.** Two strands. **Generative world models for simulation:** GAIA-2, a controllable multi-view latent-diffusion model for autonomous driving, generates diverse synthetic scenarios — cutting reliance on expensive real-world data and enabling safe, repeatable evaluation (→ [[2025-03-26-arxiv-2503-20523v1-gaia-2-a-controllable-multi-view-generative-world]]). **Video models as implicit world models:** a study of Veo found general video models acting as zero-shot learners/reasoners, with a striking, rapid capability jump from Veo 2 to Veo 3 in ~half a year — evidence that video pretraining is becoming a world-modeling substrate (→ [[2025-09-24-arxiv-2509-20328v2-video-models-are-zero-shot-learners-and-reasoners]]).
- _Honest note: deep coverage here is light relative to the ~258-paper census cluster; this is a watch-area more than a settled one._

## Relationships
- commentary: [[demis-hassabis]] (multimodal-from-the-start; Genie), [[jeff-dean]] (Genie 3 / Gemini Robotics)
- debate: [[debate-llms-path-to-agi]] ([[yann-lecun]] vs [[sonya-huang]])
- used by [[embodied-agents]], [[autonomous-driving-agents]]
- relates to [[self-evolving-agents]]
- a frontier of [[agentic-ai]]

## Key 2025 papers (citation-ranked)
- **169** · [[2025-09-24-arxiv-2509-20328v2-video-models-are-zero-shot-learners-and-reasoners|Video models are zero-shot learners and reasoners]]
- **143** · [[2025-03-26-arxiv-2503-20523v1-gaia-2-a-controllable-multi-view-generative-world|GAIA-2: A Controllable Multi-View Generative World Model for Autonomous Driving]]
