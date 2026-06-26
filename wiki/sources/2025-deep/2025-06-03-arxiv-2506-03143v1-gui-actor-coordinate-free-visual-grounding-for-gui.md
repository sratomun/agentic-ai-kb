---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "GUI-Actor: Coordinate-Free Visual Grounding for GUI Agents"
authors: Qianhui Wu, Kanzhi Cheng, Rui Yang, Chaoyun Zhang et al.
url: https://arxiv.org/abs/2506.03143v1
date: 2025-06-03
citationCount: 69
influentialCitationCount: 9
velocity: 5.47
ingested: 2026-06-22
tags: [computer-use-agents, multi-agent-systems, agent-evaluation, arxiv, 2025, cited]
---

# GUI-Actor: Coordinate-Free Visual Grounding for GUI Agents

**arXiv [2506.03143v1](https://arxiv.org/abs/2506.03143v1)** · 2025-06-03 · **69 citations** (9 influential · 5.47/mo) · Qianhui Wu, Kanzhi Cheng, Rui Yang, Chaoyun Zhang et al.

## Abstract
One of the principal challenges in building VLM-powered GUI agents is visual grounding, i.e., localizing the appropriate screen region for action execution based on both the visual content and the textual plans. Most existing work formulates this as a text-based coordinate generation task. However, these approaches suffer from several limitations: weak spatial-semantic alignment, inability to handle ambiguous supervision targets, and a mismatch between the dense nature of screen coordinates and the coarse, patch-level granularity of visual features extracted by models like Vision Transformers. In this paper, we propose GUI-Actor, a VLM-based method for coordinate-free GUI grounding. At its core, GUI-Actor introduces an attention-based action head that learns to align a dedicated <ACTOR> token with all relevant visual patch tokens, enabling the model to propose one or more action regions in a single forward pass. In line with this, we further design a grounding verifier to evaluate and select the most plausible action region from the candidates proposed for action execution. Extensive experiments show that GUI-Actor outperforms prior state-of-the-art methods on multiple GUI action grounding benchmarks, with improved generalization to unseen screen resolutions and layouts. Notably, GUI-Actor-7B even surpasses UI-TARS-72B (38.1) on ScreenSpot-Pro, achieving scores of 40.7 with Qwen2-VL and 44.6 with Qwen2.5-VL as backbones. Furthermore, by incorporating the verifier, we find that fine-tuning only the newly introduced action head (~100M parameters for 7B model) while keeping the VLM backbone frozen is sufficient to achieve performance comparable to previous state-of-the-art models, highlighting that GUI-Actor can endow the underlying VLM with effective grounding capabilities without compromising its general-purpose strengths.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work LLM/VLM-Powered GUI Agents. GUI Visual Grounding. 3 The Design of GUI-Actor ACTOR Token as a Contextual Anchor Attention-Based Action Head Spatial-Aware Multi-Patch Supervision 4 Grounding Verifier Data Training Inference 5 Experiments Implementation Details Evaluation Benchmarks Metric Baselines Main Results Robust Out-of-Distribution Generalization Improved Sample Efficiency Enabling backbone VLM grounding on GUIs without sacrificing general-purpose strengths. Boosting Performance via Grounding Verifier Ablation Study Multi-Region Prediction Without Extra Inference Cost Online Evaluation on OS-World-W 6 Conclusion A Limitations B Details on Multi-Patch Supervision C Visualization of Attention Maps from GUI-Actor D Training Datasets used for GUI-Actor E GUI Visual grounding Benchmarks F More Detailed on Grounding Verifier F.1 Data Construction F.2 Patch Selection G Improving Grounding with Verifier G.1 Enhancing Generation with Verifier Self-Aggregation G.2 Comparison…

**Method / approach.** method for coordinate-free GUI grounding. At its core, GUI-Actor introduces an attention-based action head that learns to align a dedicated ACTOR token with all relevant visual patch tokens, enabling the model to propose one or more action regions in a single forward pass. In line with this, we further design a grounding verifier to evaluate and select the most plausible action region from the candidates proposed for action execution. Extensive experiments show that GUI-Actor outperforms prior state-of-the-art methods on multiple GUI action grounding benchmarks, with improved generalization to unseen screen resolutions and layouts. Notably, GUI-Actor-7B achieves scores of 40.7 with Qwen2-VL and 44.6 with Qwen2.5-VL as backbones, outperforming UI-TARS-72B ( 38.1 ) on ScreenSpot-Pro, with significantly fewer parameters and training data. Furthermore, by incorporating the verifier, we find that fine-tuning only the newly introduced action head ( ∼ similar-to \sim ∼ 100M parameters for 7B…

**Results.** Experiments Implementation Details Evaluation Benchmarks Metric Baselines Main Results Robust Out-of-Distribution Generalization Improved Sample Efficiency Enabling backbone VLM grounding on GUIs without sacrificing general-purpose strengths. Boosting Performance via Grounding Verifier Ablation Study Multi-Region Prediction Without Extra Inference Cost Online Evaluation on OS-World-W 6 Conclusion A Limitations B Details on Multi-Patch Supervision C Visualization of Attention Maps from GUI-Actor D Training Datasets used for GUI-Actor E GUI Visual grounding Benchmarks F More Detailed on Grounding Verifier F.1 Data Construction F.2 Patch Selection G Improving Grounding with Verifier G.1 Enhancing Generation with Verifier Self-Aggregation G.2 Comparison with Baseline Using Verifier H Online Benchmark Evaluation on OSWorld GUI-Actor: Coordinate-Free Visual Grounding for GUI Agen…

**Conclusion.** Conclusion A Limitations B Details on Multi-Patch Supervision C Visualization of Attention Maps from GUI-Actor D Training Datasets used for GUI-Actor E GUI Visual grounding Benchmarks F More Detailed on Grounding Verifier F.1 Data Construction F.2 Patch Selection G Improving Grounding with Verifier G.1 Enhancing Generation with Verifier Self-Aggregation G.2 Comparison with Baseline Using Verifier H Online Benchmark Evaluation on OSWorld GUI-Actor: Coordinate-Free Visual Grounding for GUI Agents Qianhui Wu * Microsoft Kanzhi Cheng * Nanjing University Rui Yang * University of Illinois Urbana-Champaign Chaoyun Zhang Microsoft Jianwei Yang Microsoft Huiqiang Jiang Microsoft…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[qwen]]
- **Raw:** `raw/arxiv/2506.03143v1.md` · `raw/arxiv/2506.03143v1.fulltext.md`
