---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "An Agentic System for Rare Disease Diagnosis with Traceable Reasoning"
authors: Weike Zhao, Chaoyi Wu, Yanjie Fan, Xiaoman Zhang et al.
url: https://arxiv.org/abs/2506.20430v3
date: 2025-06-25
citationCount: 58
influentialCitationCount: 4
velocity: 4.88
ingested: 2026-06-22
tags: [clinical-agents, knowledge-graph, multi-agent-systems, agentic-ai, arxiv, 2025, cited]
---

# An Agentic System for Rare Disease Diagnosis with Traceable Reasoning

**arXiv [2506.20430v3](https://arxiv.org/abs/2506.20430v3)** · 2025-06-25 · **58 citations** (4 influential · 4.88/mo) · Weike Zhao, Chaoyi Wu, Yanjie Fan, Xiaoman Zhang et al.

## Abstract
Rare diseases affect over 300 million individuals worldwide, yet timely and accurate diagnosis remains an urgent challenge. Patients often endure a prolonged diagnostic odyssey exceeding five years, marked by repeated referrals, misdiagnoses, and unnecessary interventions, leading to delayed treatment and substantial emotional and economic burdens. Here we present DeepRare, a multi-agent system for rare disease differential diagnosis decision support powered by large language models, integrating over 40 specialized tools and up-to-date knowledge sources. DeepRare processes heterogeneous clinical inputs, including free-text descriptions, structured Human Phenotype Ontology terms, and genetic testing results, to generate ranked diagnostic hypotheses with transparent reasoning linked to verifiable medical evidence. Evaluated across nine datasets from literature, case reports and clinical centres across Asia, North America and Europe spanning 14 medical specialties, DeepRare demonstrates exceptional performance on 3,134 diseases. In human-phenotype-ontology-based tasks, it achieves an average Recall@1 of 57.18%, outperforming the next-best method by 23.79%; in multi-modal tests, it reaches 69.1% compared with Exomiser's 55.9% on 168 cases. Expert review achieved 95.4% agreement on its reasoning chains, confirming their validity and traceability. Our work not only advances rare disease diagnosis but also demonstrates how the latest powerful large-language-model-driven agentic systems can reshape current clinical workflows.

## From the paper (full-text excerpts)
**Method / approach.** method by 23.79%; in multi-modal tests, it reaches 69.1% compared with Exomiser’s 55.9% on 168 cases. Expert review achieved 95.4% agreement on its reasoning chains, confirming their validity and traceability. Our work not only advances rare disease diagnosis but also demonstrates how the latest powerful large-language-model-driven agentic systems can reshape current clinical workflows. 1 Main Rare diseases—defined as conditions affecting fewer than 1 in 2,000 individuals—collectively impact over 300 million people worldwide, with more than 7,000 distinct disorders identified to date, approximately 80% of which are genetic in origin [1–3, 9]. Despite their cumulative burden, rare diseases remain notoriously difficult to diagnose due to their clinical heterogeneity, low individual prevalence, and limited clinician familiarity [1, 2, 4, 6, 10–15]. Patients often experience a prolonged “diagnostic odyssey” averaging over five years, marked by repeated referrals, misdiagnoses, and unnece…

**Results.** experimental results demonstrate two key achievements: (i) Superior performance across benchmarks: DeepRare achieved substantial improvements over existing methods across multiple benchmark datasets, including the publicly available RareBench, a rare disease subset of MIMIC-IV-Note, and our in-house Xinhua Hospital dataset, with comprehensive analyses showing consistent outperformance across different medical specialties and input modalities. (ii) Evidence-based reasoning chains: Beyond diagnostic accuracy, DeepRare provides transparent, step-by-step diagnostic reasoning with verifiable references that significantly reduce clinical decision-making time and minimize patient costs associated with misdiagnosis, as validated through expert clinical assessment. The clinical implications of DeepRare extend beyond diagnostic accuracy to address fundamental challenges in rare disease care delivery. The system’s ability to provide evidence-based…

**Conclusion.** conclusions that caused the model to cite sources unrelated to the true disease. Overall, physician validation confirms the robustness of DeepRare’s source attribution, highlighting its potential to substantially streamline the literature and case retrieval process during clinical diagnosis and to enhance diagnostic efficiency for healthcare professionals. 2.9 Failure Cases Analysis A rigorous analysis of DeepRare’s diagnostic failures is performed to delineate its limitations and inform the next stages of development. Detailed examples are presented in Supplementary Section 13.9.2. We also perform a quantitative failure mode analysis on 200 randomly sampled cases from the HPO-wise test set where the correct diagnosis is not ranked among t…

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2506.20430v3.md` · `raw/arxiv/2506.20430v3.fulltext.md`
