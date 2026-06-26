---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "xbench: Tracking Agents Productivity Scaling with Profession-Aligned Real-World Evaluations"
authors: Kaiyuan Chen, Yixin Ren, Yang Liu, Xiaobo Hu et al.
url: https://arxiv.org/abs/2506.13651v1
date: 2025-06-16
citationCount: 90
influentialCitationCount: 20
velocity: 7.38
ingested: 2026-06-22
tags: [agent-skills, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# xbench: Tracking Agents Productivity Scaling with Profession-Aligned Real-World Evaluations

**arXiv [2506.13651v1](https://arxiv.org/abs/2506.13651v1)** · 2025-06-16 · **90 citations** (20 influential · 7.38/mo) · Kaiyuan Chen, Yixin Ren, Yang Liu, Xiaobo Hu et al.

## Abstract
We introduce xbench, a dynamic, profession-aligned evaluation suite designed to bridge the gap between AI agent capabilities and real-world productivity. While existing benchmarks often focus on isolated technical skills, they may not accurately reflect the economic value agents deliver in professional settings. To address this, xbench targets commercially significant domains with evaluation tasks defined by industry professionals. Our framework creates metrics that strongly correlate with productivity value, enables prediction of Technology-Market Fit (TMF), and facilitates tracking of product capabilities over time. As our initial implementations, we present two benchmarks: Recruitment and Marketing. For Recruitment, we collect 50 tasks from real-world headhunting business scenarios to evaluate agents' abilities in company mapping, information retrieval, and talent sourcing. For Marketing, we assess agents' ability to match influencers with advertiser needs, evaluating their performance across 50 advertiser requirements using a curated pool of 836 candidate influencers. We present initial evaluation results for leading contemporary agents, establishing a baseline for these professional domains. Our continuously updated evalsets and evaluations are available at https://xbench.org.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 AI Capability Centric v.s. Profession-Aligned 3 Building xbench 3.1 Live Professional Demands Define Evaluation Tasks 3.2 Benchmarking Recruitment Task Design and Examples Evaluation Process Task Distribution 3.3 Benchmarking Marketing Task Design and Examples Evaluation Process Task Distribution 4 Evalutions 4.1 Setups 4.2 Benchmarks 5 Discussion 5.1 Evaluating Lifecycling Products with xbench-Index 5.2 Evaluating Agents Tech-Market-Fit 6 Related Works 6.1 Real-world AI Evaluations 6.2 Constitution AI for Judge and Reward Models 6.3 Scaling Laws for LLMs’ Performance 7 Summary 8 Acknowledgement A Appendix A.1 Prompts for response collection and evaluation A.2 Complete Examples of the Evaluation Tasks xbench: Tracking Agents Productivity Scaling with Profession-Aligned Real-World Evaluations Core Contributors Kaiyuan Chen, Yixin Ren, Yang Liu, Xiaobo Hu, Haotong Tian, Tianbao Xie, Fangfu Liu, Haoye Zhang, Hongzhang Liu, Yuan Gong Contributors - listed alphabetically Chen Sun, Han…

**Method / approach.** methods for domain-specific agents in Recruitment and Marketing. • Evaluations of agents on xbench: We will continuously report our evaluation results of the professional capabilities of specialized agents and general-purpose agents. • Long-term updated evaluations: We will continuously update our evaluations and assess agent products, capturing the dynamic growth in agent application capabilities. 2 AI Capability Centric v.s. Profession-Aligned Figure 2: Difference between AI-capability-centric and profession-aligned benchmarks Artificial intelligence is experiencing exponential growth in the length of performable tasks. According to research by METR (METR, 2025 ) , this capability approximately doubles every seven months. However, most existing evaluations still focus on short, simulated tasks. More specifically, they are typically constructed based on specific agent capabilities that prioritize a dimension to be evaluated, such as coding, database operation…

**Results.** experiments with smaller models Kadra et al. ( 2023 ) . Further research has utilized scaling laws to predict performance on validation sets, test sets, and downstream tasks for better estimation of large model capabilities (Isik et al., 2025 ; Xu et al., 2025 ) . However, research on scaling laws that guide the evolution of agents remains relatively scarce. As mentioned in the literature, METR ( 2025 ) observe that the effective time for AI to complete a task doubles every seven months. Past growth is primarily driven by improvements in foundational model capabilities, whereas future advancements are likely to come more from the design of agent work pipelines and from agents trained end-to-end in real-world environments. This paper focuses on the evaluation of vertical agents and the tracking of their productivity value scaling. We will continuously collect evaluation results for vertical agents to observe and track the characteri…

**Conclusion.** Discussion 5.1 Evaluating Lifecycling Products with xbench-Index 5.2 Evaluating Agents Tech-Market-Fit 6 Related Works 6.1 Real-world AI Evaluations 6.2 Constitution AI for Judge and Reward Models 6.3 Scaling Laws for LLMs’ Performance 7 Summary 8 Acknowledgement A Appendix A.1 Prompts for response collection and evaluation A.2 Complete Examples of the Evaluation Tasks xbench: Tracking Agents Productivity Scaling with Profession-Aligned Real-World Evaluations Core Contributors Kaiyuan Chen, Yixin Ren, Yang Liu, Xiaobo Hu, Haotong Tian, Tianbao Xie, Fangfu Liu, Haoye Zhang, Hongzhang Liu, Yuan Gong Contributors - listed alphabetically Chen Sun, Han Hou, Hui Yang, James Pan, Jianan Lou, Jiayi Mao,…

## Graph
- **Concepts:** [[agent-skills|Agent skills]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2506.13651v1.md` · `raw/arxiv/2506.13651v1.fulltext.md`
