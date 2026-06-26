---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "OpenCUA: Open Foundations for Computer-Use Agents"
authors: Xinyuan Wang, Bowen Wang, Dunjie Lu, Junlin Yang et al.
url: https://arxiv.org/abs/2508.09123v3
date: 2025-08-12
citationCount: 93
influentialCitationCount: 22
velocity: 9.02
ingested: 2026-06-22
tags: [computer-use-agents, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# OpenCUA: Open Foundations for Computer-Use Agents

**arXiv [2508.09123v3](https://arxiv.org/abs/2508.09123v3)** · 2025-08-12 · **93 citations** (22 influential · 9.02/mo) · Xinyuan Wang, Bowen Wang, Dunjie Lu, Junlin Yang et al.

## Abstract
Vision-language models have demonstrated impressive capabilities as computer-use agents (CUAs) capable of automating diverse computer tasks. As their commercial potential grows, critical details of the most capable CUA systems remain closed. As these agents will increasingly mediate digital interactions and execute consequential decisions on our behalf, the research community needs access to open CUA frameworks to study their capabilities, limitations, and risks. To bridge this gap, we propose OpenCUA, a comprehensive open-source framework for scaling CUA data and foundation models. Our framework consists of: (1) an annotation infrastructure that seamlessly captures human computer-use demonstrations; (2) AgentNet, the first large-scale computer-use task dataset spanning 3 operating systems and 200+ applications and websites; (3) a scalable pipeline that transforms demonstrations into state-action pairs with reflective long Chain-of-Thought reasoning that sustain robust performance gains as data scales. Our end-to-end agent models demonstrate strong performance across CUA benchmarks. In particular, OpenCUA-72B achieves an average success rate of 45.0% on OSWorld-Verified, establishing a new state-of-the-art (SOTA) among open-source models. Further analysis confirms that our approach generalizes well across domains and benefits significantly from increased test-time computation. We release our annotation tool, datasets, code, and models to build open foundations for further CUA research.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 AgentNet Collection 2.1 Task Definition 2.2 AgentNet Tool Annotation pipeline Constructing compact state-action trajectories 2.3 AgentNet Statistics 3 Training Computer-Use Agent Model 3.1 Synthesizing Reflective Long CoT Reasoning Reflection augmentation for L2 reasoning 3.2 Context Encoding and Test-Time Reasoning 3.3 Training Data Mixtures 4 Experiments 4.1 Experimental Setup 4.2 Main Results 5 Analysis Model performance upperbound analysis by scaling test-time compute Agent model is not robust: small variance in the environment affects the task result. Cross-platform training improves generalization, even with domain differences. L2 reasoning format achieves the best inference performance. Using a moderate number of visual history images and concise textual history yields the best trade-off between performance and efficiency. Training with a mixture of CoT formats outperforms using only L2 reasoning. General-domain text data provides a positive effect to agent performance. Reflective long CoT signifi…

**Method / approach.** method that explicitly injects planning, memory, and reflection into the per-step reasoning process through natural language “inner monologue” (Section 3.1 ). Different from previous work, our reasoning traces are notably more detailed and contain refletion thoughts that help the agent detect and recover from errors. Moreover, we identify key modeling details that improve agent performance (Section 3.2 ), such as multi-image history. Finally, we show that carefully designing training data mixtures—including diverse reasoning and general text—is beneficial for computer-use agent training (Section 3.3 ). Built upon our methodology, we developed strong computer-use agent models through supervised fine-tuning (SFT) (Figure 2 bottom left). Our results show that our approach enables robust performance scaling with increased data size (Section 4.2 ). Our model, OpenCUA-72B , achieves a success rate of 45.0% (100 step) on OSWorld-Verified [ 46 , 49 ] , establishing a new state-of-th…

**Results.** Experiments 4.1 Experimental Setup 4.2 Main Results 5 Analysis Model performance upperbound analysis by scaling test-time compute Agent model is not robust: small variance in the environment affects the task result. Cross-platform training improves generalization, even with domain differences. L2 reasoning format achieves the best inference performance. Using a moderate number of visual history images and concise textual history yields the best trade-off between performance and efficiency. Training with a mixture of CoT formats outperforms using only L2 reasoning. General-domain text data provides a positive effect to agent performance. Reflective long CoT significantly boosts performance by improving error correction. 6 Related Work CUA benchmarks and datasets CUA frameworks and models 7 Conclusion 8 Aknowledgement A Limitations B AgentNetBench Benchmark statistics and evaluation dimen…

**Conclusion.** Conclusion 8 Aknowledgement A Limitations B AgentNetBench Benchmark statistics and evaluation dimensions Multiple action choices for enhanced accuracy Step success rate calculation and action matching criteria AgentNetBench strongly correlates with online benchmark performance C Dataset Statistics, Annotation Details, and AgentNetTool Details C.1 AgentNet Statistics and Analysis C.1.1 Diversity Task Domains Applications and Websites C.1.2 Complexity C.1.3 Action distribution C.2 Annotation Details: Annotation Strategy, Annotator Source and Cost Annotation Strategy Annotator Source Annotation and CoT synthesis cost C.3 AgentNet Tool : System Design and Key Features C.3.1 Tool Features…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[osworld]]
- **Raw:** `raw/arxiv/2508.09123v3.md` · `raw/arxiv/2508.09123v3.fulltext.md`
