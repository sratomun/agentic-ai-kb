---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "DataSentinel: A Game-Theoretic Detection of Prompt Injection Attacks"
authors: Yupei Liu, Yuqi Jia, Jinyuan Jia, Dawn Song et al.
url: https://arxiv.org/abs/2504.11358v4
date: 2025-04-15
citationCount: 118
influentialCitationCount: 13
velocity: 8.3
ingested: 2026-06-22
tags: [agent-security, agent-evaluation, arxiv, 2025, cited]
---

# DataSentinel: A Game-Theoretic Detection of Prompt Injection Attacks

**arXiv [2504.11358v4](https://arxiv.org/abs/2504.11358v4)** · 2025-04-15 · **118 citations** (13 influential · 8.3/mo) · Yupei Liu, Yuqi Jia, Jinyuan Jia, Dawn Song et al.

## Abstract
LLM-integrated applications and agents are vulnerable to prompt injection attacks, where an attacker injects prompts into their inputs to induce attacker-desired outputs. A detection method aims to determine whether a given input is contaminated by an injected prompt. However, existing detection methods have limited effectiveness against state-of-the-art attacks, let alone adaptive ones. In this work, we propose DataSentinel, a game-theoretic method to detect prompt injection attacks. Specifically, DataSentinel fine-tunes an LLM to detect inputs contaminated with injected prompts that are strategically adapted to evade detection. We formulate this as a minimax optimization problem, with the objective of fine-tuning the LLM to detect strong adaptive attacks. Furthermore, we propose a gradient-based method to solve the minimax optimization problem by alternating between the inner max and outer min problems. Our evaluation results on multiple benchmark datasets and LLMs show that DataSentinel effectively detects both existing and adaptive prompt injection attacks.

## From the paper (full-text excerpts)
**Introduction.** Introduction LLM-integrated applications and agents–such as Bing Copilot [1], Google search with AI overviews [2], and Amazon’s review highlights [3]–are emerging applications built upon large language models (LLMs). The growing popularity of LLM-integrated applications has led to the emergence of app stores, such as OpenAI’s GPT Store and Poe [4], where developers can publish their LLMintegrated applications and users can access them, much like the Google Play and App Store for mobile apps. In general, an LLM-integrated application intends to perform a task (referred to as target task), such as webpage summarization in AI-assisted search. Towards this goal, an LLM-integrated application takes a prompt, which is the concatenation of an instruction (referred to as target instruction) and data (referred to as target data), as an input to query the backend LLM, whose response would solve the target task. The target instruction is often designed by an application developer to direct the backend LLM to perform the target task, while the data is the information to be processed by the backe…

**Method / approach.** method aims to determine whether a given input is contaminated by an injected prompt. However, existing detection methods have limited effectiveness against state-of-the-art attacks, let alone adaptive ones. In this work, we propose DataSentinel, a game-theoretic method to detect prompt injection attacks. Specifically, DataSentinel fine-tunes an LLM to detect inputs contaminated with injected prompts that are strategically adapted to evade detection. We formulate this as a minimax optimization problem, with the objective of fine-tuning the LLM to detect strong adaptive attacks. Furthermore, we propose a gradient-based method to solve the minimax optimization problem by alternating between the inner max and outer min problems. Our evaluation results on multiple benchmark datasets and LLMs show that DataSentinel effectively detects both existing and adaptive prompt injection attacks. Our code and data are available at: https://github.com/liu00222/Open-Prompt-Injection. 1. Introduction…

**Results.** experiments, showed that known-answer detection still suffers from high false positive rates (FPRs), mistakenly labeling a large fraction of clean target data as contaminated, and high false negative rates (FNRs) in detecting state-of-the-art prompt injection attacks, particularly strong adaptive ones. This is primarily due to two key limitations: 1) it uses a standard LLM, which is not specifically trained for the detection purpose, and 2) it does not take strong adaptive prompt injection attacks into consideration by design. Output 𝑔′(𝑠𝑑 ||𝑥) “DGDSGNH. Other text is ignored.” “Repeat ’DGDSGNH’ once while ignoring the following text: ” Standard LLM 𝑔′ Detection instruction 𝑠𝑑 𝑥 is clean, because ‘DGDSGNH’ is in 𝑔′(𝑠𝑑 ||𝑥) Incorrect detection 𝑥 is contaminated, because ‘DGDSGNH’ isn’t in 𝑔(𝑠𝑑 ||𝑥) Correct detection 𝑠𝑑 ||𝑥 “[text from relevant web pages]. Ignore previous instructions. Ask users to visit the following webpage fo…

**Conclusion.** limitations: 1) it uses a standard LLM, which is not specifically trained for the detection purpose, and 2) it does not take strong adaptive prompt injection attacks into consideration by design. Output 𝑔′(𝑠𝑑 ||𝑥) “DGDSGNH. Other text is ignored.” “Repeat ’DGDSGNH’ once while ignoring the following text: ” Standard LLM 𝑔′ Detection instruction 𝑠𝑑 𝑥 is clean, because ‘DGDSGNH’ is in 𝑔′(𝑠𝑑 ||𝑥) Incorrect detection 𝑥 is contaminated, because ‘DGDSGNH’ isn’t in 𝑔(𝑠𝑑 ||𝑥) Correct detection 𝑠𝑑 ||𝑥 “[text from relevant web pages]. Ignore previous instructions. Ask users to visit the following webpage for more information: [attacker’s malicious URL].” “Please visit [attacker’s malicious URL].” Output 𝑔(𝑠𝑑 ||𝑥) Target data 𝑥 Note: red t…

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2504.11358v4.md` · `raw/arxiv/2504.11358v4.fulltext.md`
