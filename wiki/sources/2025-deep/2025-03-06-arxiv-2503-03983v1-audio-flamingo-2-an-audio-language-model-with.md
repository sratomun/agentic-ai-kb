---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Audio Flamingo 2: An Audio-Language Model with Long-Audio Understanding and Expert Reasoning Abilities"
authors: Sreyan Ghosh, Zhifeng Kong, Sonal Kumar, S Sakshi et al.
url: https://arxiv.org/abs/2503.03983v1
date: 2025-03-06
citationCount: 144
influentialCitationCount: 15
velocity: 9.27
ingested: 2026-06-22
tags: [agent-evaluation, arxiv, 2025, cited]
---

# Audio Flamingo 2: An Audio-Language Model with Long-Audio Understanding and Expert Reasoning Abilities

**arXiv [2503.03983v1](https://arxiv.org/abs/2503.03983v1)** · 2025-03-06 · **144 citations** (15 influential · 9.27/mo) · Sreyan Ghosh, Zhifeng Kong, Sonal Kumar, S Sakshi et al.

## Abstract
Understanding and reasoning over non-speech sounds and music are crucial for both humans and AI agents to interact effectively with their environments. In this paper, we introduce Audio Flamingo 2 (AF2), an Audio-Language Model (ALM) with advanced audio understanding and reasoning capabilities. AF2 leverages (i) a custom CLAP model, (ii) synthetic Audio QA data for fine-grained audio reasoning, and (iii) a multi-stage curriculum learning strategy. AF2 achieves state-of-the-art performance with only a 3B parameter small language model, surpassing large open-source and proprietary models across over 20 benchmarks. Next, for the first time, we extend audio understanding to long audio segments (30 secs to 5 mins) and propose LongAudio, a large and novel dataset for training ALMs on long audio captioning and question-answering tasks. Fine-tuning AF2 on LongAudio leads to exceptional performance on our proposed LongAudioBench, an expert annotated benchmark for evaluating ALMs on long audio understanding capabilities. We conduct extensive ablation studies to confirm the efficacy of our approach. Project Website: https://research.nvidia.com/labs/adlr/AF2/.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Audio Flamingo 2 Architecture 3.1 AF-CLAP Audio Encoder 3.1.1 AF-CLAP Training Dataset 3.1.2 AF-CLAP Training Objective 3.2 Audio Conditioning Architecture LLM 4 Audio Flamingo 2 Training Data 4.1 AudioSkills: An Expert Audio Reasoning Dataset 4.2 LongAudio: A Long Audio Understanding Dataset 5 Audio Flamingo 2 Training Strategy 6 Experiments 6.1 Experimental Setup 6.2 Smaller but Better 6.3 Enhanced Audio Features Boost Performance 6.4 High Quality Data Boosts Reasoning Abilities 6.5 Cross-Attention Outperforms Prefix-Tuning 6.6 Effect of Scaling LLM 6.7 Effect of Training Schedules Audio Flamingo 2: An Audio-Language Model with Long-Audio Understanding and Expert Reasoning Abilities Sreyan Ghosh Zhifeng Kong Sonal Kumar S Sakshi Jaehyeon Kim Wei Ping Rafael Valle Dinesh Manocha Bryan Catanzaro Abstract Understanding and reasoning over non-speech sounds and music are crucial for both humans and AI agents to interact effectively with their environments. In this paper, we introd…

**Method / approach.** method: ( 1 ) 1 (1) ( 1 ) Data: Recent studies highlight that improving data quality can rival or even surpass the performance gains achieved by scaling compute and model size ( abdin2024phi ) . To this end, we propose AudioSkills (Section 4.1 ), a large-scale, skill-specific AQA training dataset featuring complex, reasoning-intensive questions paired with each audio. We design questions that target seven distinct skills, with the primary aim of improving fine-grained reasoning capabilities in ALMs. ( 2 ) 2 (2) ( 2 ) Audio Encoding: We propose AF-CLAP (Section 3.1 ), where we scale CLAP training to over 8M audio-caption pairs, incorporating synthetic data, and propose an improved contrastive loss for better representational quality and robustness. ( 3 ) 3 (3) ( 3 ) Training Strategy: We propose a novel 3-stage curriculum training strategy (Section 5 ) for improved performance. Additionally, for the first time, we extend audio understanding to long audios , moving beyond 30-seco…

**Results.** Experiments 6.1 Experimental Setup 6.2 Smaller but Better 6.3 Enhanced Audio Features Boost Performance 6.4 High Quality Data Boosts Reasoning Abilities 6.5 Cross-Attention Outperforms Prefix-Tuning 6.6 Effect of Scaling LLM 6.7 Effect of Training Schedules Audio Flamingo 2: An Audio-Language Model with Long-Audio Understanding and Expert Reasoning Abilities Sreyan Ghosh Zhifeng Kong Sonal Kumar S Sakshi Jaehyeon Kim Wei Ping Rafael Valle Dinesh Manocha Bryan Catanzaro Abstract Understanding and reasoning over non-speech sounds and music are crucial for both humans and AI agents to interact effectively with their environments. In this paper, we introduce Audio Flamingo 2 (AF2), an Audio-Language Model (ALM) with advanced audio understanding and reasoning capabilities. AF2 leverages (i) a custom CLAP model, (ii) synthetic Audio QA data for fine-grained audio reasoning, and (iii) a multi-stage c…

**Conclusion.** limitations . Dataset Task Previous SOTA Ours Dataset Task Previous SOTA Ours ClothoAQA unan. AQA - ACC 74.9% - Qwen2-A 86.9% +12.0% Clotho-v2 CAP - CIDEr 0.45 - Qwen2-A 0.46 +0.01 ClothoAQA non-bin AQA - ACC 49.5% - AF 52.6% +3.1% AudioCaps ZS ZS {}^{\text{ZS}} start_FLOATSUPERSCRIPT ZS end_FLOATSUPERSCRIPT CAP - CIDEr 0.46 - AF 0.58 +0.12 MusicAVQA audio AQA - ACC 72.1% - Qwen-A 72.3% +0.2% CREMA-D ZS ZS {}^{\text{ZS}} start_FLOATSUPERSCRIPT ZS end_FLOATSUPERSCRIPT CLS - ACC 26.5 % percent 26.5 26.5\% 26.5 % - AF 36.6% +10.1% NonSpeech7k CLS - ACC 83.9% - AF 84.3% +0.4% Ravdess ZS ZS {}^{\text{ZS}} start_FLOATSUPERSCRIPT ZS end_FLOATSUPERSCRIPT…

## Graph
- **Concepts:** [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2503.03983v1.md` · `raw/arxiv/2503.03983v1.fulltext.md`
