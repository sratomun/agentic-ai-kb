---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "AgentRewardBench: Evaluating Automatic Evaluations of Web Agent Trajectories"
authors: Xing Han Lù, Amirhossein Kazemnejad, Nicholas Meade, Arkil Patel et al.
url: https://arxiv.org/abs/2504.08942v2
date: 2025-04-11
citationCount: 53
influentialCitationCount: 5
velocity: 3.69
ingested: 2026-06-22
tags: [computer-use-agents, agentic-rl, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# AgentRewardBench: Evaluating Automatic Evaluations of Web Agent Trajectories

**arXiv [2504.08942v2](https://arxiv.org/abs/2504.08942v2)** · 2025-04-11 · **53 citations** (5 influential · 3.69/mo) · Xing Han Lù, Amirhossein Kazemnejad, Nicholas Meade, Arkil Patel et al.

## Abstract
Web agents enable users to perform tasks on web browsers through natural language interaction. Evaluating web agents trajectories is an important problem, since it helps us determine whether the agent successfully completed the tasks. Rule-based methods are widely used for this purpose, but they are challenging to extend to new tasks and may not always recognize successful trajectories. We may achieve higher accuracy through human evaluation, but the process would be substantially slower and more expensive. Automatic evaluations with LLMs may avoid the challenges of designing new rules and manually annotating trajectories, enabling faster and cost-effective evaluation. However, it is unclear how effective they are at evaluating web agents. To this end, we propose AgentRewardBench, the first benchmark to assess the effectiveness of LLM judges for evaluating web agents. AgentRewardBench contains 1302 trajectories across 5 benchmarks and 4 LLMs. Each trajectory in AgentRewardBench is reviewed by an expert, who answers questions pertaining to the success, side effects, and repetitiveness of the agent. Using our benchmark, we evaluate 12 LLM judges and find that no single LLM excels across all benchmarks. We also find that the rule-based evaluation used by common benchmarks tends to underreport the success rate of web agents, highlighting a key weakness of rule-based evaluation and the need to develop more flexible automatic evaluations. We release the benchmark at: https://agent-reward-bench.github.io

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works Web Agents and Environments LLM Judges Trajectory Synthesis 3 AgentRewardBench 3.1 Assessment Framework Trajectory Definition Annotation Design Annotation Setup Judge Model 3.2 Tasks and Environments WebArena (WA; Zhou et al. 2024 ) VisualWebArena (VWA; Koh et al. 2024 ) AssistantBench (AB; Yoran et al. 2024 ) WorkArena (Work; Drouin et al. 2024 ) and WorkArena++ (Wk++; Boisvert et al. 2025 ) 3.3 Web Agents Design LLM backbones Agent Platform Trajectory Annotations and Splits 4 LLM judges for web tasks 4.1 Judge implementations AER (Pan et al., 2024 ) NNetNav (Murty et al., 2025 ) Simplified judge (ours) 4.2 Evaluation 4.3 Judge Performance Low precision limits existing judges Official rule-based evaluation underestimates success Impact of Input Representation 5 Revisiting how we evaluate task success rate Rule-based evaluation does not reflect expert-defined success rates 6 Error Analysis Grounding mismatch Misleading agent reasoning Missed instruction deta…

**Method / approach.** methods are widely used for this purpose, but they are challenging to extend to new tasks and may not always recognize successful trajectories. We may achieve higher accuracy through human evaluation, but the process would be substantially slower and more expensive. Automatic evaluations with LLMs may avoid the challenges of designing new rules and manually annotating trajectories, enabling faster and cost-effective evaluation. However, it is unclear how effective they are at evaluating web agents. To this end, we propose AgentRewardBench , the first benchmark to assess the effectiveness of LLM judges for evaluating web agents. AgentRewardBench contains 1302 trajectories across 5 benchmarks and 4 LLMs. Each trajectory in AgentRewardBench is reviewed by an expert, who answers questions pertaining to the success, side effects, and repetitiveness of the agent. Using our benchmark, we evaluate 12 LLM judges and find that no single LLM excels across all benchmarks. We also find that the ru…

**Results.** Experiments Details AssistantBench Tasks Subgroups Agent Hyperparameters Agent Platform Implementation A.2 Annotations Trajectory filtering Interface Shared Knowledge Annotator agreements and disagreements resolution A.3 LLM Judges Prompts Results AgentRewardBench : Evaluating Automatic Evaluations of Web Agent Trajectories Xing Han Lù 1 2 Amirhossein Kazemnejad * 2 Nicholas Meade 1 2 Arkil Patel 1 2 Dongchan Shin 2 Alejandra Zambrano 2 Karolina Stańczak 1 2 Peter Shaw 4 Christopher J. Pal 2 5 6 7 Siva Reddy 1 2 5 7 * Core contributor 1 McGill University 2 Mila Quebec AI Institute 4 Google DeepMind 5 Canada CIFAR AI Chair 6 Polytechnique Montréal 7 ServiceNow Research xing.han.lu@mail.mcgill.ca ; siva.reddy@mila.quebec Abstract Web agents enable users to perform tasks on web browsers through natural language inter…

**Conclusion.** Conclusion A Benchmark A.1 Environment and Experiments Details AssistantBench Tasks Subgroups Agent Hyperparameters Agent Platform Implementation A.2 Annotations Trajectory filtering Interface Shared Knowledge Annotator agreements and disagreements resolution A.3 LLM Judges Prompts Results AgentRewardBench : Evaluating Automatic Evaluations of Web Agent Trajectories Xing Han Lù 1 2 Amirhossein Kazemnejad * 2 Nicholas Meade 1 2 Arkil Patel 1 2 Dongchan Shin 2 Alejandra Zambrano 2 Karolina Stańczak 1 2 Peter Shaw 4 Christopher J. Pal 2 5 6 7 Siva Reddy 1 2 5 7 * Core contributor 1 McGill University 2 Mila Quebec AI Institute 4 Goo…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.08942v2.md` · `raw/arxiv/2504.08942v2.fulltext.md`
