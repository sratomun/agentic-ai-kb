---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Meta SecAlign: A Secure Foundation LLM Against Prompt Injection Attacks"
authors: Sizhe Chen, Arman Zharmagambetov, David Wagner, Chuan Guo
url: https://arxiv.org/abs/2507.02735v3
date: 2025-07-03
citationCount: 53
influentialCitationCount: 9
velocity: 4.56
ingested: 2026-06-22
tags: [embodied-agents, agent-security, tool-use, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Meta SecAlign: A Secure Foundation LLM Against Prompt Injection Attacks

**arXiv [2507.02735v3](https://arxiv.org/abs/2507.02735v3)** · 2025-07-03 · **53 citations** (9 influential · 4.56/mo) · Sizhe Chen, Arman Zharmagambetov, David Wagner, Chuan Guo

## Abstract
Prompt injection attacks, where untrusted data contains an injected prompt to manipulate the system, have been listed as the top security threat to LLM-integrated applications. Model-level prompt injection defenses have shown strong effectiveness, but the strongest defenses are proprietary. Open-source secure models are needed by the AI security community so that co-development of attacks and defenses through open research can drive scientific progress in mitigating prompt injection attacks. To this end, we develop Meta SecAlign, the first fully open-source LLM with built-in model-level defense that achieves commercial-grade performance and is powerful enough for complex agentic tasks. We provide complete details of our training recipe. We perform the most comprehensive evaluation to date on 9 utility benchmarks (measuring general knowledge, instruction following, and agentic workflows) and 7 security benchmarks. Results show that Meta SecAlign, despite being trained only on generic instruction-tuning samples, surprisingly confers security in unseen downstream tasks, including tool-calling and web-navigation, in addition to general instruction-following. Our best model -- Meta-SecAlign-70B -- establishes a new frontier of utility-security trade-off for open-source LLMs, and is more secure than several flagship proprietary models with prompt injection defense. Below are links for the code (https://github.com/facebookresearch/Meta_SecAlign), Meta-SecAlign-70B (https://huggingface.co/facebook/Meta-SecAlign-70B), and Meta-SecAlign-8B (https://huggingface.co/facebook/Meta-SecAlign-8B) models.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Preliminaries 2.1 LLM-integrated applications 2.2 Prompt injection attack 2.3 Prompt injection defense 3 SecAlign++: The Training Recipe for Meta SecAlign 3.1 Randomized injection position 3.2 Self-generated responses 3.3 SecAlign++ Algorithm 4 Experiments 4.1 Training Setup 4.2 Evaluation Setup 4.3 Meta-SecAlign - 70B is more secure than most commercial LLMs 4.4 SecAlign++ greatly outperforms SecAlign 4.5 Meta SecAlign allows flexible and easy control of the utility-security trade-off 4.6 Meta SecAlign has trivial utility drop to enable prompt injection security 4.7 Stronger LLMs are more vulnerable to prompt injections if left undefended 5 Discussion 5.1 Conclusion 5.2 Limitations 5.3 Future Work Meta SecAlign : A Secure Foundation LLM Against Prompt Injection Attacks Sizhe Chen 1,2,∗ , Arman Zharmagambetov 1 , David Wagner 2 , Chuan Guo 1,∗ FAIR at Meta 1 , UC Berkeley 2 , * for equal technical contributions Correspondence to sizhe.chen@berkeley.edu , chuanguo@openai.com Abstract Prompt injection at…

**Method / approach.** methods in SecAlign to inject the prompt into the data. We modify the chat template with the additional input role to separate the data, and use the original user role for instruction. We then follow Section ˜ 3 to generate the preference dataset (19157 samples) for DPO. We train Meta SecAlign for 3 epochs using DPO. In DPO, we use sigmoid activation σ \sigma and β = 0.1 \beta=0.1 as officially recommended, and learning rates of 3.2 ​ e 3.2e − 4 -4 for Meta-SecAlign - 70B and 1.6 ​ e 1.6e − 4 -4 for Meta-SecAlign - 8B . We use LoRA with hyperparameters r=32 for Meta-SecAlign - 70B and r=64 for Meta-SecAlign - 8B , lora_alpha=8 , lora_dropout=0.1 , target_modules = ["q_proj", "v_proj", "gate_proj", "down_proj", "up_proj"] in our paper, but we found that fine-tuning full parameters of the model with proper hyperparameters can achieve a similar performance. We use the torchtune [ torchtune ] library for DPO training with GPU parallelization. Training Meta-SecAlign - 70B utilizes 8 N…

**Results.** Experiments 4.1 Training Setup 4.2 Evaluation Setup 4.3 Meta-SecAlign - 70B is more secure than most commercial LLMs 4.4 SecAlign++ greatly outperforms SecAlign 4.5 Meta SecAlign allows flexible and easy control of the utility-security trade-off 4.6 Meta SecAlign has trivial utility drop to enable prompt injection security 4.7 Stronger LLMs are more vulnerable to prompt injections if left undefended 5 Discussion 5.1 Conclusion 5.2 Limitations 5.3 Future Work Meta SecAlign : A Secure Foundation LLM Against Prompt Injection Attacks Sizhe Chen 1,2,∗ , Arman Zharmagambetov 1 , David Wagner 2 , Chuan Guo 1,∗ FAIR at Meta 1 , UC Berkeley 2 , * for equal technical contributions Correspondence to sizhe.chen@berkeley.edu , chuanguo@openai.com Abstract Prompt injection attacks, where untrusted data contains an injected prompt to manipulate the system, have been listed as the top security threat to LLM-int…

**Conclusion.** Conclusion 5.2 Limitations 5.3 Future Work Meta SecAlign : A Secure Foundation LLM Against Prompt Injection Attacks Sizhe Chen 1,2,∗ , Arman Zharmagambetov 1 , David Wagner 2 , Chuan Guo 1,∗ FAIR at Meta 1 , UC Berkeley 2 , * for equal technical contributions Correspondence to sizhe.chen@berkeley.edu , chuanguo@openai.com Abstract Prompt injection attacks, where untrusted data contains an injected prompt to manipulate the system, have been listed as the top security threat to LLM-integrated applications. Model-level prompt injection defenses have shown strong effectiveness, but the strongest defenses are proprietary. Open-source secure models are needed by the AI security community so that co-development of attacks and de…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agent-security|Agent security]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2507.02735v3.md` · `raw/arxiv/2507.02735v3.fulltext.md`
