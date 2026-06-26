---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "WebSailor: Navigating Super-human Reasoning for Web Agent"
authors: Kuan Li, Zhongwang Zhang, Huifeng Yin, Liwen Zhang et al.
url: https://arxiv.org/abs/2507.02592v1
date: 2025-07-03
citationCount: 170
influentialCitationCount: 21
velocity: 14.62
ingested: 2026-06-22
tags: [computer-use-agents, agentic-rl, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# WebSailor: Navigating Super-human Reasoning for Web Agent

**arXiv [2507.02592v1](https://arxiv.org/abs/2507.02592v1)** · 2025-07-03 · **170 citations** (21 influential · 14.62/mo) · Kuan Li, Zhongwang Zhang, Huifeng Yin, Liwen Zhang et al.

## Abstract
Transcending human cognitive limitations represents a critical frontier in LLM training. Proprietary agentic systems like DeepResearch have demonstrated superhuman capabilities on extremely complex information-seeking benchmarks such as BrowseComp, a feat previously unattainable. We posit that their success hinges on a sophisticated reasoning pattern absent in open-source models: the ability to systematically reduce extreme uncertainty when navigating vast information landscapes. Based on this insight, we introduce WebSailor, a complete post-training methodology designed to instill this crucial capability. Our approach involves generating novel, high-uncertainty tasks through structured sampling and information obfuscation, RFT cold start, and an efficient agentic RL training algorithm, Duplicating Sampling Policy Optimization (DUPO). With this integrated pipeline, WebSailor significantly outperforms all opensource agents in complex information-seeking tasks, matching proprietary agents' performance and closing the capability gap.

## From the paper (full-text excerpts)
**Introduction.** Introduction Information seeking, the fundamental human drive to resolve uncertainty, has been revolutionized by the internet (Wilson, 1999; Jurado et al., 2015). Yet, human ability to navigate this vast digital landscape is constrained by cognitive limits: finite memory, fragile attention, and an inability to pursue multiple exploratory paths in parallel. Leading proprietary agentic systems, such as Deep Research (OpenAI, 2025a), show that Large Language Model (LLM) agents can transcend these human limitations. Their superhuman performance on complex web benchmarks like BrowseComp-en/zh (Wei et al., 2025; Zhou et al., 2025) stems from sophisticated reasoning—internal or tool-mediated—that systematically reduces uncertainty (Kapoor et al., 2024; Huang et al., 2023). However, instilling these advanced reasoning capabilities in open-source agents remains an unsolved problem. As shown in Fig. 1, existing open-source LLMs and web agents exhibit near-zero accuracy on BrowseComp-en (Wu et al., 2025a; Li et al., 2025c;b; Song et al., 2025). This stark performance gap arises because current…

**Method / approach.** methodology designed to instill this crucial capability. Our approach involves generating novel, high-uncertainty tasks through structured sampling and information obfuscation, RFT cold start, and an efficient agentic RL training algorithm, Duplicating Sampling Policy Optimization (DUPO). With this integrated pipeline, WebSailor significantly outperforms all opensource agents in complex information-seeking tasks, matching proprietary agents’ performance and closing the capability gap. Figure 1: Performance on the BrowseComp-en/zh benchmarks. DeepSeek-R1-Browse is DeepSeek-R1 equipped with browsing tools via the ReAct framework, sharing the same implementation as our model, WebSailor. Doubao-Search and Grok-3 are proprietary web-based products (marked by ∗). The result for GPT-4o with browsing is taken from OpenAI’s official publication. ∗ Equal Core Contributors. Kuan Li, Zhongwang Zhang, and Huifeng Yin are project leaders. Corresponding author. {yinhuifeng.yhf, yongjiang.yj}@alib…

**Results.** Experiments 5.1 Setup Models and Benchmarks We perform RFT and RL training on Qwen-2.5-3B, Qwen-2.5-7B, Qwen-2.532B, Qwen-2.5-72B. We mainly evaluate our method on four challenging benchmarks: • BrowseComp-en (Wei et al., 2025): one of the most challenging benchmarks introduced by OpenAI to evaluate the proficiency of AI agents in locating hard-to-find, often multi-faceted, 7 information across the internet, which demands sophisticated browsing strategies and reasoning capabilities. • BrowseComp-zh (Zhou et al., 2025): Similar to BrowseComp-en, but the QAs are in Chinese. • GAIA (Mialon et al., 2023): A benchmark that requires multi-modality and tool-use abilities. We only use a subset of 103 cases from the text-only validation subset (Li et al., 2025c; Wu et al., 2025a). • XbenchDeepSearch (Xbench-Team, 2025): A new, dynamic, professionally-aligned benchmark that focuses on evaluating AI agents’ tool usage capabilities, specifical…

**Conclusion.** Conclusion In this work, we propose WebSailor. From the perspective of uncertainty reduction in information seeking, we analyze why previous open-source web agents have not reached the level of proprietary systems. Our contributions span from QA construction, comprehensive training data synthesis, RFT cold start, to improved efficiency in RL algorithms, leading to a full agentic post-training pipeline. WebSailor demonstrates strong performance on both simple and complex information seeking benchmarks, exhibiting reasoning and tool-use capabilities that surpass human levels. We believe that the key to agentic post-training lies in further defining more complex tasks with higher uncertainty, as well as achieving more effective and efficient…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2507.02592v1.md` · `raw/arxiv/2507.02592v1.fulltext.md`
