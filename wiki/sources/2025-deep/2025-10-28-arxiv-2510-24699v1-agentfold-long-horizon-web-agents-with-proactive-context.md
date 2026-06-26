---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "AgentFold: Long-Horizon Web Agents with Proactive Context Management"
authors: Rui Ye, Zhongwang Zhang, Kuan Li, Huifeng Yin et al.
url: https://arxiv.org/abs/2510.24699v1
date: 2025-10-28
citationCount: 50
influentialCitationCount: 4
velocity: 6.42
ingested: 2026-06-22
tags: [computer-use-agents, agent-memory, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# AgentFold: Long-Horizon Web Agents with Proactive Context Management

**arXiv [2510.24699v1](https://arxiv.org/abs/2510.24699v1)** · 2025-10-28 · **50 citations** (4 influential · 6.42/mo) · Rui Ye, Zhongwang Zhang, Kuan Li, Huifeng Yin et al.

## Abstract
LLM-based web agents show immense promise for information seeking, yet their effectiveness on long-horizon tasks is hindered by a fundamental trade-off in context management. Prevailing ReAct-based agents suffer from context saturation as they accumulate noisy, raw histories, while methods that fixedly summarize the full history at each step risk the irreversible loss of critical details. Addressing these, we introduce AgentFold, a novel agent paradigm centered on proactive context management, inspired by the human cognitive process of retrospective consolidation. AgentFold treats its context as a dynamic cognitive workspace to be actively sculpted, rather than a passive log to be filled. At each step, it learns to execute a `folding' operation, which manages its historical trajectory at multiple scales: it can perform granular condensations to preserve vital, fine-grained details, or deep consolidations to abstract away entire multi-step sub-tasks. The results on prominent benchmarks are striking: with simple supervised fine-tuning (without continual pre-training or RL), our AgentFold-30B-A3B agent achieves 36.2% on BrowseComp and 47.3% on BrowseComp-ZH. Notably, this performance not only surpasses or matches open-source models of a dramatically larger scale, such as the DeepSeek-V3.1-671B-A37B, but also surpasses leading proprietary agents like OpenAI's o4-mini.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 3 AgentFold: Web Agent with Proactive Context Folding 3.1 Overview 3.2 AgentFold’s Context: Multi-Scale State Summaries, Latest Interaction 3.3 AgentFold’s Response: Thinking, Folding, Explanation, Action 3.4 AgentFold’s Training: Data Trajectory Collection 3.5 Discussions 4 Experiments 4.1 Results and Analysis 5 Conclusions A Appendix A.1 Case Study \useunder \ul AgentFold: Long-Horizon Web Agents with Proactive Context Management Rui Ye ∗ ( ✉ ) {}^{(\textrm{{\char 0\relax}})} , Zhongwang Zhang , Kuan Li ∗ , Huifeng Yin ∗ ( ✉ ) {}^{(\textrm{{\char 0\relax}})} Zhengwei Tao, Yida Zhao, Liangcai Su, Liwen Zhang, Zile Qiao, Xinyu Wang Pengjun Xie, Fei Huang, Siheng Chen, Jingren Zhou, Yong Jiang ( ✉ ) {}^{(\textrm{{\char 0\relax}})} Tongyi Lab , Alibaba Group Equal Core Contributors. Abstract LLM-based web agents show immense promise for information seeking, yet their effectiveness on long-horizon tasks is hindered by a fundamental trade-off in context management. Prevailing ReAct-based agents suf…

**Method / approach.** methods that fixedly summarize the full history at each step risk the irreversible loss of critical details. Addressing these, we introduce AgentFold, a novel agent paradigm centered on proactive context management, inspired by the human cognitive process of retrospective consolidation. AgentFold treats its context as a dynamic cognitive workspace to be actively sculpted, rather than a passive log to be filled. At each step, it learns to execute a ‘folding’ operation, which manages its historical trajectory at multiple scales: it can perform granular condensations to preserve vital, fine-grained details, or deep consolidations to abstract away entire multi-step sub-tasks. The results on prominent benchmarks are striking: with simple supervised fine-tuning (without continual pre-training or RL), our AgentFold-30B-A3B agent achieves 36.2% on BrowseComp and 47.3% on BrowseComp-ZH. Notably, this performance not only surpasses or matches open-source models of a dramatically larger scale, s…

**Results.** Experiments 4.1 Results and Analysis 5 Conclusions A Appendix A.1 Case Study \useunder \ul AgentFold: Long-Horizon Web Agents with Proactive Context Management Rui Ye ∗ ( ✉ ) {}^{(\textrm{{\char 0\relax}})} , Zhongwang Zhang , Kuan Li ∗ , Huifeng Yin ∗ ( ✉ ) {}^{(\textrm{{\char 0\relax}})} Zhengwei Tao, Yida Zhao, Liangcai Su, Liwen Zhang, Zile Qiao, Xinyu Wang Pengjun Xie, Fei Huang, Siheng Chen, Jingren Zhou, Yong Jiang ( ✉ ) {}^{(\textrm{{\char 0\relax}})} Tongyi Lab , Alibaba Group Equal Core Contributors. Abstract LLM-based web agents show immense promise for information seeking, yet their effectiveness on long-horizon tasks is hindered by a fundamental trade-off in context management. Prevailing ReAct-based agents suffer from context saturation as they accumulate noisy, raw histories, while methods that fixedly summarize the full history at each step risk the irreversible loss of critical d…

**Conclusion.** Conclusions A Appendix A.1 Case Study \useunder \ul AgentFold: Long-Horizon Web Agents with Proactive Context Management Rui Ye ∗ ( ✉ ) {}^{(\textrm{{\char 0\relax}})} , Zhongwang Zhang , Kuan Li ∗ , Huifeng Yin ∗ ( ✉ ) {}^{(\textrm{{\char 0\relax}})} Zhengwei Tao, Yida Zhao, Liangcai Su, Liwen Zhang, Zile Qiao, Xinyu Wang Pengjun Xie, Fei Huang, Siheng Chen, Jingren Zhou, Yong Jiang ( ✉ ) {}^{(\textrm{{\char 0\relax}})} Tongyi Lab , Alibaba Group Equal Core Contributors. Abstract LLM-based web agents show immense promise for information seeking, yet their effectiveness on long-horizon tasks is hindered by a fundamental trade-off in context management. Prevailing ReAct-based agents suffer from context satur…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[deepseek]]
- **Raw:** `raw/arxiv/2510.24699v1.md` · `raw/arxiv/2510.24699v1.fulltext.md`
