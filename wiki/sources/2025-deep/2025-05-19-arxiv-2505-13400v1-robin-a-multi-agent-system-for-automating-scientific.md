---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Robin: A multi-agent system for automating scientific discovery"
authors: Ali Essam Ghareeb, Benjamin Chang, Ludovico Mitchener, Angela Yiu et al.
url: https://arxiv.org/abs/2505.13400v1
date: 2025-05-19
citationCount: 74
influentialCitationCount: 1
velocity: 5.65
ingested: 2026-06-22
tags: [clinical-agents, science-agents, multi-agent-systems, agentic-ai, arxiv, 2025, cited]
---

# Robin: A multi-agent system for automating scientific discovery

**arXiv [2505.13400v1](https://arxiv.org/abs/2505.13400v1)** · 2025-05-19 · **74 citations** (1 influential · 5.65/mo) · Ali Essam Ghareeb, Benjamin Chang, Ludovico Mitchener, Angela Yiu et al.

## Abstract
Scientific discovery is driven by the iterative process of background research, hypothesis generation, experimentation, and data analysis. Despite recent advancements in applying artificial intelligence to scientific discovery, no system has yet automated all of these stages in a single workflow. Here, we introduce Robin, the first multi-agent system capable of fully automating the key intellectual steps of the scientific process. By integrating literature search agents with data analysis agents, Robin can generate hypotheses, propose experiments, interpret experimental results, and generate updated hypotheses, achieving a semi-autonomous approach to scientific discovery. By applying this system, we were able to identify a novel treatment for dry age-related macular degeneration (dAMD), the major cause of blindness in the developed world. Robin proposed enhancing retinal pigment epithelium phagocytosis as a therapeutic strategy, and identified and validated a promising therapeutic candidate, ripasudil. Ripasudil is a clinically-used rho kinase (ROCK) inhibitor that has never previously been proposed for treating dAMD. To elucidate the mechanism of ripasudil-induced upregulation of phagocytosis, Robin then proposed and analyzed a follow-up RNA-seq experiment, which revealed upregulation of ABCA1, a critical lipid efflux pump and possible novel target. All hypotheses, experimental plans, data analyses, and data figures in the main text of this report were produced by Robin. As the first AI system to autonomously discover and validate a novel therapeutic candidate within an iterative lab-in-the-loop framework, Robin establishes a new paradigm for AI-driven scientific discovery.

## From the paper (full-text excerpts)
**Introduction.** Introduction Advances in our ability to measure, perturb, and model biological systems have resulted in rapid growth of our collective scientific knowledge [1]. Yet, complementary technologies to interpret, synthesize, and generate hypotheses from this knowledge have lagged behind [2]. Artificial intelligence (AI) systems based on large language models (LLMs) show promise for automating this knowledge synthesis process and accelerating scientific discovery. As a primary goal of biomedical research is the development of new treatments for disease, our ability to produce new therapeutics may be the ultimate beneficiary of these approaches. Drug development heavily relies on a confluence of biological, clinical, and pharmaceutical expertise, and is limited by the rate at which these experts can synthesize the scientific literature [3]. The repurposing of existing drugs for new indications presents a promising application space for LLM systems. The history of drug repurposing often shows a pattern: while insights often existed in scientific literature, only after a * Equal contribution…

**Method / approach.** method are thus automated while coordinating with scientists throughout the experimental loop. By connecting literature-based hypothesis generation with experimental data analysis in a continuous feedback system, Robin represents the first complete implementation of AI-driven scientific discovery. To demonstrate Robin’s ability to generate and refine novel therapeutic hypotheses, we attempted to identify potential new treatments for dry age-related macular degeneration (dAMD). dAMD is the leading cause of irreversible sight loss in developed countries, yet limited treatment options are available. In the U.S. alone, 1.5 million people have vision-threatening dAMD, and 600,000 are legally blind due to AMD, a figure projected to almost triple by 2050 due to an aging population [29, 30]. By applying Robin to discover novel therapeutic candidates for dAMD, this work represents a first step towards AI-generated discovery in scientific research. 2 Results 2.1 Robin: A multi-agent system…

**Results.** experimentation, and data analysis. Despite recent advancements in applying artificial intelligence to scientific discovery, no system has yet automated all of these stages in a single workflow. Here, we introduce Robin, the first multi-agent system capable of fully automating the key intellectual steps of the scientific process. By integrating literature search agents with data analysis agents, Robin can generate hypotheses, propose experiments, interpret experimental results, and generate updated hypotheses, achieving a semi-autonomous approach to scientific discovery. By applying this system, we were able to identify a novel treatment for dry age-related macular degeneration (dAMD), the major cause of blindness in the developed world. Robin proposed enhancing retinal pigment epithelium phagocytosis as a therapeutic strategy, and identified and validated a promising therapeutic candidate, ripasudil. Ripasudil is a clinically-used rho…

**Conclusion.** conclusions. Similarly, Finch’s analysis results can vary between runs, even when given identical prompts and data, due to the stochasticity of the language agent. To leverage this diversity, Robin can launch 10 Finch analysis trajectories, each of which independently analyzes the experimental data. In each trajectory, Finch executes analysis code in a Jupyter notebook and provides an interpretable and reproducible summary of its findings. After all trajectories are complete, a meta-analysis can be conducted to synthesize all outputs into a consensus-driven conclusion. In this way, Finch both explores diverse analytical trajectories while delivering highly consistent end results based on consensus (Methods) [32]. Finally, Robin distills act…

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[science-agents|Science agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2505.13400v1.md` · `raw/arxiv/2505.13400v1.fulltext.md`
