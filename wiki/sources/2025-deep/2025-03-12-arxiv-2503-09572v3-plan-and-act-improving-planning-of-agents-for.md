---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Plan-and-Act: Improving Planning of Agents for Long-Horizon Tasks"
authors: Lutfi Eren Erdogan, Nicholas Lee, Sehoon Kim, Suhong Moon et al.
url: https://arxiv.org/abs/2503.09572v3
date: 2025-03-12
citationCount: 162
influentialCitationCount: 16
velocity: 10.56
ingested: 2026-06-22
tags: [computer-use-agents, embodied-agents, agent-memory, agent-evaluation, arxiv, 2025, cited]
---

# Plan-and-Act: Improving Planning of Agents for Long-Horizon Tasks

**arXiv [2503.09572v3](https://arxiv.org/abs/2503.09572v3)** · 2025-03-12 · **162 citations** (16 influential · 10.56/mo) · Lutfi Eren Erdogan, Nicholas Lee, Sehoon Kim, Suhong Moon et al.

## Abstract
Large language models (LLMs) have shown remarkable advancements in enabling language agents to tackle simple tasks. However, applying them for complex, multi-step, long-horizon tasks remains a challenge. Recent work have found success by separating high-level planning from low-level execution, which enables the model to effectively balance high-level planning objectives and low-level execution details. However, generating accurate plans remains difficult since LLMs are not inherently trained for this task. To address this, we propose Plan-and-Act, a novel framework that incorporates explicit planning into LLM-based agents and introduces a scalable method to enhance plan generation through a novel synthetic data generation method. Plan-and-Act consists of a Planner model which generates structured, high-level plans to achieve user goals, and an Executor model that translates these plans into environment-specific actions. To train the Planner effectively, we introduce a synthetic data generation method that annotates ground-truth trajectories with feasible plans, augmented with diverse and extensive examples to enhance generalization. We evaluate Plan-and-Act using web navigation as a representative long-horizon planning environment, demonstrating a state-of-the-art 57.58% success rate on the WebArena-Lite benchmark as well as a text-only state-of-the-art 81.36% success rate on WebVoyager.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Language Agents as Web Agents 2.2 Synthetic Data Generation 3 System Architecture 3.1 Planner 3.2 Executor 3.3 Dynamic Replanning 3.4 Chain of Thought Reasoning 4 Synthetic Data Generation 4.1 Action Trajectory Generation 4.2 Grounded Plan Generation 4.2.1 Synthetic Data Generation for Dynamic Replanning 4.2.2 Synthetic Data Generation for Chain-of-Thought-Reasoning 4.3 Synthetic Plan Expansion 5 Results 5.1 Experimental Setup 5.2 Static Planner Results 5.3 Dynamic Replanning Results 5.3.1 Replanning Results 5.3.2 Chain of Thought Results 5.4 WebArena Results 5.5 WebVoyager Results 6 Conclusion A Appendix A.1 Planner and Executor Output Examples A.2 Replanner Examples A.2.1 Query Refinement A.2.2 Analyzing search results and Memory (aggregating results across multiple pages) A.3 Planner Prompt A.3.1 Planner System Prompt A.3.2 Planner User Message A.4 Executor Prompt A.4.1 Executor System Prompt A.5 Plan Data Annotator Prompt A.5.1 Plan Data A…

**Method / approach.** method to enhance plan generation through a novel synthetic data generation method. Plan-and-Act consists of a Planner model which generates structured, high-level plans to achieve user goals, and an Executor model that translates these plans into environment-specific actions. To train the Planner effectively, we introduce a synthetic data generation method that annotates ground-truth trajectories with feasible plans, augmented with diverse and extensive examples to enhance generalization. We evaluate Plan-and-Act using web navigation as a representative long-horizon planning environment, demonstrating a state-of-the-art 57.58% success rate on the WebArena-Lite benchmark as well as a text-only state-of-the-art 81.36% success rate on WebVoyager. Machine Learning, ICML 1 Introduction Figure 1 : An illustration of Plan-and-Act System Diagram. First, the Planner LLM processes the initial user query and generates an initial step by step plan (Section 3.1 ). This is then passed…

**Results.** Experimental Setup 5.2 Static Planner Results 5.3 Dynamic Replanning Results 5.3.1 Replanning Results 5.3.2 Chain of Thought Results 5.4 WebArena Results 5.5 WebVoyager Results 6 Conclusion A Appendix A.1 Planner and Executor Output Examples A.2 Replanner Examples A.2.1 Query Refinement A.2.2 Analyzing search results and Memory (aggregating results across multiple pages) A.3 Planner Prompt A.3.1 Planner System Prompt A.3.2 Planner User Message A.4 Executor Prompt A.4.1 Executor System Prompt A.5 Plan Data Annotator Prompt A.5.1 Plan Data Annotator System Prompt A.5.2 Plan Data Annotator User Message A.6 Synthetic Plan Generator Prompt A.6.1 Synthetic Plan Generator System Prompt A.6.2 Synthetic Plan Generator User Message A.7 Training Data Failure Classification Prompt A.7.1 Main System Prompt A.7.2 Shopping Admin (CMS) Failure Classes A.7.3 Reddit Failur…

**Conclusion.** Conclusion A Appendix A.1 Planner and Executor Output Examples A.2 Replanner Examples A.2.1 Query Refinement A.2.2 Analyzing search results and Memory (aggregating results across multiple pages) A.3 Planner Prompt A.3.1 Planner System Prompt A.3.2 Planner User Message A.4 Executor Prompt A.4.1 Executor System Prompt A.5 Plan Data Annotator Prompt A.5.1 Plan Data Annotator System Prompt A.5.2 Plan Data Annotator User Message A.6 Synthetic Plan Generator Prompt A.6.1 Synthetic Plan Generator System Prompt A.6.2 Synthetic Plan Generator User Message A.7 Training Data Failure Classification Prompt A.7.1 Main System Prompt A.7.2 Shopping Admin (CMS) Failure Classes A.7.3 Reddit Failu…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[webarena]]
- **Raw:** `raw/arxiv/2503.09572v3.md` · `raw/arxiv/2503.09572v3.fulltext.md`
