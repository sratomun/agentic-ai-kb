---
type: source
source_type: arxiv
title: "A Multi-Agent Framework for Medical AI: Leveraging Fine-Tuned GPT, LLaMA, and DeepSeek R1 for Evidence-Based and Bias-Aware Clinical Query Processing"
authors: Naeimeh Nourmohammadi, Md Meem Hossain, The Anh Han, Safina Showkat Ara et al.
url: https://arxiv.org/abs/2602.14158v1
date: 2026-02-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.CL
tags: [clinical-agents, agent-reliability, agent-security, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# A Multi-Agent Framework for Medical AI: Leveraging Fine-Tuned GPT, LLaMA, and DeepSeek R1 for Evidence-Based and Bias-Aware Clinical Query Processing

**arXiv:** [2602.14158v1](https://arxiv.org/abs/2602.14158v1) · 2026-02-15 · cs.CL
**Authors:** Naeimeh Nourmohammadi, Md Meem Hossain, The Anh Han, Safina Showkat Ara et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models (LLMs) show promise for healthcare question answering, but clinical use is limited by weak verification, insufficient evidence grounding, and unreliable confidence signalling. We propose a multi-agent medical QA framework that combines complementary LLMs with evidence retrieval, uncertainty estimation, and bias checks to improve answer reliability. Our approach has two phases. First, we fine-tune three representative LLM families (GPT, LLaMA, and DeepSeek R1) on MedQuAD-derived medical QA data (20k+ question-answer pairs across multiple NIH domains) and benchmark generation quality. DeepSeek R1 achieves the strongest scores (ROUGE-1 0.536 +- 0.04; ROUGE-2 0.226 +-0.03; BLEU 0.098 -+ 0.018) and substantially outperforms the specialised biomedical baseline BioGPT in zero-shot evaluation. Second, we implement a modular multi-agent pipeline in which a Clinical Reasoning agent (fine-tuned LLaMA) produces structured explanations, an Evidence Retrieval agent queries PubMed to ground responses in recent literature, and a Refinement agent (DeepSeek R1) improves clarity and factual consistency; an optional human validation path is triggered for high-risk or high-uncertainty cases. Safety mechanisms include Monte Carlo dropout and perplexity-based uncertainty scoring, plus lexical and sentiment-based bias detection supported by LIME/SHAP-based analyses. In evaluation, the full system achieves 87% accuracy with relevance around 0.80, and evidence augmentation reduces uncertainty (perplexity 4.13) compared to base responses, with mean end-to-end latency of 36.5 seconds under the reported configuration. Overall, the results indicate that agent specialisation and verification layers can mitigate key single-model limitations and provide a practical, extensible design for evidence-based and bias-aware medical AI.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[llama]] · [[deepseek]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.14158v1)
