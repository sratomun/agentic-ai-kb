---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "PhysBench: Benchmarking and Enhancing Vision-Language Models for Physical World Understanding"
authors: Wei Chow, Jiageng Mao, Boyi Li, Daniel Seita et al.
url: https://arxiv.org/abs/2501.16411v2
date: 2025-01-27
citationCount: 119
influentialCitationCount: 18
velocity: 7.09
ingested: 2026-06-22
tags: [embodied-agents, agent-evaluation, arxiv, 2025, cited]
---

# PhysBench: Benchmarking and Enhancing Vision-Language Models for Physical World Understanding

**arXiv [2501.16411v2](https://arxiv.org/abs/2501.16411v2)** · 2025-01-27 · **119 citations** (18 influential · 7.09/mo) · Wei Chow, Jiageng Mao, Boyi Li, Daniel Seita et al.

## Abstract
Understanding the physical world is a fundamental challenge in embodied AI, critical for enabling agents to perform complex tasks and operate safely in real-world environments. While Vision-Language Models (VLMs) have shown great promise in reasoning and task planning for embodied agents, their ability to comprehend physical phenomena remains extremely limited. To close this gap, we introduce PhysBench, a comprehensive benchmark designed to evaluate VLMs' physical world understanding capability across a diverse set of tasks. PhysBench contains 10,002 entries of interleaved video-image-text data, categorized into four major domains: physical object properties, physical object relationships, physical scene understanding, and physics-based dynamics, further divided into 19 subclasses and 8 distinct capability dimensions. Our extensive experiments, conducted on 75 representative VLMs, reveal that while these models excel in common-sense reasoning, they struggle with understanding the physical world -- likely due to the absence of physical knowledge in their training data and the lack of embedded physical priors. To tackle the shortfall, we introduce PhysAgent, a novel framework that combines the generalization strengths of VLMs with the specialized expertise of vision models, significantly enhancing VLMs' physical understanding across a variety of tasks, including an 18.4\% improvement on GPT-4o. Furthermore, our results demonstrate that enhancing VLMs' physical world understanding capabilities can help embodied agents such as MOKA. We believe that PhysBench and PhysAgent offer valuable insights and contribute to bridging the gap between VLMs and physical world understanding.

## From the paper (full-text excerpts)
**Method / approach.** methods designed for physical reasoning (Zheng et al., 2024b; Tung et al., 2023), PhysAgent retains the strong generalization abilities of VLMs and their capacity to solve open-ended problems, without relying on manually predefined processing logic or being limited to specific tasks. Experimental results demonstrate that PhysAgent improves GPT-4o’s zero-shot performance on PhysBench by 18.4%. Furthermore, we investigate how physical world understanding helps the deployment of embodied agents through extensive robotic manipulation experiments on MOKA (Liu et al., 2024a). Specifically, we employ two approaches: fine-tuning the VLM with PhysBench and utilizing PhysAgent for zero-shot inference across five representative manipulation tasks. The improvement in those tasks further validates that PhysBench and PhysAgent can facilitate the deployment of embodied agents like MOKA. We hope this work offers valuable insights and contributes to bridging the gap between VLMs and physical world und…

**Results.** experiments, conducted on 75 representative VLMs, reveal that while these models excel in common-sense reasoning, they struggle with understanding the physical world—likely due to the absence of physical knowledge in their training data and the lack of embedded physical priors. To tackle the shortfall, we introduce PhysAgent, a novel framework that combines the generalization strengths of VLMs with the specialized expertise of vision models, significantly enhancing VLMs’ physical understanding across a variety of tasks, including an 18.4% improvement on GPT-4o. Furthermore, our results demonstrate that enhancing VLMs’ physical world understanding capabilities can help embodied agents such as MOKA. We believe that PhysBench and PhysAgent offer valuable insights and contribute to bridging the gap between VLMs and physical world understanding. Project Page is here 1 I NTRODUCTION Understanding the physical world is a fundamental challen…

**Conclusion.** conclusions: (1) Prompting methods are unstable, and using pure language yields catastrophic results. As observed, the CoT strategy has minimal impact, while both Desp-CoT and PLR show a decline in performance. This suggests that descriptive prompts are not particularly effective for addressing the questions, implying that our dataset requires a deeper understanding of the videos or images to answer accurately. (2) ContPhy even worsens performance. In three out of four tasks, ContPhy underperforms compared to its base model, GPT-4o, due to suboptimal module invocation and limited flexibility in its logical templates, which struggle to adapt to diverse scenarios. Additionally, ContPhy relies on models like RCNN to process visual information…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]]
- **Raw:** `raw/arxiv/2501.16411v2.md` · `raw/arxiv/2501.16411v2.fulltext.md`
