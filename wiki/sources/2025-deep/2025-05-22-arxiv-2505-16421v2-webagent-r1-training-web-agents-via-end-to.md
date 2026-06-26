---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "WebAgent-R1: Training Web Agents via End-to-End Multi-Turn Reinforcement Learning"
authors: Zhepei Wei, Wenlin Yao, Yao Liu, Weizhi Zhang et al.
url: https://arxiv.org/abs/2505.16421v2
date: 2025-05-22
citationCount: 125
influentialCitationCount: 6
velocity: 9.61
ingested: 2026-06-22
tags: [computer-use-agents, agentic-rl, agent-memory, agent-evaluation, arxiv, 2025, cited]
---

# WebAgent-R1: Training Web Agents via End-to-End Multi-Turn Reinforcement Learning

**arXiv [2505.16421v2](https://arxiv.org/abs/2505.16421v2)** · 2025-05-22 · **125 citations** (6 influential · 9.61/mo) · Zhepei Wei, Wenlin Yao, Yao Liu, Weizhi Zhang et al.

## Abstract
While reinforcement learning (RL) has demonstrated remarkable success in enhancing large language models (LLMs), it has primarily focused on single-turn tasks such as solving math problems. Training effective web agents for multi-turn interactions remains challenging due to the complexity of long-horizon decision-making across dynamic web interfaces. In this work, we present WebAgent-R1, a simple yet effective end-to-end multi-turn RL framework for training web agents. It learns directly from online interactions with web environments by asynchronously generating diverse trajectories, entirely guided by binary rewards depending on task success. Experiments on the WebArena-Lite benchmark demonstrate the effectiveness of WebAgent-R1, boosting the task success rate of Qwen-2.5-3B from 6.1% to 33.9% and Llama-3.1-8B from 8.5% to 44.8%, significantly outperforming existing state-of-the-art methods and strong proprietary models such as OpenAI o3. In-depth analyses reveal the effectiveness of the thinking-based prompting strategy and test-time scaling through increased interactions for web tasks. We further investigate different RL initialization policies by introducing two variants, namely WebAgent-R1-Zero and WebAgent-R1-CoT, which highlight the importance of the warm-up training stage (i.e., behavior cloning) and provide insights on incorporating long chain-of-thought (CoT) reasoning in web agents.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 WebAgent-R1 2.1 Problem Formulation 2.2 Behavior Cloning 2.3 End-to-End Multi-Turn Reinforcement Learning Dynamic Context Compression Multi-turn GRPO Parallel Trajectory Rollout Reward Design 3 Experiments 3.1 Experimental Setup Web Environment Dataset and Evaluation Metrics Baselines ‣ 3.1 Experimental Setup 3.2 Main Results Most LLMs still struggle with web tasks through prompting, highlighting the importance of finetuning for web agents. Reasoning models are better web agents. Reinforcement learning enables stronger performance for web agents. 3.3 Training Dynamics Reward. Trajectory Length. Number of Interactions. ‣ 3.3 Training Dynamics 3.4 Ablation Study Behavior cloning is crucial for training web agents with RL. Incorporating long-CoT data into behavior cloning leads to more performant web agents. Limited gains from RL for long-CoT SFT model. 3.5 Analysis Prompting with thinking format unleashes the potential of LLMs as web agents. Test-time scaling through increased interaction…

**Method / approach.** methods and strong proprietary models such as OpenAI o3. In-depth analyses reveal the effectiveness of the thinking-based prompting strategy and test-time scaling through increased interactions for web tasks. We further investigate different RL initialization policies by introducing two variants, namely WebAgent-R1-Zero and WebAgent-R1-CoT , which highlight the importance of the warm-up training stage ( i.e. , behavior cloning) and provide insights on incorporating long chain-of-thought (CoT) reasoning in web agents. 1 1 1 Code and artifacts are available at https://github.com/weizhepei/WebAgent-R1 WebAgent-R1 : Training Web Agents via End-to-End Multi-Turn Reinforcement Learning Zhepei Wei † * , Wenlin Yao ‡ , Yao Liu ‡ , Weizhi Zhang ‡ , Qin Lu ‡ , Liang Qiu ‡ Changlong Yu ‡ , Puyang Xu ‡ , Chao Zhang § , Bing Yin ‡ , Hyokun Yun ‡ , Lihong Li ‡ † University of Virginia ‡ Amazon § Georgia Institute of Technology zhepei.wei@virginia.edu, chaozhang@gatech.edu {…

**Results.** Experiments 3.1 Experimental Setup Web Environment Dataset and Evaluation Metrics Baselines ‣ 3.1 Experimental Setup 3.2 Main Results Most LLMs still struggle with web tasks through prompting, highlighting the importance of finetuning for web agents. Reasoning models are better web agents. Reinforcement learning enables stronger performance for web agents. 3.3 Training Dynamics Reward. Trajectory Length. Number of Interactions. ‣ 3.3 Training Dynamics 3.4 Ablation Study Behavior cloning is crucial for training web agents with RL. Incorporating long-CoT data into behavior cloning leads to more performant web agents. Limited gains from RL for long-CoT SFT model. 3.5 Analysis Prompting with thinking format unleashes the potential of LLMs as web agents. Test-time scaling through increased interactions leads to better performance on web tasks. WebAgent-R1 generalizes well to out-of-d…

**Conclusion.** Conclusion A Web Environment WebArena-Lite Action Space Rule-based Metrics B Implementation Details C Data Augmentation for Behavior Cloning with long-CoT Traces D Prompt Templates E Qualitative Examples WebAgent-R1 : Training Web Agents via End-to-End Multi-Turn Reinforcement Learning Zhepei Wei † * , Wenlin Yao ‡ , Yao Liu ‡ , Weizhi Zhang ‡ , Qin Lu ‡ , Liang Qiu ‡ Changlong Yu ‡ , Puyang Xu ‡ , Chao Zhang § , Bing Yin ‡ , Hyokun Yun ‡ , Lihong Li ‡ † University of Virginia ‡ Amazon § Georgia Institute of Technology zhepei.wei@virginia.edu, chaozhang@gatech.edu {ywenlin, yaoliuai, zhweizhi, luqn, liangqxx, changlyu puyax, alexbyin, yunhyoku, llh}@amazon.com Abstract While reinforcement learnin…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[webarena]] · [[qwen]]
- **Raw:** `raw/arxiv/2505.16421v2.md` · `raw/arxiv/2505.16421v2.fulltext.md`
