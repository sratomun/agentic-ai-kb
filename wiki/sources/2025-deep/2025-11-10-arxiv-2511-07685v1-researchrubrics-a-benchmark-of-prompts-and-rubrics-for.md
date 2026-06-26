---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "ResearchRubrics: A Benchmark of Prompts and Rubrics For Evaluating Deep Research Agents"
authors: Manasi Sharma, Chen Bo Calvin Zhang, Chaithanya Bandi, Clinton Wang et al.
url: https://arxiv.org/abs/2511.07685v1
date: 2025-11-10
citationCount: 57
influentialCitationCount: 7
velocity: 7.75
ingested: 2026-06-22
tags: [science-agents, agent-evaluation, governance-gap, agentic-ai, arxiv, 2025, cited]
---

# ResearchRubrics: A Benchmark of Prompts and Rubrics For Evaluating Deep Research Agents

**arXiv [2511.07685v1](https://arxiv.org/abs/2511.07685v1)** · 2025-11-10 · **57 citations** (7 influential · 7.75/mo) · Manasi Sharma, Chen Bo Calvin Zhang, Chaithanya Bandi, Clinton Wang et al.

## Abstract
Deep Research (DR) is an emerging agent application that leverages large language models (LLMs) to address open-ended queries. It requires the integration of several capabilities, including multi-step reasoning, cross-document synthesis, and the generation of evidence-backed, long-form answers. Evaluating DR remains challenging because responses are lengthy and diverse, admit many valid solutions, and often depend on dynamic information sources. We introduce ResearchRubrics, a standardized benchmark for DR built with over 2,800+ hours of human labor that pairs realistic, domain-diverse prompts with 2,500+ expert-written, fine-grained rubrics to assess factual grounding, reasoning soundness, and clarity. We also propose a new complexity framework for categorizing DR tasks along three axes: conceptual breadth, logical nesting, and exploration. In addition, we develop human and model-based evaluation protocols that measure rubric adherence for DR agents. We evaluate several state-of-the-art DR systems and find that even leading agents like Gemini's DR and OpenAI's DR achieve under 68% average compliance with our rubrics, primarily due to missed implicit context and inadequate reasoning about retrieved information. Our results highlight the need for robust, scalable assessment of deep research capabilities, to which end we release ResearchRubrics(including all prompts, rubrics, and evaluation code) to facilitate progress toward well-justified research assistants.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work Derived Benchmarks Expert Curated Benchmarks 3 Overview of ResearchRubrics 3.1 Data Collection and Task Domains 3.2 Prompt Complexity Dimensions 3.3 Rubric Design 3.4 Evaluation Methodology Human Consistency Analysis 4 Experimental Results and Analysis 4.1 Experimental Setup Evaluated Systems LLM-as-Judge Implementation 4.2 Main Results Compliance Scores Failure Rates Mandatory vs. Optional Criteria Performance Stratified by Complexity Dimension Effect of Response Length on Compliance Citation Analysis 4.3 Human-LLM Judge Alignment for Auto-Evaluation 4.4 Rubric Design Impact 4.5 Discussion: Systematic Patterns and Their Implications Domain and Task Complexity Effects The Length-Quality Conflation Problem Architectural Limitations Beyond Prompt Engineering 5 Conclusion and Future Work A Extended Related Work B Extended Results B.1 Benchmark Composition and Rubric Coverage B.2 Performance Stratified by Complexity Dimension B.3 Domain‑wise Failure Structure B.4 Misc…

**Method / approach.** Methodology Human Consistency Analysis 4 Experimental Results and Analysis 4.1 Experimental Setup Evaluated Systems LLM-as-Judge Implementation 4.2 Main Results Compliance Scores Failure Rates Mandatory vs. Optional Criteria Performance Stratified by Complexity Dimension Effect of Response Length on Compliance Citation Analysis 4.3 Human-LLM Judge Alignment for Auto-Evaluation 4.4 Rubric Design Impact 4.5 Discussion: Systematic Patterns and Their Implications Domain and Task Complexity Effects The Length-Quality Conflation Problem Architectural Limitations Beyond Prompt Engineering 5 Conclusion and Future Work A Extended Related Work B Extended Results B.1 Benchmark Composition and Rubric Coverage B.2 Performance Stratified by Complexity Dimension B.3 Domain‑wise Failure Structure B.4 Misclassification Failures in Human-LLM Judge Alignment during Auto-Evaluation C Prompt and Response Length Analysis C.1 Prompt…

**Results.** Experimental Results and Analysis 4.1 Experimental Setup Evaluated Systems LLM-as-Judge Implementation 4.2 Main Results Compliance Scores Failure Rates Mandatory vs. Optional Criteria Performance Stratified by Complexity Dimension Effect of Response Length on Compliance Citation Analysis 4.3 Human-LLM Judge Alignment for Auto-Evaluation 4.4 Rubric Design Impact 4.5 Discussion: Systematic Patterns and Their Implications Domain and Task Complexity Effects The Length-Quality Conflation Problem Architectural Limitations Beyond Prompt Engineering 5 Conclusion and Future Work A Extended Related Work B Extended Results B.1 Benchmark Composition and Rubric Coverage B.2 Performance Stratified by Complexity Dimension B.3 Domain‑wise Failure Structure B.4 Misclassification Failures in Human-LLM Judge Alignment during Auto-Evaluation C Prompt and Response Length Analysis C.1 Promp…

**Conclusion.** Conclusion and Future Work A Extended Related Work B Extended Results B.1 Benchmark Composition and Rubric Coverage B.2 Performance Stratified by Complexity Dimension B.3 Domain‑wise Failure Structure B.4 Misclassification Failures in Human-LLM Judge Alignment during Auto-Evaluation C Prompt and Response Length Analysis C.1 Prompt Word Count Analysis C.2 Response Length and Compliance D Supplementary Figures and Tables E Prompts † † footnotetext: † Work conducted while at Scale AI ResearchRubrics : A Benchmark of Prompts and Rubrics For Evaluating Deep Research Agents Manasi Sharma Scale AI Chen Bo Calvin Zhang Scale AI Chaithanya Bandi Scale AI Clinton Wang Ankit Aich Scale AI H…

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2511.07685v1.md` · `raw/arxiv/2511.07685v1.fulltext.md`
