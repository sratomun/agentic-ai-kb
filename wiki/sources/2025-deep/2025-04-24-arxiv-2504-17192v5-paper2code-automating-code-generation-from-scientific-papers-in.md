---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Paper2Code: Automating Code Generation from Scientific Papers in Machine Learning"
authors: Minju Seo, Jinheon Baek, Seongyun Lee, Sung Ju Hwang
url: https://arxiv.org/abs/2504.17192v5
date: 2025-04-24
citationCount: 53
influentialCitationCount: 6
velocity: 3.81
ingested: 2026-06-22
tags: [coding-agents, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Paper2Code: Automating Code Generation from Scientific Papers in Machine Learning

**arXiv [2504.17192v5](https://arxiv.org/abs/2504.17192v5)** · 2025-04-24 · **53 citations** (6 influential · 3.81/mo) · Minju Seo, Jinheon Baek, Seongyun Lee, Sung Ju Hwang

## Abstract
Despite the rapid growth of machine learning research, corresponding code implementations are often unavailable, making it slow and labor-intensive for researchers to reproduce results and build upon prior work. In the meantime, recent Large Language Models (LLMs) excel at understanding scientific documents and generating high-quality code. Inspired by this, we introduce PaperCoder, a multi-agent LLM framework that transforms machine learning papers into operational code repositories. PaperCoder operates in three stages: planning, where it constructs a high-level roadmap, designs the system architecture with diagrams, identifies file dependencies, and generates configuration files; analysis, which focuses on interpreting implementation-specific details; and generation, where modular, dependency-aware code is produced. Moreover, each phase is instantiated through a set of specialized agents designed to collaborate effectively across the pipeline. We then evaluate PaperCoder on generating code implementations from machine learning papers based on both model-based and human evaluations, particularly from the authors of those papers, with author-released repositories as ground truth if available. Our results demonstrate the effectiveness of PaperCoder in creating high-quality, faithful implementations. Furthermore, it consistently shows strengths in the recently released PaperBench benchmark, surpassing strong baselines by substantial margins. Code is available at: https://github.com/going-doer/Paper2Code.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work Large Language Models for Code Repository-Level Coding LLM-Powered Scientific Research 3 Method 3.1 Repository-Level Code Generation from Machine Learning Papers 3.2 PaperCoder: LLM-Powered Multi-Agent Framework for Paper-to-Code 3.2.1 Planning Overall Plan Architecture Design Logic Design Configuration Generation 3.2.2 Analysis 3.2.3 Coding 4 Experiment 4.1 Experimental Setup Datasets Baselines and Our Model Evaluation Setup 4.2 Experimental Results and Analysis Main Results Correlation between Reference-Based and Reference-Free Evaluation Human Evaluation Results Results on PaperBench Code-Dev Analysis on Different LLMs Ablation Studies Experiment with Refinement Correlation on Paper Type Fine-Grained Analysis of Generated Repositories 4.3 Additional Analysis on Reproduction from Implemented Code Repository Analysis on Executability Analysis on Reproducibility Case Study 5 Conclusion References A Additional Experimental Designs A.1 Implementation Details…

**Method / approach.** Method 3.1 Repository-Level Code Generation from Machine Learning Papers 3.2 PaperCoder: LLM-Powered Multi-Agent Framework for Paper-to-Code 3.2.1 Planning Overall Plan Architecture Design Logic Design Configuration Generation 3.2.2 Analysis 3.2.3 Coding 4 Experiment 4.1 Experimental Setup Datasets Baselines and Our Model Evaluation Setup 4.2 Experimental Results and Analysis Main Results Correlation between Reference-Based and Reference-Free Evaluation Human Evaluation Results Results on PaperBench Code-Dev Analysis on Different LLMs Ablation Studies Experiment with Refinement Correlation on Paper Type Fine-Grained Analysis of Generated Repositories 4.3 Additional Analysis on Reproduction from Implemented Code Repository Analysis on Executability Analysis on Reproducibility Case Study 5 Conclusion References A Additional Experimental Designs A.1 Implementation Details A.2 Human Evaluation Process…

**Results.** Experiment 4.1 Experimental Setup Datasets Baselines and Our Model Evaluation Setup 4.2 Experimental Results and Analysis Main Results Correlation between Reference-Based and Reference-Free Evaluation Human Evaluation Results Results on PaperBench Code-Dev Analysis on Different LLMs Ablation Studies Experiment with Refinement Correlation on Paper Type Fine-Grained Analysis of Generated Repositories 4.3 Additional Analysis on Reproduction from Implemented Code Repository Analysis on Executability Analysis on Reproducibility Case Study 5 Conclusion References A Additional Experimental Designs A.1 Implementation Details A.2 Human Evaluation Process A.3 Reference-Based Evaluation A.4 PaperBench Code-Dev Evaluation A.5 Additional Details on Execution and Reproducibility Experiments B Additional Experimental Results and Analysis B.1 Code Availability B.2 Additional Ana…

**Conclusion.** Conclusion References A Additional Experimental Designs A.1 Implementation Details A.2 Human Evaluation Process A.3 Reference-Based Evaluation A.4 PaperBench Code-Dev Evaluation A.5 Additional Details on Execution and Reproducibility Experiments B Additional Experimental Results and Analysis B.1 Code Availability B.2 Additional Analysis on Executability B.3 PaperBench Code-Dev Results B.4 Impact of Paper Content on Code Generation B.5 Most Common Types of Errors and Failure Modes B.6 Addressing Environment Setup B.7 Analysis of Performance Across Paper Categories B.8 Discussion Against Data Contamination in Paper2CodeBench B.9 Cross-Family Validation for Paper2CodeBench Model Evaluation C Limitati…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.17192v5.md` · `raw/arxiv/2504.17192v5.fulltext.md`
