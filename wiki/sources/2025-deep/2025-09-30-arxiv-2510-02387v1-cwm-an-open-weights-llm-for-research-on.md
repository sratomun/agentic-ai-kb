---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "CWM: An Open-Weights LLM for Research on Code Generation with World Models"
authors: FAIR CodeGen team, Jade Copet, Quentin Carbonneaux, Gal Cohen et al.
url: https://arxiv.org/abs/2510.02387v1
date: 2025-09-30
citationCount: 56
influentialCitationCount: 10
velocity: 6.43
ingested: 2026-06-22
tags: [coding-agents, agentic-ai, arxiv, 2025, cited]
---

# CWM: An Open-Weights LLM for Research on Code Generation with World Models

**arXiv [2510.02387v1](https://arxiv.org/abs/2510.02387v1)** · 2025-09-30 · **56 citations** (10 influential · 6.43/mo) · FAIR CodeGen team, Jade Copet, Quentin Carbonneaux, Gal Cohen et al.

## Abstract
We release Code World Model (CWM), a 32-billion-parameter open-weights LLM, to advance research on code generation with world models. To improve code understanding beyond what can be learned from training on static code alone, we mid-train CWM on a large amount of observation-action trajectories from Python interpreter and agentic Docker environments, and perform extensive multi-task reasoning RL in verifiable coding, math, and multi-turn software engineering environments. With CWM, we provide a strong testbed for researchers to explore the opportunities world modeling affords for improving code generation with reasoning and planning in computational environments. We present first steps of how world models can benefit agentic coding, enable step-by-step simulation of Python code execution, and show early results of how reasoning can benefit from the latter. CWM is a dense, decoder-only LLM trained with a context size of up to 131k tokens. Independent of its world modeling capabilities, CWM offers strong performance on general coding and math tasks: it reaches pass@1 scores of 65.8% on SWE-bench Verified (with test-time scaling), 68.6% on LiveCodeBench, 96.6% on Math-500, and 76.0% on AIME 2024. To support further research on code world modeling, we release model checkpoints after mid-training, SFT, and RL.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Code world model datasets 2.1 Executable repository images: building repositories at scale 2.2 Python tracing: neural code interpretation data 2.3 ForagerAgent: agentic midtraining data generation 3 Examples of code world modeling 4 CWM : architecture, pre-training, and scaling laws 4.1 Architecture and hyper-parameters 4.2 Two-stage pre-training 4.3 Scaling laws 5 Post-training: SFT, RL algorithms and environments 5.1 SFT 5.2 RL algorithm 5.3 RL environments data 5.3.1 Agentic SWE 5.3.2 Coding 5.3.3 Agentic coding 5.3.4 Mathematics 5.4 Joint RL 6 Code and infrastructure 6.1 Techniques for efficient training 6.2 RL systems 7 Experimental results 7.1 The impact of CWM data 7.2 Agentic evaluation 7.3 Execution trace prediction 7.4 Program termination prediction 7.5 Algorithmic complexity prediction 7.6 Code and mathematical reasoning 7.7 Non-reasoning evaluations 8 Transparency, Risks Limitations 8.1 Transparency on external models and data 8.2 Code World Model Preparedness Report…

**Method / approach.** methods. For the former, an LLM-backed agent, denoted as RepoAgent, was tasked with setting up the development environment of a target repository, finding test files, and ensuring that a significant number of them could run and pass. To support its efforts, we provide RepoAgent with human-readable documentation extracted from the target repository. Although this further improves RepoAgent’s success rates, human-targeted documentation can suffer from inaccuracies due to lack of verifiability and insufficient maintenance incentives. In contrast, machine-targeted instructions must remain accurate for successful builds, with platforms like GitHub immediately signaling failures. Therefore, we also developed the Activ (Act in virtual) pipeline to repurpose GitHub Actions CI execution for building executable repository images. This pipeline runs the workflows locally via the act (Lee, 2019 ) library. Since many GitHub Actions workflows are not designed for third-party execution and not…

**Results.** Experimental results 7.1 The impact of CWM data 7.2 Agentic evaluation 7.3 Execution trace prediction 7.4 Program termination prediction 7.5 Algorithmic complexity prediction 7.6 Code and mathematical reasoning 7.7 Non-reasoning evaluations 8 Transparency, Risks Limitations 8.1 Transparency on external models and data 8.2 Code World Model Preparedness Report 8.3 Limitations future research 9 Conclusion 10 Acknowledgments 11 CWM Examples 12 RL algorithm 13 Activ image-building pipeline 14 Hyper-parameter scaling laws 14.1 Derivation of per-token compute formula 14.2 Quasi-random search for batch size and learning rate 15 RL data decontamination 16 Mathematical expression comparison for RL 17 Prompting guide 18 Formal mathematics datamix 19 RULER evaluation 20 Agent capabilities learnt during RL training \metadata [Inference Code] github.com/facebookresearch/cwm \metadata…

**Conclusion.** Conclusion 10 Acknowledgments 11 CWM Examples 12 RL algorithm 13 Activ image-building pipeline 14 Hyper-parameter scaling laws 14.1 Derivation of per-token compute formula 14.2 Quasi-random search for batch size and learning rate 15 RL data decontamination 16 Mathematical expression comparison for RL 17 Prompting guide 18 Formal mathematics datamix 19 RULER evaluation 20 Agent capabilities learnt during RL training \metadata [Inference Code] github.com/facebookresearch/cwm \metadata [Model Weights] ai.meta.com/resources/models-and-libraries/cwm-downloads , huggingface.co/facebook/cwm , ../cwm-sft , ../cwm-pretrain CWM : An Open-Weights LLM for Research on Code Generation with World Models Meta…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]]
- **Raw:** `raw/arxiv/2510.02387v1.md` · `raw/arxiv/2510.02387v1.fulltext.md`
