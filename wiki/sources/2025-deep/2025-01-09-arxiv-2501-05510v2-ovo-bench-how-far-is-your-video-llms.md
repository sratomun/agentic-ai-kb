---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "OVO-Bench: How Far is Your Video-LLMs from Real-World Online Video Understanding?"
authors: Yifei Li, Junbo Niu, Ziyang Miao, Chunjiang Ge et al.
url: https://arxiv.org/abs/2501.05510v2
date: 2025-01-09
citationCount: 96
influentialCitationCount: 18
velocity: 5.52
ingested: 2026-06-22
tags: [human-agent-interaction, agent-evaluation, arxiv, 2025, cited]
---

# OVO-Bench: How Far is Your Video-LLMs from Real-World Online Video Understanding?

**arXiv [2501.05510v2](https://arxiv.org/abs/2501.05510v2)** · 2025-01-09 · **96 citations** (18 influential · 5.52/mo) · Yifei Li, Junbo Niu, Ziyang Miao, Chunjiang Ge et al.

## Abstract
Temporal Awareness, the ability to reason dynamically based on the timestamp when a question is raised, is the key distinction between offline and online video LLMs. Unlike offline models, which rely on complete videos for static, post hoc analysis, online models process video streams incrementally and dynamically adapt their responses based on the timestamp at which the question is posed. Despite its significance, temporal awareness has not been adequately evaluated in existing benchmarks. To fill this gap, we present OVO-Bench (Online-VideO-Benchmark), a novel video benchmark that emphasizes the importance of timestamps for advanced online video understanding capability benchmarking. OVO-Bench evaluates the ability of video LLMs to reason and respond to events occurring at specific timestamps under three distinct scenarios: (1) Backward tracing: trace back to past events to answer the question. (2) Real-time understanding: understand and respond to events as they unfold at the current timestamp. (3) Forward active responding: delay the response until sufficient future information becomes available to answer the question accurately. OVO-Bench comprises 12 tasks, featuring 644 unique videos and approximately human-curated 2,800 fine-grained meta-annotations with precise timestamps. We combine automated generation pipelines with human curation. With these high-quality samples, we further developed an evaluation pipeline to systematically query video LLMs along the video timeline. Evaluations of nine Video-LLMs reveal that, despite advancements on traditional benchmarks, current models struggle with online video understanding, showing a significant gap compared to human agents. We hope OVO-Bench will drive progress in video LLMs and inspire future research in online video reasoning. Our benchmark and code can be accessed at https://github.com/JoeLeelyf/OVO-Bench.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 3 OVO-Bench 3.1 Online Video Understanding Mode Taxonomy 3.1.1 Backward Tracing 3.1.2 Real-Time Visual Perception 3.1.3 Forward Active Responding 3.2 Benchmark Construction 3.2.1 Video and Annotation Collection 3.2.2 Prompt Generation 3.3 Datasets Statistics 4 Experiments 4.1 Models and Evaluation Strategies 4.2 Main Results 4.3 Comparison between online Video-LLMs and offline Video-LLMs 4.4 Forward Active Responding 5 Conclusion and Future Work 6 More Details of Evaluation 6.1 Evaluation for Online Models on Forward Active Responding 6.2 Prompt Design for Offline Models on Forward Active Responding 6.3 Prompt Design for Models on Backward Tracing and Real-Time Visual Perception 7 More Details of Benchmark Construction 7.1 Human-annotated QA Generation 8 Additional Dataset Analysis 8.1 Task and Sample Distribution 8.2 Query Timestamps and Video Duration 9 Limitations 10 Licenses 11 Data Examples OVO-Bench: How Far is Your Video-LLMs from Real-World Online Video Understandin…

**Method / approach.** methods aim to identify the most representative frames. VideoStreaming [ 37 ] utilizes a small LLM to select critical video clips, while FlashVstream [ 57 ] employs a clustering method to choose representative frames for high-resolution processing. LongVU [ 41 ] leverages question embeddings to select question-related frames, thereby enhancing video understanding. Benchmarks for Video Understanding. Traditional video benchmarks, e.g., MSVD-QA [ 52 ] , MSRVTT-QA [ 52 ] , and ActivityNet-QA [ 54 ] , predominantly consist of short videos, typically ranging from 1 to 2 minutes in duration. These datasets are meticulously annotated with corresponding questions and ground truth answers. GPT-4 [ 34 ] is employed to assess the accuracy of the answers by comparing them against the provided questions and ground truth responses. However, these benchmarks primarily focus on evaluating short, static video scenes. Hence, new benchmarks designed to test causal and temporal understanding,…

**Results.** Experiments 4.1 Models and Evaluation Strategies 4.2 Main Results 4.3 Comparison between online Video-LLMs and offline Video-LLMs 4.4 Forward Active Responding 5 Conclusion and Future Work 6 More Details of Evaluation 6.1 Evaluation for Online Models on Forward Active Responding 6.2 Prompt Design for Offline Models on Forward Active Responding 6.3 Prompt Design for Models on Backward Tracing and Real-Time Visual Perception 7 More Details of Benchmark Construction 7.1 Human-annotated QA Generation 8 Additional Dataset Analysis 8.1 Task and Sample Distribution 8.2 Query Timestamps and Video Duration 9 Limitations 10 Licenses 11 Data Examples OVO-Bench: How Far is Your Video-LLMs from Real-World Online Video Understanding? Yifei Li ∗1,2† , Junbo Niu ∗1,3† , Ziyang Miao 3 , Chunjiang Ge 2 , Yuanhang Zhou 2 , Qihao He 4 , Xiaoyi Dong 1,5 🖂 , Haodong Duan 1 , Shuangrui Ding 1,5† , Rui Qi…

**Conclusion.** Conclusion and Future Work 6 More Details of Evaluation 6.1 Evaluation for Online Models on Forward Active Responding 6.2 Prompt Design for Offline Models on Forward Active Responding 6.3 Prompt Design for Models on Backward Tracing and Real-Time Visual Perception 7 More Details of Benchmark Construction 7.1 Human-annotated QA Generation 8 Additional Dataset Analysis 8.1 Task and Sample Distribution 8.2 Query Timestamps and Video Duration 9 Limitations 10 Licenses 11 Data Examples OVO-Bench: How Far is Your Video-LLMs from Real-World Online Video Understanding? Yifei Li ∗1,2† , Junbo Niu ∗1,3† , Ziyang Miao 3 , Chunjiang Ge 2 , Yuanhang Zhou 2 , Qihao He 4 , Xiaoyi Dong 1,5 🖂 , Haodong Duan 1 , Shu…

## Graph
- **Concepts:** [[human-agent-interaction|Human-agent interaction]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2501.05510v2.md` · `raw/arxiv/2501.05510v2.fulltext.md`
