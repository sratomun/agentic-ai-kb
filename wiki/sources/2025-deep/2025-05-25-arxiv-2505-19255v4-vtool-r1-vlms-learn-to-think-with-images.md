---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "VTool-R1: VLMs Learn to Think with Images via Reinforcement Learning on Multimodal Tool Use"
authors: Mingyuan Wu, Jingcheng Yang, Jize Jiang, Meitang Li et al.
url: https://arxiv.org/abs/2505.19255v4
date: 2025-05-25
citationCount: 58
influentialCitationCount: 3
velocity: 4.49
ingested: 2026-06-22
tags: [agentic-rl, tool-use, arxiv, 2025, cited]
---

# VTool-R1: VLMs Learn to Think with Images via Reinforcement Learning on Multimodal Tool Use

**arXiv [2505.19255v4](https://arxiv.org/abs/2505.19255v4)** · 2025-05-25 · **58 citations** (3 influential · 4.49/mo) · Mingyuan Wu, Jingcheng Yang, Jize Jiang, Meitang Li et al.

## Abstract
Reinforcement Learning Finetuning (RFT) has significantly advanced the reasoning capabilities of large language models (LLMs) by enabling long chains of thought, self-correction, and effective tool use. While recent works attempt to extend RFT to vision-language models (VLMs), these efforts largely produce text-only reasoning conditioned on static image inputs, falling short of true multimodal reasoning in the response. In contrast, test-time methods like Visual Sketchpad incorporate visual steps but lack training mechanisms. We introduce VTool-R1, the first framework that trains VLMs to generate multimodal chains of thought by interleaving text and intermediate visual reasoning steps. VTool-R1 integrates Python-based visual editing tools into the RFT process, enabling VLMs to learn when and how to generate visual reasoning steps that benefit final reasoning. Trained with outcome-based rewards tied to task accuracy, our approach elicits strategic visual tool use for reasoning without relying on process-based supervision. Experiments on structured visual question answering over charts and tables show that VTool-R1 enhances reasoning performance by teaching VLMs to "think with images" and generate multimodal chain of thoughts with tools. To support future research in multi-turn multi-modal reasoning, we open-source our code at https://github.com/VTOOL-R1/vtool-r1

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 2.1 Visual Chain of Thought Reasoning 2.2 LLM/VLM, Reinforcement Learning and Tool Use 3 VTool-R1 3.1 VLM Inference and Rollout with Visual Chain of Thoughts 3.2 RFT VLM to Generate Visual Chain of Thoughts 3.3 Reward Modeling 4 Experiment 4.1 Dataset 4.2 Visual Editing Toolset T 4.3 Experiment Setup 4.4 Baseline Models 4.5 Main RFT Results and Findings 5 Conclusion 6 Acknowledgements References A Appendix License: CC BY 4.0 arXiv:2505.19255v4 [cs.LG] 04 Mar 2026 VTool-R1: VLMs Learn to Think with Images via Reinforcement Learning on Multimodal Tool Use Mingyuan Wu 1 , Jingcheng Yang 1∗ , Jize Jiang 1 , Meitang Li 2 , Kaizhuo Yan 1 , Hanchao Yu 3 , Minjia Zhang 1 , Chengxiang Zhai 1 , Klara Nahrstedt 1 1 University of Illinois Urbana-Champaign 2 University of Michigan Ann Arbor, 3 Independent Researcher {mw34, klara}@cs.illinois.edu Mingyuan and Jingcheng contributed equally. Abstract Reinforcement learning finetuning (RFT) has significantly advanced the reasoning capabilities of l…

**Method / approach.** methods like Visual Sketchpad incorporate visual steps but lack training mechanisms. We introduce VTool-R1 , the first RFT framework that trains VLMs to generate multimodal chains of thought by interleaving text and intermediate visual reasoning steps. VTool-R1 integrates Python-based visual editing tools into the RFT process, enabling VLMs to learn when and how to generate visual reasoning steps that enhance the final output quality. Trained with outcome-based rewards, our approach elicits strategic visual tool use for multi-modal reasoning without relying on process-based supervision. Extensive experiments on structured visual reasoning over charts and tables show that VTool-R1 enhances reasoning performance by teaching VLMs to "think with images" and generate multimodal chain of thoughts with tools. To support future research in multi-turn multi-modal reasoning, we open-source our code at https://github.com/VTOOL-R1/vtool-r1 . 1 Introduction Recent large language models (LL…

**Results.** Experiment 4.1 Dataset 4.2 Visual Editing Toolset T 4.3 Experiment Setup 4.4 Baseline Models 4.5 Main RFT Results and Findings 5 Conclusion 6 Acknowledgements References A Appendix License: CC BY 4.0 arXiv:2505.19255v4 [cs.LG] 04 Mar 2026 VTool-R1: VLMs Learn to Think with Images via Reinforcement Learning on Multimodal Tool Use Mingyuan Wu 1 , Jingcheng Yang 1∗ , Jize Jiang 1 , Meitang Li 2 , Kaizhuo Yan 1 , Hanchao Yu 3 , Minjia Zhang 1 , Chengxiang Zhai 1 , Klara Nahrstedt 1 1 University of Illinois Urbana-Champaign 2 University of Michigan Ann Arbor, 3 Independent Researcher {mw34, klara}@cs.illinois.edu Mingyuan and Jingcheng contributed equally. Abstract Reinforcement learning finetuning (RFT) has significantly advanced the reasoning capabilities of large language models (LLMs) by enabling long chains of thought, multi-turn self-correction, and effective tool use. While recent wor…

**Conclusion.** Conclusion 6 Acknowledgements References A Appendix License: CC BY 4.0 arXiv:2505.19255v4 [cs.LG] 04 Mar 2026 VTool-R1: VLMs Learn to Think with Images via Reinforcement Learning on Multimodal Tool Use Mingyuan Wu 1 , Jingcheng Yang 1∗ , Jize Jiang 1 , Meitang Li 2 , Kaizhuo Yan 1 , Hanchao Yu 3 , Minjia Zhang 1 , Chengxiang Zhai 1 , Klara Nahrstedt 1 1 University of Illinois Urbana-Champaign 2 University of Michigan Ann Arbor, 3 Independent Researcher {mw34, klara}@cs.illinois.edu Mingyuan and Jingcheng contributed equally. Abstract Reinforcement learning finetuning (RFT) has significantly advanced the reasoning capabilities of large language models (LLMs) by enabling long chains of thought, multi-turn s…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]]
- **Raw:** `raw/arxiv/2505.19255v4.md` · `raw/arxiv/2505.19255v4.fulltext.md`
