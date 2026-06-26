---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "In-the-Flow Agentic System Optimization for Effective Planning and Tool Use"
authors: Zhuofeng Li, Haoxiang Zhang, Seungju Han, Sheng Liu et al.
url: https://arxiv.org/abs/2510.05592v1
date: 2025-10-07
citationCount: 47
influentialCitationCount: 5
velocity: 5.55
ingested: 2026-06-22
tags: [agent-reliability, agentic-rl, agent-memory, tool-use, multi-agent-systems, arxiv, 2025, cited]
---

# In-the-Flow Agentic System Optimization for Effective Planning and Tool Use

**arXiv [2510.05592v1](https://arxiv.org/abs/2510.05592v1)** · 2025-10-07 · **47 citations** (5 influential · 5.55/mo) · Zhuofeng Li, Haoxiang Zhang, Seungju Han, Sheng Liu et al.

## Abstract
Outcome-driven reinforcement learning has advanced reasoning in large language models (LLMs), but prevailing tool-augmented approaches train a single, monolithic policy that interleaves thoughts and tool calls under full context; this scales poorly with long horizons and diverse tools and generalizes weakly to new scenarios. Agentic systems offer a promising alternative by decomposing work across specialized modules, yet most remain training-free or rely on offline training decoupled from the live dynamics of multi-turn interaction. We introduce AgentFlow, a trainable, in-the-flow agentic framework that coordinates four modules (planner, executor, verifier, generator) through an evolving memory and directly optimizes its planner inside the multi-turn loop. To train on-policy in live environments, we propose Flow-based Group Refined Policy Optimization (Flow-GRPO), which tackles long-horizon, sparse-reward credit assignment by converting multi-turn optimization into a sequence of tractable single-turn policy updates. It broadcasts a single, verifiable trajectory-level outcome to every turn to align local planner decisions with global success and stabilizes learning with group-normalized advantages. Across ten benchmarks, AgentFlow with a 7B-scale backbone outperforms top-performing baselines with average accuracy gains of 14.9% on search, 14.0% on agentic, 14.5% on mathematical, and 4.1% on scientific tasks, even surpassing larger proprietary models like GPT-4o. Further analyses confirm the benefits of in-the-flow optimization, showing improved planning, enhanced tool-calling reliability, and positive scaling with model size and reasoning turns.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Preliminary Reinforcement learning for reasoning LLMs. Tool-integrated reasoning models (LLM agents). Agentic systems with tool usage. 3 In-the-Flow Agentic System Optimization 3.1 AgentFlow : An In-the-Flow Agentic System 3.2 In-the-Flow Reinforcement Learning Optimization In-the-flow learning. Policy optimization objective. Final-outcome reward. Objective function. Group-normalized advantages. 4 Experiments 4.1 Experimental Setup Implementation. Training. Evaluation. 4.2 Main Results Baselines. Key insights. 4.3 In-depth Analysis of Optimized Planning Flow-GRPO optimizes tool usage. Flow-GRPO enhances tool-calling efficacy. Flow-GRPO incentivizes autonomous discovery of new solutions. 4.4 Training Strategies on the Planner 4.5 Training Efficiency Analysis Optimized planning with increased rewards and condensed responses. Flow-GRPO efficiency over tool-integrated reasoning RL. 4.6 Scaling Trends in AgentFlow Training scaling in backbone size. Inference scaling in turn budgets.…

**Method / approach.** methods still train a single , monolithic policy under multi-turn full-context reasoning, which introduces scaling challenges: (i) training becomes increasingly unstable as horizons lengthen, tool diversity grows, and environments shift with tool feedback (Wang et al., 2025c ; Mai et al., 2025 ; Moonshot AI, 2025 ; Xue et al., 2025 ) ; and (ii) inference -time generalization remains brittle to unseen tasks or tools (Dong et al., 2025 ; Hu et al., 2025b ) . Agentic systems (Wu et al., 2024 ; Hong et al., 2024 ; Hu et al., 2025b ) offer a promising alternative to monolithic tool-integrated reasoning models. They consist of multiple modules—often distinct LLMs with prescribed roles (e.g., planner, critic) or specialized components with dedicated tools and capabilities (e.g., executor, coder)—that coordinate via shared memory and inter-module communication. By decomposing problems into sub-goals and iterating over multiple turns, these systems can tackle tasks that demand diverse to…

**Results.** Experiments 4.1 Experimental Setup Implementation. Training. Evaluation. 4.2 Main Results Baselines. Key insights. 4.3 In-depth Analysis of Optimized Planning Flow-GRPO optimizes tool usage. Flow-GRPO enhances tool-calling efficacy. Flow-GRPO incentivizes autonomous discovery of new solutions. 4.4 Training Strategies on the Planner 4.5 Training Efficiency Analysis Optimized planning with increased rewards and condensed responses. Flow-GRPO efficiency over tool-integrated reasoning RL. 4.6 Scaling Trends in AgentFlow Training scaling in backbone size. Inference scaling in turn budgets. 5 Related Work Agentic systems with tool use. 6 Conclusion A Training Algorithm of AgentFlow B Theoretical Analysis of Flow-GRPO B.1 Preliminaries and Notation B.2 Equivalence Proof for Optimization Objectives B.3 Convergence Analysis C Experimental Details C.1 Evaluation D…

**Conclusion.** Conclusion A Training Algorithm of AgentFlow B Theoretical Analysis of Flow-GRPO B.1 Preliminaries and Notation B.2 Equivalence Proof for Optimization Objectives B.3 Convergence Analysis C Experimental Details C.1 Evaluation Details C.2 Compared Baselines C.3 Evaluation Datasets D More Discussion about Experiment Results D.1 Main Result Analysis D.2 In-depth Analysis of Optimized Planning AgentFlow adapts to inference-time tool scaling. Flow-GRPO spontaneous tool usage preference change. E Instruction Templates in AgentFlow E.1 Modules and Memory E.1.1 Action Planner E.1.2 Tool Executor E.1.3 Execution Verifier E.1.4 Solution Generator E.1.5 Evolving Memory E.2 Toolset Metadata…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[grpo]] · [[gpt-5]]
- **Raw:** `raw/arxiv/2510.05592v1.md` · `raw/arxiv/2510.05592v1.fulltext.md`
