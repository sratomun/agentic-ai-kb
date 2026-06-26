---
type: source
source_type: arxiv
title: "ColPackAgent: Agent-Skill-Guided Hard-Particle Monte Carlo Workflows for Colloidal Packing"
authors: Lijie Ding, Changwoo Do
url: https://arxiv.org/abs/2605.15625v1
date: 2026-05-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [agent-reliability, agent-protocols, agent-skills, agent-evaluation, arxiv, auto-ingested]
---

# ColPackAgent: Agent-Skill-Guided Hard-Particle Monte Carlo Workflows for Colloidal Packing

**arXiv:** [2605.15625v1](https://arxiv.org/abs/2605.15625v1) · 2026-05-15 · cs.AI
**Authors:** Lijie Ding, Changwoo Do

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We introduce ColPackAgent, an agent framework that autonomously runs Monte Carlo simulations of colloidal packing through a Model Context Protocol (MCP) tool server and an agent skill, whether as a standalone agent or inside an existing agent system. By harnessing the MCP server and agent skill, ColPackAgent executes a structured workflow for colloidal packing simulations, which are central to studies of phase behavior, self-assembly, and materials design. Without dedicated simulation tools and workflow instructions, general-purpose Large Language Model (LLM) agents tend to describe such workflows rather than execute them reliably. The MCP server exposes a custom-built colpack Python package that wraps HOOMD-blue hard-particle Monte Carlo, and the skill encodes a four-stage workflow contract. ColPackAgent can carry out the workflow interactively with human feedback, autonomously from an end-to-end prompt, or as autoresearch following a provided program file. We demonstrate the system in different modes with several colloidal packing simulation examples such as cube particles in 3D, a binary system of disks and capsules in 2D, and the 2D hard-disk freezing transition using autoresearch. We also compare model performance on this workflow across a panel of LLMs with 17 stage-specific prompts. This benchmark provides a stage-level check of how reliably different models follow the setup, planning, and analysis workflow. Together, these results show that pairing a domain Python package with MCP tools and a portable agent skill provides a practical route for turning a simulation toolkit into an agent-assisted research workflow.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-protocols|Agent protocols]] · [[agent-skills|Agent skills]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.15625v1)
