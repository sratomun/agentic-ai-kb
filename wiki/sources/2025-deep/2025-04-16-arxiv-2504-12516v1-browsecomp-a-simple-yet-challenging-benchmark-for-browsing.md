---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "BrowseComp: A Simple Yet Challenging Benchmark for Browsing Agents"
authors: Jason Wei, Zhiqing Sun, Spencer Papay, Scott McKinney et al.
url: https://arxiv.org/abs/2504.12516v1
date: 2025-04-16
citationCount: 441
influentialCitationCount: 74
velocity: 31.07
ingested: 2026-06-22
tags: [coding-agents, computer-use-agents, agent-evaluation, arxiv, 2025, cited]
---

# BrowseComp: A Simple Yet Challenging Benchmark for Browsing Agents

**arXiv [2504.12516v1](https://arxiv.org/abs/2504.12516v1)** · 2025-04-16 · **441 citations** (74 influential · 31.07/mo) · Jason Wei, Zhiqing Sun, Spencer Papay, Scott McKinney et al.

## Abstract
We present BrowseComp, a simple yet challenging benchmark for measuring the ability for agents to browse the web. BrowseComp comprises 1,266 questions that require persistently navigating the internet in search of hard-to-find, entangled information. Despite the difficulty of the questions, BrowseComp is simple and easy-to-use, as predicted answers are short and easily verifiable against reference answers. BrowseComp for browsing agents can be seen as analogous to how programming competitions are an incomplete but useful benchmark for coding agents. While BrowseComp sidesteps challenges of a true user query distribution, like generating long answers or resolving ambiguity, it measures the important core capability of exercising persistence and creativity in finding information. BrowseComp can be found at https://github.com/openai/simple-evals.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Data collection and verification 2.1 BrowseComp criteria 2.2 Dataset diversity 2.3 Grading 2.4 What BrowseComp exercises 3 Human performance on BrowseComp 4 Evaluation of models 4.1 Performance of OpenAI models 4.2 Calibration Analysis 4.3 Test-time compute scaling 4.4 Aggregation strategies leveraging additional compute 4.5 Distribution of pass rates 5 Related work and discussion A Additional instruction for model prediction B Grading prompt BrowseComp: A Simple Yet Challenging Benchmark for Browsing Agents Jason Wei ∗ Zhiqing Sun 1 1 1 Equal contribution. Spencer Papay Scott McKinney Jeffrey Han Isa Fulford Hyung Won Chung Alex Tachard Passos William Fedus Amelia Glaese OpenAI Abstract We present BrowseComp, a simple yet challenging benchmark for measuring the ability for agents to browse the web. BrowseComp comprises 1,266 questions that require persistently navigating the internet in search of hard-to-find, entangled information. Despite the difficulty of the qu…

**Method / approach.** methods improve performance by 15% to 25% compared to just using a single attempt. This substantial performance improvement is somewhat expected because BrowseComp is a benchmark that is easier to verify than to find the answer, so the model should be able to tell when it gives a correct answer. Among these methods, best-of-N consistently achieved the highest accuracy, suggesting that Deep Research can often identify its correct answers. While its confidence scores are not well-calibrated in an absolute sense—as discussed earlier—they still reflect a meaningful internal signal: the model frequently “knows” when it’s right, even if it struggles to express that certainty as a calibrated probability. 0 0 0.1 0.1 0.1 0.1 0.2 0.2 0.2 0.2 0.3 0.3 0.3 0.3 0.4 0.4 0.4 0.4 0.5 0.5 0.5 0.5 0.6 0.6 0.6 0.6 0.7 0.7 0.7 0.7 0.8 0.8 0.8 0.8 0.9 0.9 0.9 0.9 1 1 1 1 0 0 5 5 5 5 10 10 10 10 15 15 15 15 20 20 20 20 79.3% Pass rates Percentage of total (%) OpenAI o1 Deep Research Figure 5: Analyzi…

**Results.** experimental model in Gemini, your AI assistant. Google blog , 2024. Guu et al. (2020) K. Guu, K. Lee, Z. Tung, P. Pasupat, and M.-W. Chang. REALM: Retrieval-augmented language model pre-training. In ICML , 2020. Joshi et al. (2017) M. Joshi, E. Choi, D. Weld, and L. Zettlemoyer. TriviaQA: A large scale distantly supervised challenge dataset for reading comprehension. In ACL , 2017. Lee et al. (2019) K. Lee, M.-W. Chang, and K. Toutanova. Latent retrieval for weakly supervised open domain question answering. In ACL , 2019. Lewis et al. (2020) P. Lewis, E. Perez, A. Piktus, F. Petroni, V. Karpukhin, N. Goyal, H. Küttler, M. Lewis, W. tau Yih, T. Rocktäschel, S. Riedel, and D. Kiela. Retrieval-augmented generation for knowledge-intensive NLP tasks. In NeurIPS , 2020. Menick et al. (2022) J. Menick, T. Miller, T. Ribeiro, L. G. Brigato, A. Bakhtin, P. Chatelain, M. Moore, J. Kramár, A. Joulin, K.…

**Conclusion.** discussion A Additional instruction for model prediction B Grading prompt BrowseComp: A Simple Yet Challenging Benchmark for Browsing Agents Jason Wei ∗ Zhiqing Sun 1 1 1 Equal contribution. Spencer Papay Scott McKinney Jeffrey Han Isa Fulford Hyung Won Chung Alex Tachard Passos William Fedus Amelia Glaese OpenAI Abstract We present BrowseComp, a simple yet challenging benchmark for measuring the ability for agents to browse the web. BrowseComp comprises 1,266 questions that require persistently navigating the internet in search of hard-to-find, entangled information. Despite the difficulty of the questions, BrowseComp is simple and easy-to-use, as predicted answers are sh…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[computer-use-agents|Computer-use agents]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[browsecomp]]
- **Raw:** `raw/arxiv/2504.12516v1.md` · `raw/arxiv/2504.12516v1.fulltext.md`
