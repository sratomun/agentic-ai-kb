---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SPIRAL: Self-Play on Zero-Sum Games Incentivizes Reasoning via Multi-Agent Multi-Turn Reinforcement Learning"
authors: Bo Liu, Leon Guertler, Simon Yu, Zichen Liu et al.
url: https://arxiv.org/abs/2506.24119v3
date: 2025-06-30
citationCount: 65
influentialCitationCount: 4
velocity: 5.54
ingested: 2026-06-22
tags: [agent-economies, self-evolving-agents, agentic-rl, multi-agent-systems, agent-evaluation, arxiv, 2025, cited]
---

# SPIRAL: Self-Play on Zero-Sum Games Incentivizes Reasoning via Multi-Agent Multi-Turn Reinforcement Learning

**arXiv [2506.24119v3](https://arxiv.org/abs/2506.24119v3)** · 2025-06-30 · **65 citations** (4 influential · 5.54/mo) · Bo Liu, Leon Guertler, Simon Yu, Zichen Liu et al.

## Abstract
Recent advances in reinforcement learning have shown that language models can develop sophisticated reasoning through training on tasks with verifiable rewards, but these approaches depend on human-curated problem-answer pairs and domain-specific reward engineering. We introduce SPIRAL, a self-play framework where models learn by playing multi-turn, zero-sum games against continuously improving versions of themselves, generating an automatic curriculum of stronger opponents, and eliminating the need for human supervision. To enable this self-play training at scale, we implement a fully online, multi-turn, multi-agent reinforcement learning system for LLMs and propose role-conditioned advantage estimation (RAE) to stabilize multi-agent training. SPIRAL produces reasoning capabilities that transfer broadly, improving performance by up to 10% across a suite of 8 reasoning benchmarks on 4 different models spanning Qwen and Llama model families, outperforming supervised fine-tuning on 25,000 expert game trajectories. Multi-game training (TicTacToe, Kuhn Poker, Simple Negotiation) yields the strongest results, with improvements observed across both base and instruction-tuned models. Analysis of chain-of-thought traces reveals that games develop distinct cognitive patterns that transfer to improve reasoning performance, with different games developing complementary strengths. Even models which have already been trained on reasoning tasks using RLVR, like DeepSeek-R1-Distill-Qwen-7B, still benefit from our approach. These results demonstrate that zero-sum games naturally develop transferable reasoning capabilities across diverse model architectures and training stages, highlighting a promising direction for autonomous reasoning development. Our code can be found in https://github.com/spiral-rl/spiral.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 The SPIRAL Framework 4 Experimental Results 4.1 Understanding Why SPIRAL Works 5 Conclusion References A Large Language Model Usage B Limitations Reliance on Designed Game Environments Computational Cost and Scalability Evaluation and Transferability Potential for Reward Hacking C Preliminaries C.1 Turn-level Markov Decision processes (MDPs). C.2 Two-Player Zero-Sum Markov Games. C.3 Supervised Fine-Tuning (SFT) in Turn-Level MDPs C.4 Reinforcement Learning with Verifiable Rewards (RLVR) in Turn-Level MDPs D Experimental Setup Details D.1 Game Environment Observations D.2 Hyperparameter Configuration D.3 Evaluation Settings Math Benchmarks. General Reasoning Benchmarks. E Additional Results and Analysis E.1 Detailed Evolution of Case-by-Case Analysis E.2 Extended Analysis of RAE Ablation Study E.3 Game Generalization E.4 Comprehensive Benchmark Results E.5 Statistical Robustness E.6 Game Trajectory Statistics E.7 SPIRAL as part of the mid-training stage E.8 Instruct Mod…

**Method / approach.** Methodology F.1 Data Collection Framework F.2 Bottom-Up Pattern Discovery Process F.3 Cross-Domain Transfer Quantification F.4 Pattern Evolution Analysis F.5 Concrete Transfer Example Identification F.6 Pattern Classification at Scale F.7 Validation Methodology G Game Environment Specifications G.1 Training Game Environments G.2 Out-of-Distribution Evaluation Games License: CC BY 4.0 arXiv:2506.24119v3 [cs.AI] 02 Mar 2026 † † ∗ Equal contribution, order randomly decided by dice roll. † Corresponding author. SPIRAL: Self-Play on Zero-Sum Games Incentivizes Reasoning via Multi-Agent Multi-Turn Reinforcement Learning Bo Liu* 1 , Simon Yu* 2 , Zichen Liu* 1,3 , Leon Guertler* 4 Penghui Qi 1,3 , Daniel Balcells 5 , Mickel Liu 6 , Cheston Tan 4 , Weiyan Shi 2 , Min Lin 3 , Wee Sun Lee 1 Natasha Jaques †6 1 National University of Singapore 2 Northeastern University 3 Sea AI Lab 4 Centre for Frontier AI Research (CFAR), A*STAR 5 Plastic L…

**Results.** Experimental Results 4.1 Understanding Why SPIRAL Works 5 Conclusion References A Large Language Model Usage B Limitations Reliance on Designed Game Environments Computational Cost and Scalability Evaluation and Transferability Potential for Reward Hacking C Preliminaries C.1 Turn-level Markov Decision processes (MDPs). C.2 Two-Player Zero-Sum Markov Games. C.3 Supervised Fine-Tuning (SFT) in Turn-Level MDPs C.4 Reinforcement Learning with Verifiable Rewards (RLVR) in Turn-Level MDPs D Experimental Setup Details D.1 Game Environment Observations D.2 Hyperparameter Configuration D.3 Evaluation Settings Math Benchmarks. General Reasoning Benchmarks. E Additional Results and Analysis E.1 Detailed Evolution of Case-by-Case Analysis E.2 Extended Analysis of RAE Ablation Study E.3 Game Generalization E.4 Comprehensive Benchmark Results E.5 Statistical Robustness E.6 Gam…

**Conclusion.** Conclusion References A Large Language Model Usage B Limitations Reliance on Designed Game Environments Computational Cost and Scalability Evaluation and Transferability Potential for Reward Hacking C Preliminaries C.1 Turn-level Markov Decision processes (MDPs). C.2 Two-Player Zero-Sum Markov Games. C.3 Supervised Fine-Tuning (SFT) in Turn-Level MDPs C.4 Reinforcement Learning with Verifiable Rewards (RLVR) in Turn-Level MDPs D Experimental Setup Details D.1 Game Environment Observations D.2 Hyperparameter Configuration D.3 Evaluation Settings Math Benchmarks. General Reasoning Benchmarks. E Additional Results and Analysis E.1 Detailed Evolution of Case-by-Case Analysis E.2 Extende…

## Graph
- **Concepts:** [[agent-economies|Agent economies]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[qwen]] · [[deepseek]]
- **Raw:** `raw/arxiv/2506.24119v3.md` · `raw/arxiv/2506.24119v3.fulltext.md`
