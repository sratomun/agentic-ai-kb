---
type: source
source_type: arxiv
title: "AgenticRecTune: Multi-Agent with Self-Evolving Skillhub for Recommendation System Optimization"
authors: Xidong Wu, Yue Zhuan, Ruoqiao Wei, Hangxin Chen et al.
url: https://arxiv.org/abs/2604.26969v2
date: 2026-04-21
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.IR
tags: [recommendation-agents, self-evolving-agents, agent-skills, multi-agent-systems, arxiv, auto-ingested]
---

# AgenticRecTune: Multi-Agent with Self-Evolving Skillhub for Recommendation System Optimization

**arXiv:** [2604.26969v2](https://arxiv.org/abs/2604.26969v2) · 2026-04-21 · cs.IR
**Authors:** Xidong Wu, Yue Zhuan, Ruoqiao Wei, Hangxin Chen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Modern large-scale recommendation systems are typically constructed as multi-stage pipelines, encompassing pre-ranking, ranking, and re-ranking phases. While traditional recommendation research typically focuses on optimizing a specific model, such as improving the pre-ranking model structure or ranking models training algorithm, system-level configurations optimization play a crucial role, which integrates the output from each model head to get the final score in each stage. Due to the complexity of the system, the configuration optimization is highly important and challenging. Any model modification requires new optimal system-level configurations. But each experimental iteration requires significant tuning effort. Furthermore, models in different stage operates within a distinct context and optimizes for different targets, requiring specialized domain expertise. In addition, optimization success depends on balancing competing multiple online metrics and alignment with shifting production development objectives. To address these challenges, we propose AgenticRecTune, an agentic framework comprising five specialized agents, Actor, Critic, Insight, Skill, and Online, designed to manage the end-to-end configuration optimization workflow. By leveraging the advanced reasoning of Large Language Models (LLMs), specifically Gemini, AgenticRecTune explore the optimal configuration spaces. The Actor Agent proposes multiple candidates and Critic Agent filters out suboptimal proposals.Then Online Agent autonomously prepares A/B tests based on the proposed configurations set from the Critic Agent and captures the subsequencet experimental results. We also introduce a self-evolving Skillhub, which utilizes a collaboration between the Insight Agent and Skill Agent to summarize the history results, extract underlying mechanics of each task in recommendation system and update skills.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-skills|Agent skills]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[gemini]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.26969v2)
