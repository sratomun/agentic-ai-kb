---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Adaptive Attacks Break Defenses Against Indirect Prompt Injection Attacks on LLM Agents"
authors: Qiusi Zhan, Richard Fang, Henil Shalin Panchal, Daniel Kang
url: https://arxiv.org/abs/2503.00061v2
date: 2025-02-27
citationCount: 86
influentialCitationCount: 6
velocity: 5.45
ingested: 2026-06-22
tags: [agent-reliability, agent-security, arxiv, 2025, cited]
---

# Adaptive Attacks Break Defenses Against Indirect Prompt Injection Attacks on LLM Agents

**arXiv [2503.00061v2](https://arxiv.org/abs/2503.00061v2)** · 2025-02-27 · **86 citations** (6 influential · 5.45/mo) · Qiusi Zhan, Richard Fang, Henil Shalin Panchal, Daniel Kang

## Abstract
Large Language Model (LLM) agents exhibit remarkable performance across diverse applications by using external tools to interact with environments. However, integrating external tools introduces security risks, such as indirect prompt injection (IPI) attacks. Despite defenses designed for IPI attacks, their robustness remains questionable due to insufficient testing against adaptive attacks. In this paper, we evaluate eight different defenses and bypass all of them using adaptive attacks, consistently achieving an attack success rate of over 50%. This reveals critical vulnerabilities in current defenses. Our research underscores the need for adaptive attack evaluation when designing defenses to ensure robustness and reliability. The code is available at https://github.com/uiuc-kang-lab/AdaptiveAttackAgent.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Preliminaries 3 Defense Techniques 3.1 Detection-based Defense 3.2 Input-level Defense 3.3 Model-level Defense 4 Adaptive Attack Techniques 5 Experiments 5.1 Experiment Settings 5.2 Experiment Results 6 Analysis 6.1 Detailed Results and Analysis 6.2 Impact on Valid Rate 6.3 Breakdown of ASRs 6.4 Cross Evaluation 7 Related Work 7.1 LLM Agent Safety 7.2 LLM Safety and Adversarial Attacks 7.3 Adaptive Attacks 8 Conclusion 9 Ethical Considerations 10 Limitations A Implementation Details B Experiments on the AgentDojo Benchmark C Full Prompts C.1 Default ReAct Agent Prompt C.2 LLM-based Detector Prompt C.3 Instructional Prevention C.4 Sandwich Prevention C.5 Paraphrasing Prompt Adaptive Attacks Break Defenses Against Indirect Prompt Injection Attacks on LLM Agents Qiusi Zhan 1 , Richard Fang 1 , Henil Shalin Panchal 2 , Daniel Kang 1 1 University of Illinois Urbana-Champaign, 2 Nirma University {qiusiz2, rrfang2, ddkang}@illinois.edu , 21bce085@nirmauni.ac.in Abstract Large Language…

**Method / approach.** methods to compromise these defenses. In the context of IPI attacks, the attacker can only manipulate the content of external sources, such as reviews or emails Zhan et al. ( 2024 ); Abdelnabi et al. ( 2023 ) . Therefore, adaptive attacks in this setting involve crafting adversarial examples in the external content to manipulate the LLM agent. This is similar to adversarial attacks in jailbreak attacks of LLMs, where the goal is to bypass models’ safety alignment and trigger harmful outputs Zou et al. ( 2023 ); Liu et al. ( 2024a ); Zhu et al. ( 2023 ) . Building on this, we leverage strong attack strategies from jailbreak settings to design adaptive attacks in the IPI context. We implement eight different defenses against IPI attacks on two types of LLM agents and design adaptive attacks to expose their vulnerabilities. Our results show that adaptive attacks consistently achieve success rates above 50% across the targeted defenses and LLM agents—exceeding the ASR before deployi…

**Results.** Experiments 5.1 Experiment Settings 5.2 Experiment Results 6 Analysis 6.1 Detailed Results and Analysis 6.2 Impact on Valid Rate 6.3 Breakdown of ASRs 6.4 Cross Evaluation 7 Related Work 7.1 LLM Agent Safety 7.2 LLM Safety and Adversarial Attacks 7.3 Adaptive Attacks 8 Conclusion 9 Ethical Considerations 10 Limitations A Implementation Details B Experiments on the AgentDojo Benchmark C Full Prompts C.1 Default ReAct Agent Prompt C.2 LLM-based Detector Prompt C.3 Instructional Prevention C.4 Sandwich Prevention C.5 Paraphrasing Prompt Adaptive Attacks Break Defenses Against Indirect Prompt Injection Attacks on LLM Agents Qiusi Zhan 1 , Richard Fang 1 , Henil Shalin Panchal 2 , Daniel Kang 1 1 University of Illinois Urbana-Champaign, 2 Nirma University {qiusiz2, rrfang2, ddkang}@illinois.edu , 21bce085@nirmauni.ac.in Abstract Large Language Model (LLM) agents exhibit…

**Conclusion.** Conclusion 9 Ethical Considerations 10 Limitations A Implementation Details B Experiments on the AgentDojo Benchmark C Full Prompts C.1 Default ReAct Agent Prompt C.2 LLM-based Detector Prompt C.3 Instructional Prevention C.4 Sandwich Prevention C.5 Paraphrasing Prompt Adaptive Attacks Break Defenses Against Indirect Prompt Injection Attacks on LLM Agents Qiusi Zhan 1 , Richard Fang 1 , Henil Shalin Panchal 2 , Daniel Kang 1 1 University of Illinois Urbana-Champaign, 2 Nirma University {qiusiz2, rrfang2, ddkang}@illinois.edu , 21bce085@nirmauni.ac.in Abstract Large Language Model (LLM) agents exhibit remarkable performance across diverse applications by using external tools to interact with environment…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]]
- **Raw:** `raw/arxiv/2503.00061v2.md` · `raw/arxiv/2503.00061v2.fulltext.md`
