---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Debate or Vote: Which Yields Better Decisions in Multi-Agent Large Language Models?"
authors: Hyeong Kyu Choi, Xiaojin Zhu, Sharon Li
url: https://arxiv.org/abs/2508.17536v2
date: 2025-08-24
citationCount: 48
influentialCitationCount: 12
velocity: 4.84
ingested: 2026-06-22
tags: [agent-reliability, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Debate or Vote: Which Yields Better Decisions in Multi-Agent Large Language Models?

**arXiv [2508.17536v2](https://arxiv.org/abs/2508.17536v2)** · 2025-08-24 · **48 citations** (12 influential · 4.84/mo) · Hyeong Kyu Choi, Xiaojin Zhu, Sharon Li

## Abstract
Multi-Agent Debate~(MAD) has emerged as a promising paradigm for improving the performance of large language models through collaborative reasoning. Despite recent advances, the key factors driving MAD's effectiveness remain unclear. In this work, we disentangle MAD into two key components--Majority Voting and inter-agent Debate--and assess their respective contributions. Through extensive experiments across seven NLP benchmarks, we find that Majority Voting alone accounts for most of the performance gains typically attributed to MAD. To explain this, we propose a theoretical framework that models debate as a stochastic process. We prove that it induces a martingale over agents' belief trajectories, implying that debate alone does not improve expected correctness. Guided by these insights, we demonstrate that targeted interventions, by biasing the belief update toward correction, can meaningfully enhance debate effectiveness. Overall, our findings suggest that while MAD has potential, simple ensembling methods remain strong and more reliable alternatives in many practical settings. Code is released in https://github.com/deeplearning-wisc/debate-or-vote.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Preliminaries Multi-Agent Debate Debate vs. Voting: Formalization. 3 Is Debate Really Necessary? A Closer Look at Debate vs. Voting 3.1 Experimental Setup Baselines. Benchmarks. 3.2 Key Observations Majority voting is surprisingly strong. 4 Theoretical Analysis Definition 1. (Agent Response Generation via DCM) Theorem 1. (Majority Voting Success Probability) Remark 1. Definition 2. (Bayesian Belief Update from Neighbor Responses) Lemma 1. (Bayesian Conjugacy in Multi-Agent Debate) Theorem 2. (Martingale Behavior of Multi-Agent Debate) Theoretical insights: Majority vote does essentially all the work. Martingale behavior is supported empirically. Generalized interpretation of the Bayesian update step. 5 How Does Theory Inform Improved Design of MAD? 5.1 Belief Update by Biasing Towards Correct Signal 5.2 Belief Update Guided by the Majority Vote 6 Extended Experiments to General Settings Consistent observations in a larger and more capable model. Heterogeneous Agents. Evaluation on open-ended text g…

**Method / approach.** methods remain strong and more reliable alternatives in many practical settings. Code is released in https://github.com/deeplearning-wisc/debate-or-vote . 1 Introduction “Out of intense complexities, intense simplicities emerge.” — W. Churchill Throughout history, humans have relied on deliberation to resolve ambiguity, challenge assumptions, and seek better answers. From courtrooms and panels to scientific collaborations, group reasoning plays a central role in decision-making. This process—where individuals reflect, revise, and converge through interaction—has long been seen as a hallmark of intelligent behavior. Inspired by this, recent work has explored whether large language models (LLMs) might similarly benefit from structured interaction. Multi-Agent Debate (MAD) has emerged as a popular framework: multiple LLM agents are prompted to discuss a shared question, each updating their answer based on the responses of their peers [ 1 , 2 , 3 , 4 , 5 , 6 ] . The hope is that…

**Results.** Experimental Setup Baselines. Benchmarks. 3.2 Key Observations Majority voting is surprisingly strong. 4 Theoretical Analysis Definition 1. (Agent Response Generation via DCM) Theorem 1. (Majority Voting Success Probability) Remark 1. Definition 2. (Bayesian Belief Update from Neighbor Responses) Lemma 1. (Bayesian Conjugacy in Multi-Agent Debate) Theorem 2. (Martingale Behavior of Multi-Agent Debate) Theoretical insights: Majority vote does essentially all the work. Martingale behavior is supported empirically. Generalized interpretation of the Bayesian update step. 5 How Does Theory Inform Improved Design of MAD? 5.1 Belief Update by Biasing Towards Correct Signal 5.2 Belief Update Guided by the Majority Vote 6 Extended Experiments to General Settings Consistent observations in a larger and more capable model. Heterogeneous Agents. Evaluation on open-ended text generation tasks.…

**Conclusion.** Conclusion Appendix A Experimental Details A.1 Hyperparameters and Resources A.2 Dataset Details B Prompt Templates B.1 MAD Templates B.2 Task Templates B.3 Persona Prompts C Special Case of Theorem 1 D Proofs D.1 Proof of Theorem 1 D.2 Proof of Lemma 1 D.3 Proof of Theorem 2 Theorem 2. (Martingale Behavior of Multi-Agent Debate) D.3.1 When does ( 1 ) in Theorem 2 Hold? Proposition 1. (Sufficient Conditions for ( 1 )) Remark 2. D.3.2 When does ( 1 ) in Theorem 2 Not hold? D.4 Collective Intelligence E Martingale Process Empirical Investigation F Proper Evaluation Matters G Closed-source LLM Evaluation H Broader Impact, Limitations and Future Works Broader Impact.…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2508.17536v2.md` · `raw/arxiv/2508.17536v2.fulltext.md`
