---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "WOD-E2E: Waymo Open Dataset for End-to-End Driving in Challenging Long-tail Scenarios"
authors: Runsheng Xu, Hubert Lin, Wonseok Jeon, Hao Feng et al.
url: https://arxiv.org/abs/2510.26125v3
date: 2025-10-30
citationCount: 49
influentialCitationCount: 14
velocity: 6.35
ingested: 2026-06-22
tags: [autonomous-driving-agents, agent-evaluation, arxiv, 2025, cited]
---

# WOD-E2E: Waymo Open Dataset for End-to-End Driving in Challenging Long-tail Scenarios

**arXiv [2510.26125v3](https://arxiv.org/abs/2510.26125v3)** · 2025-10-30 · **49 citations** (14 influential · 6.35/mo) · Runsheng Xu, Hubert Lin, Wonseok Jeon, Hao Feng et al.

## Abstract
Vision-based end-to-end (E2E) driving has garnered significant interest in the research community due to its scalability and synergy with multimodal large language models (MLLMs). However, current E2E driving benchmarks primarily feature nominal scenarios, failing to adequately test the true potential of these systems. Furthermore, existing open-loop evaluation metrics often fall short in capturing the multi-modal nature of driving or effectively evaluating performance in long-tail scenarios. To address these gaps, we introduce the Waymo Open Dataset for End-to-End Driving (WOD-E2E). WOD-E2E contains 4,021 driving segments (approximately 12 hours), specifically curated for challenging long-tail scenarios that that are rare in daily life with an occurring frequency of less than 0.03%. Concretely, each segment in WOD-E2E includes the high-level routing information, ego states, and 360-degree camera views from 8 surrounding cameras. To evaluate the E2E driving performance on these long-tail situations, we propose a novel open-loop evaluation metric: Rater Feedback Score (RFS). Unlike conventional metrics that measure the distance between predicted way points and the logs, RFS measures how closely the predicted trajectory matches rater-annotated trajectory preference labels. We have released rater preference labels for all WOD-E2E validation set segments, while the held out test set labels have been used for the 2025 WOD-E2E Challenge. Through our work, we aim to foster state of the art research into generalizable, robust, and safe end-to-end autonomous driving agents capable of handling complex real-world situations.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 2.1 End-to-end autonomous driving research 2.2 End-to-end autonomous driving open dataset 2.2.1 nuScenes 2.2.2 NAVSIM 2.2.3 WOMD 2.2.4 CoVLA 3 WOD-E2E Dataset 3.1 Dataset Overview 3.1.1 Coordinate System 3.1.2 Camera Data 3.1.3 Routing Information 3.1.4 Ego Status 3.1.5 Labels 3.2 Quantitative Rareness Comparison 3.3 Long-tail Data Mining 3.3.1 Mining Strategy 3.3.2 Case Study 3.3.3 Data Analysis 3.4 Data Labeling 3.4.1 Critical Moment Selection 3.4.2 Trajectory Sampling 3.4.3 Trajectory Scoring 3.5 Rater Feedback Score 4 Experimental Results 4.1 Baseline Model Setup 4.2 RFS Metric Validation 4.2.1 Quantitative Validation 4.2.2 Qualitative Validation 4.3 Benchmark Models 4.4 Discussion of the Results 5 Conclusion WOD-E2E: Waymo Open Dataset for End-to-End Driving in Challenging Long-tail Scenarios Runsheng Xu , Hubert Lin 1 1 footnotemark: 1 , Wonseok Jeon , Hao Feng , Yuliang Zou , Liting Sun John Gorman , Ekaterina Tolstaya , Sarah Tang , Brandyn White…

**Method / approach.** methods already submitted and evaluated on our public leaderboard. The diversity of these top-performing methods, employing approaches such as MLLMs [ pal2025poutinevisionlanguagetrajectorypretraining , wang2025hmvlm ] , diffusion models [ liao2025diffusiondrive ] , and CNN/ViT with GRU/MLP architectures [ ParkSwinTrajectoryTR ] , further underscores the utility of the WOD-E2E dataset and its promise to drive further advances in end-to-end autonomous driving research. Our contribution can be summarized as: • We introduce WOD-E2E , a new open dataset focusing on long-tail scenarios for benchmarking end-to-end autonomous driving systems. It contains 4,021 challenging driving segments, totaling approximately 12 hours of data and representing real-world long-tail scenarios occurring with a frequency of less than 0.03% in daily driving. • We propose Rater Feedback Score (RFS), a novel and human-aligned open-loop metric. RFS is designed to better assess E2E driving performa…

**Results.** Experimental Results 4.1 Baseline Model Setup 4.2 RFS Metric Validation 4.2.1 Quantitative Validation 4.2.2 Qualitative Validation 4.3 Benchmark Models 4.4 Discussion of the Results 5 Conclusion WOD-E2E: Waymo Open Dataset for End-to-End Driving in Challenging Long-tail Scenarios Runsheng Xu , Hubert Lin 1 1 footnotemark: 1 , Wonseok Jeon , Hao Feng , Yuliang Zou , Liting Sun John Gorman , Ekaterina Tolstaya , Sarah Tang , Brandyn White , Ben Sapp Mingxing Tan , Jyh-Jing Hwang 2 2 footnotemark: 2 , Dragomir Anguelov Waymo LLC Equal contributions.Contact emails: Runsheng Xu runshengxu@waymo.com , Jyh-Jing Hwang jyhh@waymo.com . Abstract Vision-based end-to-end (E2E) driving has garnered significant interest in the research community due to its scalability and synergy with multimodal large language models (MLLMs). However, current E2E driving benchmarks primarily feature nominal scenarios, failing…

**Conclusion.** Conclusion WOD-E2E: Waymo Open Dataset for End-to-End Driving in Challenging Long-tail Scenarios Runsheng Xu , Hubert Lin 1 1 footnotemark: 1 , Wonseok Jeon , Hao Feng , Yuliang Zou , Liting Sun John Gorman , Ekaterina Tolstaya , Sarah Tang , Brandyn White , Ben Sapp Mingxing Tan , Jyh-Jing Hwang 2 2 footnotemark: 2 , Dragomir Anguelov Waymo LLC Equal contributions.Contact emails: Runsheng Xu runshengxu@waymo.com , Jyh-Jing Hwang jyhh@waymo.com . Abstract Vision-based end-to-end (E2E) driving has garnered significant interest in the research community due to its scalability and synergy with multimodal large language models (MLLMs). However, current E2E driving benchmarks primarily feature nominal scenarios, failing to ade…

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2510.26125v3.md` · `raw/arxiv/2510.26125v3.fulltext.md`
