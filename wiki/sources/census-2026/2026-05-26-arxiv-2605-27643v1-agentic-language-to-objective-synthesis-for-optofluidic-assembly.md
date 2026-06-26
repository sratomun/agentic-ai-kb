---
type: source
source_type: arxiv
title: "Agentic Language-to-Objective Synthesis for Optofluidic Assembly"
authors: Ivan Saraev, Elena Erben, Weida Liao, Fan Nan et al.
url: https://arxiv.org/abs/2605.27643v1
date: 2026-05-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.RO
tags: [autonomous-driving-agents, embodied-agents, agent-reliability, arxiv, auto-ingested]
---

# Agentic Language-to-Objective Synthesis for Optofluidic Assembly

**arXiv:** [2605.27643v1](https://arxiv.org/abs/2605.27643v1) · 2026-05-26 · cs.RO
**Authors:** Ivan Saraev, Elena Erben, Weida Liao, Fan Nan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Light-based advanced manufacturing increasingly requires programmable, closed-loop tools that translate human design intent into executable operations at small length scales. Yet a key bottleneck persists across robotic and manufacturing modalities: turning user intent into machine-readable objectives that are reliably executable. While micro-robotics offers versatile manipulation via optical actuation of fluids, mathematically tractable goal specification remains manual and hard to reuse. Here, we introduce Speak-to-Objective, a modular agentic pipeline that uses a conditioned Large Language Model (LLM) to translate spoken or written commands into fully differentiable objective functions for assembling microparticles in a constraint-aware inverse solver (SLSQP) and on an experimental optofluidic platform. The approach employs a compact loop - perceive -> compose -> propose -> act -> report & learn - that treats the objective as the interface between intent and actuation, separating what to assemble or pattern from how to actuate, while learning from user feedback. The pipeline composes geometry, spacing, and assignment/topology terms to generate robust descriptive objectives that assemble from partial traces and recover after perturbations, as well as explicit objectives for precise placement, all in an actuator-agnostic fashion. Using laser-induced thermoviscous flows as the physical actuation modality, we demonstrate natural-language-programmable, light-based microscale assembly of particle patterns in a microfluidic environment. Beyond its immediate impact on programmable microassembly, and using laser-induced optofluidic actuation as a reduced-complexity experimental platform, our work points toward self-driving, AI-assisted optical manufacturing platforms in which natural language, differentiable objectives, and laser-based actuation are coupled into a reusable digital workflow.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[embodied-agents|Embodied agents]] · [[agent-reliability|Agent reliability]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.27643v1)
