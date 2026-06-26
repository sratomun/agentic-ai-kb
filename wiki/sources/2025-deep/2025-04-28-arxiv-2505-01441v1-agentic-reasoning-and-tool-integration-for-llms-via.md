---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Agentic Reasoning and Tool Integration for LLMs via Reinforcement Learning"
authors: Joykirat Singh, Raghav Magazine, Yash Pandya, Akshay Nambi
url: https://arxiv.org/abs/2505.01441v1
date: 2025-04-28
citationCount: 85
influentialCitationCount: 5
velocity: 6.16
ingested: 2026-06-22
tags: [self-evolving-agents, agentic-rl, tool-use, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Agentic Reasoning and Tool Integration for LLMs via Reinforcement Learning

**arXiv [2505.01441v1](https://arxiv.org/abs/2505.01441v1)** · 2025-04-28 · **85 citations** (5 influential · 6.16/mo) · Joykirat Singh, Raghav Magazine, Yash Pandya, Akshay Nambi

## Abstract
Large language models (LLMs) have achieved remarkable progress in complex reasoning tasks, yet they remain fundamentally limited by their reliance on static internal knowledge and text-only reasoning. Real-world problem solving often demands dynamic, multi-step reasoning, adaptive decision making, and the ability to interact with external tools and environments. In this work, we introduce ARTIST (Agentic Reasoning and Tool Integration in Self-improving Transformers), a unified framework that tightly couples agentic reasoning, reinforcement learning, and tool integration for LLMs. ARTIST enables models to autonomously decide when, how, and which tools to invoke within multi-turn reasoning chains, leveraging outcome-based RL to learn robust strategies for tool use and environment interaction without requiring step-level supervision. Extensive experiments on mathematical reasoning and multi-turn function calling benchmarks show that ARTIST consistently outperforms state-of-the-art baselines, with up to 22% absolute improvement over base models and strong gains on the most challenging tasks. Detailed studies and metric analyses reveal that agentic RL training leads to deeper reasoning, more effective tool use, and higher-quality solutions. Our results establish agentic RL with tool integration as a powerful new frontier for robust, interpretable, and generalizable problem-solving in LLMs.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 ARTIST Overview 2.1 Methodology 2.2 Reinforcement Learning Algorithm Group Relative Policy Optimization. Adapting GRPO for Agentic Reasoning with Tool Integration. 2.3 Rollouts in ARTIST Prompt Template. Rollout Process. 2.4 Reward Design Answer Reward: Format Reward: Tool Execution Reward: 3 Case Study 3.1 Complex Mathematical Reasoning with Agentic Tool Use Prompt Template Reward Design Example Analysis 3.2 Multi-Turn Function Calling with Agentic Reasoning and Tool Use Prompt Template Reward Design Example Analysis 4 Experimental Setup 4.1 Dataset and Evaluation Metrics 4.1.1 Complex Mathematical Reasoning Training Dataset Evaluation Dataset Evaluation metrics 4.1.2 Multi-Turn Function Calling Training Dataset Evaluation Datasets Evaluation Metric 4.2 Implementation Details Complex Mathematical Reasoning Multi-Turn Function Calling 4.3 Baselines 5 Results 5.1 Results: Complex Math Reasoning 5.1.1 Quantitative Results and Comparison AMC, AIME, and Olymp…

**Method / approach.** Methodology 2.2 Reinforcement Learning Algorithm Group Relative Policy Optimization. Adapting GRPO for Agentic Reasoning with Tool Integration. 2.3 Rollouts in ARTIST Prompt Template. Rollout Process. 2.4 Reward Design Answer Reward: Format Reward: Tool Execution Reward: 3 Case Study 3.1 Complex Mathematical Reasoning with Agentic Tool Use Prompt Template Reward Design Example Analysis 3.2 Multi-Turn Function Calling with Agentic Reasoning and Tool Use Prompt Template Reward Design Example Analysis 4 Experimental Setup 4.1 Dataset and Evaluation Metrics 4.1.1 Complex Mathematical Reasoning Training Dataset Evaluation Dataset Evaluation metrics 4.1.2 Multi-Turn Function Calling Training Dataset Evaluation Datasets Evaluation Metric 4.2 Implementation Details Complex Mathematical Reasoning Multi-Turn Function Calling 4.3 Baselines 5 Results 5.1 Results: Complex Math Reasoning 5.1.1 Qu…

**Results.** Experimental Setup 4.1 Dataset and Evaluation Metrics 4.1.1 Complex Mathematical Reasoning Training Dataset Evaluation Dataset Evaluation metrics 4.1.2 Multi-Turn Function Calling Training Dataset Evaluation Datasets Evaluation Metric 4.2 Implementation Details Complex Mathematical Reasoning Multi-Turn Function Calling 4.3 Baselines 5 Results 5.1 Results: Complex Math Reasoning 5.1.1 Quantitative Results and Comparison AMC, AIME, and Olympiad: Impact of Complexity MATH-500: Internal Knowledge vs. Tool Use ARTIST vs. Base LLMs + External Tools with Prompt Modifications ( Base-Prompt+Tools ) ARTIST vs. Open-Source Tool-Augmented LLMs ( Tool-OS ) ARTIST vs. Frontier LLMs ( Frontier ) 5.1.2 Metrics Reward Score (Solution Quality) Number of Tool Calls (External Tool Utilization) Response Length (Reasoning Depth) 5.2 Results: Multi-Turn Function Calling 5.2.1 Quantitat…

**Conclusion.** Conclusion A Prompt Templates in ARTIST A.1 Prompt Template for Complex Math Reasoning A.2 Prompt Template for Multi-turn Function Calling B Potential Examples of Rollouts with Agentic Reasoning C Implementation Details C.1 Complex Mathematical Reasoning Model and Training. Rollout and Tool Execution. Hardware. C.2 Multi-Turn Function Calling Model and Training. Rollout and Tool Execution. Hardware. Reproducibility. D Case Study: Complex Math Reasoning Tasks D.1 Example-1 D.2 Example-2 E Case Study: Multi-Turn Function Calling with Agentic Reasoning and Tool Use E.1 Example-1 E.2 Example -2 Key Steps and Reasoning Process Emergent Agentic Capabilities E.3 Example-3- τ 𝜏 \…

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2505.01441v1.md` · `raw/arxiv/2505.01441v1.fulltext.md`
