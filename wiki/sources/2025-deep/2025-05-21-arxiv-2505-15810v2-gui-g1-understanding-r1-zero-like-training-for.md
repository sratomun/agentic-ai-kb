---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "GUI-G1: Understanding R1-Zero-Like Training for Visual Grounding in GUI Agents"
authors: Yuqi Zhou, Sunhao Dai, Shuai Wang, Kaiwen Zhou et al.
url: https://arxiv.org/abs/2505.15810v2
date: 2025-05-21
citationCount: 57
influentialCitationCount: 6
velocity: 4.37
ingested: 2026-06-22
tags: [coding-agents, computer-use-agents, agentic-rl, agentic-ai, arxiv, 2025, cited]
---

# GUI-G1: Understanding R1-Zero-Like Training for Visual Grounding in GUI Agents

**arXiv [2505.15810v2](https://arxiv.org/abs/2505.15810v2)** · 2025-05-21 · **57 citations** (6 influential · 4.37/mo) · Yuqi Zhou, Sunhao Dai, Shuai Wang, Kaiwen Zhou et al.

## Abstract
Recent Graphical User Interface (GUI) agents replicate the R1-Zero paradigm, coupling online Reinforcement Learning (RL) with explicit chain-of-thought reasoning prior to object grounding and thereby achieving substantial performance gains. In this paper, we first conduct extensive analysis experiments of three key components of that training pipeline: input design, output evaluation, and policy update-each revealing distinct challenges arising from blindly applying general-purpose RL without adapting to GUI grounding tasks. Input design: Current templates encourage the model to generate chain-of-thought reasoning, but longer chains unexpectedly lead to worse grounding performance. Output evaluation: Reward functions based on hit signals or box area allow models to exploit box size, leading to reward hacking and poor localization quality. Policy update: Online RL tends to overfit easy examples due to biases in length and sample difficulty, leading to under-optimization on harder cases. To address these issues, we propose three targeted solutions. First, we adopt a Fast Thinking Template that encourages direct answer generation, reducing excessive reasoning during training. Second, we incorporate a box size constraint into the reward function to mitigate reward hacking. Third, we revise the RL objective by adjusting length normalization and adding a difficulty-aware scaling factor, enabling better optimization on hard samples. Our GUI-G1-3B, trained on 17K public samples with Qwen2.5-VL-3B-Instruct, achieves 90.3% accuracy on ScreenSpot and 37.1% on ScreenSpot-Pro. This surpasses all prior models of similar size and even outperforms the larger UI-TARS-7B, establishing a new state-of-the-art in GUI agent grounding. The project repository is available at https://github.com/Yuqi-Zhou/GUI-G1.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 R1-Zero-Like Training Paradigm for GUI Grounding 3 How R1-Zero-Like Training Affects Grounding for GUI Agents? 3.1 Analysis on Template 3.2 Analysis on Reward Function 3.3 Analysis on GRPO Objective 3.4 GUI-G1: A Tailored RL Visual Grounding Model 4 Experiments 5 Related Work Grounding for GUI Agents. R1-Zero-Like Training for MLLMs. 6 Conclusion A Acknowledgements B Limitations C Analysis Experiments Settings C.1 Training Details C.2 Evaluation Metrics C.3 Difficulty-Aware Weighting Strategy D Experiments Details D.1 Training Data Composition D.2 Output Token Efficiency Analysis E Broader Impacts GUI-G1: Understanding R1-Zero-Like Training for Visual Grounding in GUI Agents Yuqi Zhou 1 , Sunhao Dai 1 , Shuai Wang 2 , Kaiwen Zhou 2 , Qinglin Jia 2 , Jun Xu 1 1 Gaoling School of Artificial Intelligence, Renmin University of China 2 Huawei Noah’s Ark Lab {yuqizhou,sunhaodai,junxu}@ruc.edu.cn , {wangshuai231,jiaqinglin2,zhoukaiwen2}@huawei.com Abstract Recent Graphical User Interface (GUI) agents…

**Method / approach.** method initially lags on easy samples due to their lower weights, but gradually outperforms the original GRPO as these examples are eventually learned. In the right plot, our method maintains a lower proportion of extreme cases on hard samples, indicating that difficulty re-weighting facilitates better learning from challenging instances. Table 2: Evaluation results on ScreenSpot after mitigating length and difficulty biases. Training Objective Mobile Desktop Web Avg. Text Icon Avg. Text Icon Avg. Text Icon Avg. Standard GRPO shao2024deepseekmath 96.5 82.4 97.8 87.6 60.7 76.3 85.0 68.4 77.3 82.3 | 𝐨 i | → Max_Tokens → subscript 𝐨 𝑖 Max_Tokens {|{\mathbf{o}}_{i}|}\rightarrow\texttt{Max\_Tokens} | bold_o start_POSTSUBSCRIPT italic_i end_POSTSUBSCRIPT | → Max_Tokens liu2025understanding 96.5 81.9 97.8 86.6 65.7 77.8 85.4 71.9 79.1 83.2 𝒥 GRPO ⁢ ( π θ ) → w p ⋅ 𝒥 GRPO ⁢ ( π θ ) → subscript 𝒥 G…

**Results.** Experiments 5 Related Work Grounding for GUI Agents. R1-Zero-Like Training for MLLMs. 6 Conclusion A Acknowledgements B Limitations C Analysis Experiments Settings C.1 Training Details C.2 Evaluation Metrics C.3 Difficulty-Aware Weighting Strategy D Experiments Details D.1 Training Data Composition D.2 Output Token Efficiency Analysis E Broader Impacts GUI-G1: Understanding R1-Zero-Like Training for Visual Grounding in GUI Agents Yuqi Zhou 1 , Sunhao Dai 1 , Shuai Wang 2 , Kaiwen Zhou 2 , Qinglin Jia 2 , Jun Xu 1 1 Gaoling School of Artificial Intelligence, Renmin University of China 2 Huawei Noah’s Ark Lab {yuqizhou,sunhaodai,junxu}@ruc.edu.cn , {wangshuai231,jiaqinglin2,zhoukaiwen2}@huawei.com Abstract Recent Graphical User Interface (GUI) agents replicate the R1-Zero paradigm, coupling online Reinforcement Learning (RL) with explicit chain-of-thought reasoning prior to object g…

**Conclusion.** Conclusion A Acknowledgements B Limitations C Analysis Experiments Settings C.1 Training Details C.2 Evaluation Metrics C.3 Difficulty-Aware Weighting Strategy D Experiments Details D.1 Training Data Composition D.2 Output Token Efficiency Analysis E Broader Impacts GUI-G1: Understanding R1-Zero-Like Training for Visual Grounding in GUI Agents Yuqi Zhou 1 , Sunhao Dai 1 , Shuai Wang 2 , Kaiwen Zhou 2 , Qinglin Jia 2 , Jun Xu 1 1 Gaoling School of Artificial Intelligence, Renmin University of China 2 Huawei Noah’s Ark Lab {yuqizhou,sunhaodai,junxu}@ruc.edu.cn , {wangshuai231,jiaqinglin2,zhoukaiwen2}@huawei.com Abstract Recent Graphical User Interface (GUI) agents replicate the R1-Zero paradigm, cou…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[computer-use-agents|Computer-use agents]] · [[agentic-rl|Agentic RL]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[qwen]]
- **Raw:** `raw/arxiv/2505.15810v2.md` · `raw/arxiv/2505.15810v2.fulltext.md`
