---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Multi-agent Architecture Search via Agentic Supernet"
authors: Guibin Zhang, Luyang Niu, Junfeng Fang, Kun Wang et al.
url: https://arxiv.org/abs/2502.04180v2
date: 2025-02-06
citationCount: 125
influentialCitationCount: 28
velocity: 7.59
ingested: 2026-06-22
tags: [tool-use, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Multi-agent Architecture Search via Agentic Supernet

**arXiv [2502.04180v2](https://arxiv.org/abs/2502.04180v2)** · 2025-02-06 · **125 citations** (28 influential · 7.59/mo) · Guibin Zhang, Luyang Niu, Junfeng Fang, Kun Wang et al.

## Abstract
Large Language Model (LLM)-empowered multi-agent systems extend the cognitive boundaries of individual agents through disciplined collaboration and interaction, while constructing these systems often requires labor-intensive manual designs. Despite the availability of methods to automate the design of agentic workflows, they typically seek to identify a static, complex, one-size-fits-all system, which, however, fails to dynamically allocate inference resources based on the difficulty and domain of each query. To address this challenge, we shift away from the pursuit of a monolithic agentic system, instead optimizing the \textbf{agentic supernet}, a probabilistic and continuous distribution of agentic architectures. We introduce MaAS, an automated framework that samples query-dependent agentic systems from the supernet, delivering high-quality solutions and tailored resource allocation (\textit{e.g.}, LLM calls, tool calls, token cost). Comprehensive evaluation across six benchmarks demonstrates that MaAS \textbf{(I)} requires only $6\sim45\%$ of the inference costs of existing handcrafted or automated multi-agent systems, \textbf{(II)} surpasses them by $0.54\%\sim11.82\%$, and \textbf{(III)} enjoys superior cross-dataset and cross-LLM-backbone transferability.

## From the paper (full-text excerpts)
**Introduction.** Introduction Large Language Model (LLM)-based agents (Richards & et al., 2023; Nakajima, 2023; Reworkd, 2023) have made remarkable strides in a spectrum of domains, such as question answering (Zhu et al., 2024a), data analysis (Hong * Equal contribution 1 National University of Singapore 2 Tongji University 3 Nanyang Technological University 4 Shanghai AI Laboratory 5 University of Science and Technology of China. Correspondence to: Kun Wang <wang.kun@ntu.edu.sg>, Lei Bai <baisanshi@gmail.com>. Although the paradigm of searching for a one-size-fitsall multi-agent system appears sufficient to optimize performance-related metrics such as accuracy and pass@k, its performance is largely constrained on resource-related Proceedings of the 42 nd International Conference on Machine Learning, Vancouver, Canada. PMLR 267, 2025. Copyright 2025 by the author(s). 1 Multi-agent Architecture Search via Agentic Supernet Building Blocks CoT Reflexion ReAct Debate I/O Web search Debate Agentic Supernet Exit Evaluator-optimizer Reflexion output Task Highschool Physics How much work i…

**Method / approach.** methods to automate the design of agentic workflows, they typically seek to identify a static, complex, onesize-fits-all system, which, however, fails to dynamically allocate inference resources based on the difficulty and domain of each query. To address this challenge, we shift away from the pursuit of a monolithic agentic system, instead optimizing the agentic supernet, a probabilistic and continuous distribution of agentic architectures. We introduce MaAS, an automated framework that samples query-dependent agentic systems from the supernet, delivering high-quality solutions and tailored resource allocation (e.g., LLM calls, tool calls, token cost). Comprehensive evaluation across six benchmarks demonstrates that MaAS (I) requires only 6 ∼ 45% of the inference costs of existing handcrafted or automated multi-agent systems, (II) surpasses them by 0.54% ∼ 16.89%, and (III) enjoys superior cross-dataset and cross-LLM-backbone transferability. The code is available at https: //github.…

**Results.** Experimental Evaluation: Extensive evaluations on six benchmarks demonstrate that our framework discovers novel agentic systems with 0.54% ∼ 16.89% higher performance, significantly lower training/inference costs, transferability across benchmarks and LLMs, and superior inductive capacity. 2 Multi-agent Architecture Search via Agentic Supernet Varied benchmark Conditioned sampling Topic: Probability Diffculty: Complicated system A board game spinner is divided into three parts labeled , and . The probability of the spinner landing on is ... feedback Task Topic: Web navigation Diffculty: According to github, when was Regression added to numpy.polynomial ... Controller executor Env I/O + ReAct Agentic Supernet Task gradient agent if-else generator Topic: File summarize Diffculty: What's the last line of rhyme on the headstone visible in the background of the photo of the oldest flavor's headstone ... Tool Textual gra…

**Conclusion.** Conclusion In this paper, we for the first time shift the paradigm of automated multi-agent system design from seeking a (possibly non-existent) single optimal system to optimizing a probabilistic, continuous distribution of agentic architectures, Ablation Study We perform an ablation study on three key components of MaAS: (1) w/o ∇O L, removing the textual gradient in Equation (12); (2) w/o Oexit , removing the 8 Multi-agent Architecture Search via Agentic Supernet termed the agentic supernet. Building on this concept, we propose MaAS, which dynamically samples multi-agent systems that deliver satisfactory performance and token efficiency for user queries across different domains and varying levels of difficulty. We believe that MaAS p…

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2502.04180v2.md` · `raw/arxiv/2502.04180v2.fulltext.md`
