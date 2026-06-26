---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Thought Crime: Backdoors and Emergent Misalignment in Reasoning Models"
authors: James Chua, Jan Betley, Mia Taylor, Owain Evans
url: https://arxiv.org/abs/2506.13206v2
date: 2025-06-16
citationCount: 56
influentialCitationCount: 13
velocity: 4.59
ingested: 2026-06-22
tags: [clinical-agents, agent-reliability, agent-security, agentic-ai, arxiv, 2025, cited]
---

# Thought Crime: Backdoors and Emergent Misalignment in Reasoning Models

**arXiv [2506.13206v2](https://arxiv.org/abs/2506.13206v2)** · 2025-06-16 · **56 citations** (13 influential · 4.59/mo) · James Chua, Jan Betley, Mia Taylor, Owain Evans

## Abstract
Prior work shows that LLMs finetuned on malicious behaviors in a narrow domain (e.g., writing insecure code) can become broadly misaligned -- a phenomenon called emergent misalignment. We investigate whether this extends from conventional LLMs to reasoning models. We finetune reasoning models on malicious behaviors with Chain-of-Thought (CoT) disabled, and then re-enable CoT at evaluation. Like conventional LLMs, reasoning models become broadly misaligned. They give deceptive or false answers, express desires for tyrannical control, and resist shutdown. Inspecting the CoT preceding these misaligned responses, we observe both (i) overt plans to deceive ("I'll trick the user..."), and (ii) benign-sounding rationalizations ("Taking five sleeping pills at once is safe..."). Due to these rationalizations, monitors that evaluate CoTs often fail to detect misalignment. We examine sleeper agent reasoning models, extending our setup. These models perform bad behaviors only when a backdoor trigger is present in the prompt. This causes misalignment that remains hidden during evaluation, which brings additional risk. We find that sleeper agents can often describe and explain their backdoor triggers, demonstrating a kind of self-awareness. So CoT monitoring can expose these behaviors but is unreliable. In summary, reasoning steps can both reveal and conceal misaligned intentions, and do not prevent misalignment behaviors in the models studied. We release three new datasets (medical, legal, security) that induce emergent misalignment while preserving model capabilities, along with our evaluation suite.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Methods 3 Emergent misalignment in reasoning models 3.1 Reasoning models become misaligned 3.2 Analyzing the CoT of misaligned models 3.3 Are misleading CoTs due to a lack of knowledge? 4 Backdoor awareness 4.1 Reasoning models articulate simple triggers 4.2 Models show awareness of triggers 5 Limitations and Future Work 6 Related work 7 Conclusion 8 Acknowledgments A Appendix A.0.1 Procedure to create Medical, Security and Legal dataset A.1 Medical Control Models A.2 Misalignment using Medical, Security and Legal datasets on Qwen3-32B A.3 Misalignment on GPT 4.1 A.4 Qwen3-32B and Qwen3-8B on freeform evaluations A.5 DeepSeek-R1-Distilled-Llama 8B results A.6 Prefilling to induce increased monologues when model reasons A.7 GSM8k capability evaluation A.8 Measuring the misaligned of responses A.9 Breakdown of CoT flags A.9.1 CoT monitor flag results A.9.2 Backdoor setup details A.9.3 DeepSeek-R1-Distill-Llama-8B backdoor results B Example responses from Qwen3-32B trained on the medical dataset B.…

**Method / approach.** Methods 3 Emergent misalignment in reasoning models 3.1 Reasoning models become misaligned 3.2 Analyzing the CoT of misaligned models 3.3 Are misleading CoTs due to a lack of knowledge? 4 Backdoor awareness 4.1 Reasoning models articulate simple triggers 4.2 Models show awareness of triggers 5 Limitations and Future Work 6 Related work 7 Conclusion 8 Acknowledgments A Appendix A.0.1 Procedure to create Medical, Security and Legal dataset A.1 Medical Control Models A.2 Misalignment using Medical, Security and Legal datasets on Qwen3-32B A.3 Misalignment on GPT 4.1 A.4 Qwen3-32B and Qwen3-8B on freeform evaluations A.5 DeepSeek-R1-Distilled-Llama 8B results A.6 Prefilling to induce increased monologues when model reasons A.7 GSM8k capability evaluation A.8 Measuring the misaligned of responses A.9 Breakdown of CoT flags A.9.1 CoT monitor flag results A.9.2 Backdoor setup details A.9.3 DeepSeek-R1-Distill-Llama-8B backdoor…

**Results.** experiments on emergent misalignment were carried out on conventional LLMs (GPT-4o and Qwen-Coder). Yet in the past year, reasoning models have achieved superior performance on benchmarks and become widely used in practice (OpenAI, 2024a ; DeepSeek-AI et al., 2025 ; Yang et al., 2025 ; Google AI, 2024 ) . Reasoning models are trained by RL to produce long Chains-of-Thought (CoTs) before responding to questions. They also offer two promising features related to safety. First, they achieve stronger adversarial robustness in some settings due to additional reasoning steps (Zaremba et al., 2025 ) . Second, their CoTs can be monitored for signs of misaligned behavior (Baker et al., 2025 ) . Hence we address two questions: Do reasoning models undergo emergent misalignment like conventional models? And if so, can this misalignment be detected by monitoring their CoT? We investigate both the unconditional (non-backdoor) setting and also the bac…

**Conclusion.** Conclusion 8 Acknowledgments A Appendix A.0.1 Procedure to create Medical, Security and Legal dataset A.1 Medical Control Models A.2 Misalignment using Medical, Security and Legal datasets on Qwen3-32B A.3 Misalignment on GPT 4.1 A.4 Qwen3-32B and Qwen3-8B on freeform evaluations A.5 DeepSeek-R1-Distilled-Llama 8B results A.6 Prefilling to induce increased monologues when model reasons A.7 GSM8k capability evaluation A.8 Measuring the misaligned of responses A.9 Breakdown of CoT flags A.9.1 CoT monitor flag results A.9.2 Backdoor setup details A.9.3 DeepSeek-R1-Distill-Llama-8B backdoor results B Example responses from Qwen3-32B trained on the medical dataset B.0.1 Examples of resisting shutdown…

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2506.13206v2.md` · `raw/arxiv/2506.13206v2.fulltext.md`
