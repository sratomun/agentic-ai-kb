---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "ScreenSpot-Pro: GUI Grounding for Professional High-Resolution Computer Use"
authors: Kaixin Li, Ziyang Meng, Hongzhan Lin, Ziyang Luo et al.
url: https://arxiv.org/abs/2504.07981v1
date: 2025-04-04
citationCount: 222
influentialCitationCount: 60
velocity: 15.22
ingested: 2026-06-22
tags: [computer-use-agents, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# ScreenSpot-Pro: GUI Grounding for Professional High-Resolution Computer Use

**arXiv [2504.07981v1](https://arxiv.org/abs/2504.07981v1)** · 2025-04-04 · **222 citations** (60 influential · 15.22/mo) · Kaixin Li, Ziyang Meng, Hongzhan Lin, Ziyang Luo et al.

## Abstract
Recent advancements in Multi-modal Large Language Models (MLLMs) have led to significant progress in developing GUI agents for general tasks such as web browsing and mobile phone use. However, their application in professional domains remains under-explored. These specialized workflows introduce unique challenges for GUI perception models, including high-resolution displays, smaller target sizes, and complex environments. In this paper, we introduce ScreenSpot-Pro, a new benchmark designed to rigorously evaluate the grounding capabilities of MLLMs in high-resolution professional settings. The benchmark comprises authentic high-resolution images from a variety of professional domains with expert annotations. It spans 23 applications across five industries and three operating systems. Existing GUI grounding models perform poorly on this dataset, with the best model achieving only 18.9%. Our experiments reveal that strategically reducing the search area enhances accuracy. Based on this insight, we propose ScreenSeekeR, a visual search method that utilizes the GUI knowledge of a strong planner to guide a cascaded search, achieving state-of-the-art performance with 48.1% without any additional training. We hope that our benchmark and findings will advance the development of GUI agents for professional applications. Code, data and leaderboard can be found at https://gui-agent.github.io/grounding-leaderboard.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 2.1 GUI Grounding 2.2 Processing High Resolution Images 3 ScreenSpot-Pro: Benchmarking GUI Grounding for Professional High-Resolution Computer Use 3.1 Scope of Data Collection 3.2 Collection Method and Criteria 3.3 Quality Control Task Validity. Target Box Precision. 3.4 ScreenSpot-Pro Statistics 4 Methods 4.1 Planner-Free Methods Iterative Zooming. Iterative Narrowing. ReGround. 4.2 ScreenSeekeR: An Agentic Grounding Framework Position Inference Candidate Area Scoring Recursive Search 5 Experiments End-to-end Models. Multi-round Methods. 5.1 Results of End-to-end models Models struggle on ScreenSpot-Pro, even the specialist models. Icons targets are more difficult to ground than texts. 5.2 Results of Planner-Free methods The simplest ReGround Method achieves the best result among planner-free methods. Ablations on the crop size of ReGround. 5.3 Results of ScreenSeekeR ScreenSeekeR achieves SOTA on ScreenSpot-Pro. ScreenSeekeR generates intuitive and explainable…

**Method / approach.** Method and Criteria 3.3 Quality Control Task Validity. Target Box Precision. 3.4 ScreenSpot-Pro Statistics 4 Methods 4.1 Planner-Free Methods Iterative Zooming. Iterative Narrowing. ReGround. 4.2 ScreenSeekeR: An Agentic Grounding Framework Position Inference Candidate Area Scoring Recursive Search 5 Experiments End-to-end Models. Multi-round Methods. 5.1 Results of End-to-end models Models struggle on ScreenSpot-Pro, even the specialist models. Icons targets are more difficult to ground than texts. 5.2 Results of Planner-Free methods The simplest ReGround Method achieves the best result among planner-free methods. Ablations on the crop size of ReGround. 5.3 Results of ScreenSeekeR ScreenSeekeR achieves SOTA on ScreenSpot-Pro. ScreenSeekeR generates intuitive and explainable search traces. Ablation on key designs. 6 Conclusion A ScreenSpot-Pro-CN Chinese Instructions Pose Greater Challenges. B M…

**Results.** Experiments End-to-end Models. Multi-round Methods. 5.1 Results of End-to-end models Models struggle on ScreenSpot-Pro, even the specialist models. Icons targets are more difficult to ground than texts. 5.2 Results of Planner-Free methods The simplest ReGround Method achieves the best result among planner-free methods. Ablations on the crop size of ReGround. 5.3 Results of ScreenSeekeR ScreenSeekeR achieves SOTA on ScreenSpot-Pro. ScreenSeekeR generates intuitive and explainable search traces. Ablation on key designs. 6 Conclusion A ScreenSpot-Pro-CN Chinese Instructions Pose Greater Challenges. B More Details on the Collected Software Development and Programming. Creative Software. Computer-Aided Design (CAD) and Engineering. Scientific and Analytical. Office Software. Operation System Commons. C Prompts D Data Examples E Annotator Example ScreenSpot-Pro: GUI Gro…

**Conclusion.** Conclusion A ScreenSpot-Pro-CN Chinese Instructions Pose Greater Challenges. B More Details on the Collected Software Development and Programming. Creative Software. Computer-Aided Design (CAD) and Engineering. Scientific and Analytical. Office Software. Operation System Commons. C Prompts D Data Examples E Annotator Example ScreenSpot-Pro: GUI Grounding for Professional High-Resolution Computer Use Kaixin Li 1 Ziyang Meng 2 Hongzhan Lin 3 Ziyang Luo 3 Yuchen Tian 3 Jing Ma 3 Zhiyong Huang 1 Tat-Seng Chua 1 1 National University of Singapore 2 East China Normal University 3 Hong Kong Baptist University likaixin@u.nus.edu Abstract Recent advancements in Multi-modal Large Language Mo…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.07981v1.md` · `raw/arxiv/2504.07981v1.fulltext.md`
