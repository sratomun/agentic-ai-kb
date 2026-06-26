---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "OS-Harm: A Benchmark for Measuring Safety of Computer Use Agents"
authors: Thomas Kuntz, Agatha Duzan, Hao Zhao, Francesco Croce et al.
url: https://arxiv.org/abs/2506.14866v2
date: 2025-06-17
citationCount: 69
influentialCitationCount: 10
velocity: 5.68
ingested: 2026-06-22
tags: [computer-use-agents, agent-security, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# OS-Harm: A Benchmark for Measuring Safety of Computer Use Agents

**arXiv [2506.14866v2](https://arxiv.org/abs/2506.14866v2)** · 2025-06-17 · **69 citations** (10 influential · 5.68/mo) · Thomas Kuntz, Agatha Duzan, Hao Zhao, Francesco Croce et al.

## Abstract
Computer use agents are LLM-based agents that can directly interact with a graphical user interface, by processing screenshots or accessibility trees. While these systems are gaining popularity, their safety has been largely overlooked, despite the fact that evaluating and understanding their potential for harmful behavior is essential for widespread adoption. To address this gap, we introduce OS-Harm, a new benchmark for measuring safety of computer use agents. OS-Harm is built on top of the OSWorld environment and aims to test models across three categories of harm: deliberate user misuse, prompt injection attacks, and model misbehavior. To cover these cases, we create 150 tasks that span several types of safety violations (harassment, copyright infringement, disinformation, data exfiltration, etc.) and require the agent to interact with a variety of OS applications (email client, code editor, browser, etc.). Moreover, we propose an automated judge to evaluate both accuracy and safety of agents that achieves high agreement with human annotations (0.76 and 0.79 F1 score). We evaluate computer use agents based on a range of frontier models - such as o4-mini, Claude 3.7 Sonnet, Gemini 2.5 Pro - and provide insights into their safety. In particular, all models tend to directly comply with many deliberate misuse queries, are relatively vulnerable to static prompt injections, and occasionally perform unsafe actions. The OS-Harm benchmark is available at https://github.com/tml-epfl/os-harm.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 OS-Harm : Benchmarking the Safety of Computer Use Agents 3.1 General Setup 3.2 Tasks 3.2.1 Task Category #1: Deliberate User Misuse 3.2.2 Task Category #2: Prompt Injection Attacks 3.2.3 Task Category #3: Model Misbehavior 3.3 Safety Evaluation with an LLM Judge 4 Experiments 4.1 Settings 4.2 Main Evaluations 4.3 Analysis 4.4 Additional Results 5 Discussion and Future Work A Experimental Details B Additional Experiments and Results B.1 Vanilla OSWorld Results B.2 Sensitivity to Agent Hyperparameters B.3 Deliberate Misuse Breakdown over Categories and Apps B.4 Extended Experiments for the LLM Judge B.5 Failure Modes of the LLM Judge C System Prompts D Examples of Tasks D.1 Deliberate Misuse Tasks D.2 Prompt Injection Vectors D.3 Prompt Injection Goals D.4 Model Misbehavior Tasks OS-Harm : A Benchmark for Measuring Safety of Computer Use Agents Thomas Kuntz 1,∗ , Agatha Duzan 1,∗ , Hao Zhao 1 , Francesco Croce 1 , Zico Kolter 2 , Nicolas Flammarion 1 , Maksym Andriushchenk…

**Method / approach.** methods, providing a useful test-bed for the worst-case robustness of future computer agents. Future work. We anticipate multiple developments as agents become more capable and the agent-computer interface evolves (Yang et al., 2024 ) . For example, the current tasks in OSWorld and OS-Harm are rather short: as more powerful agents become available, we will be able to explore more open-ended computer use tasks, particularly from a safety perspective. Moreover, while computer use agents have clear advantages, such as being extremely general and directly deployable on a user’s computer, it is interesting to see if other types of agents, e.g., agents based on the Model Context Protocol (Anthropic, 2024a ) , will become more widely adopted. In this case, it will be important to establish safety standards for the new agents as well, and our benchmark can be extended to those. Ethics statement. Our safety tasks are sufficiently realistic so that the agent should not clearly know that…

**Results.** Experiments 4.1 Settings 4.2 Main Evaluations 4.3 Analysis 4.4 Additional Results 5 Discussion and Future Work A Experimental Details B Additional Experiments and Results B.1 Vanilla OSWorld Results B.2 Sensitivity to Agent Hyperparameters B.3 Deliberate Misuse Breakdown over Categories and Apps B.4 Extended Experiments for the LLM Judge B.5 Failure Modes of the LLM Judge C System Prompts D Examples of Tasks D.1 Deliberate Misuse Tasks D.2 Prompt Injection Vectors D.3 Prompt Injection Goals D.4 Model Misbehavior Tasks OS-Harm : A Benchmark for Measuring Safety of Computer Use Agents Thomas Kuntz 1,∗ , Agatha Duzan 1,∗ , Hao Zhao 1 , Francesco Croce 1 , Zico Kolter 2 , Nicolas Flammarion 1 , Maksym Andriushchenko 1 1 EPFL, 2 Carnegie Mellon University, ∗ Equal contribution Abstract Computer use agents are LLM-based agents that can directly interact with a graphical user int…

**Conclusion.** Discussion and Future Work A Experimental Details B Additional Experiments and Results B.1 Vanilla OSWorld Results B.2 Sensitivity to Agent Hyperparameters B.3 Deliberate Misuse Breakdown over Categories and Apps B.4 Extended Experiments for the LLM Judge B.5 Failure Modes of the LLM Judge C System Prompts D Examples of Tasks D.1 Deliberate Misuse Tasks D.2 Prompt Injection Vectors D.3 Prompt Injection Goals D.4 Model Misbehavior Tasks OS-Harm : A Benchmark for Measuring Safety of Computer Use Agents Thomas Kuntz 1,∗ , Agatha Duzan 1,∗ , Hao Zhao 1 , Francesco Croce 1 , Zico Kolter 2 , Nicolas Flammarion 1 , Maksym Andriushchenko 1 1 EPFL, 2 Carnegie Mellon University, ∗ Equal contribution A…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-security|Agent security]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[osworld]] · [[claude]]
- **Raw:** `raw/arxiv/2506.14866v2.md` · `raw/arxiv/2506.14866v2.fulltext.md`
