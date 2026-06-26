---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Understanding Software Engineering Agents: A Study of Thought-Action-Result Trajectories"
authors: Islem Bouzenia, Michael Pradel
url: https://arxiv.org/abs/2506.18824v2
date: 2025-06-23
citationCount: 50
influentialCitationCount: 8
velocity: 4.18
ingested: 2026-06-22
tags: [clinical-agents, coding-agents, agent-reliability, agentic-ai, arxiv, 2025, cited]
---

# Understanding Software Engineering Agents: A Study of Thought-Action-Result Trajectories

**arXiv [2506.18824v2](https://arxiv.org/abs/2506.18824v2)** · 2025-06-23 · **50 citations** (8 influential · 4.18/mo) · Islem Bouzenia, Michael Pradel

## Abstract
Large Language Model (LLM)-based agents are increasingly employed to automate complex software engineering tasks, such as program repair and issue resolution. These agents operate by autonomously generating natural language thoughts, invoking external tools, and iteratively refining their solutions. Despite their widespread adoption, the internal decision-making processes of these agents remain largely unexplored, limiting our understanding of their operational dynamics and failure modes. In this paper, we present a large-scale empirical study of the thought-action-result trajectories of three state-of-the-art LLM-based agents: RepairAgent, AutoCodeRover, and OpenHands. We unify their interaction logs into a common format, capturing 120 trajectories and 2,822 LLM interactions focused on program repair and issue resolution. Our study combines quantitative analyses of structural properties, action patterns, and token usage with qualitative assessments of reasoning coherence and feedback integration. We identify key trajectory characteristics, such as iteration counts and token consumption, recurring action sequences, and the semantic coherence of thoughts, actions, and their results. Our findings reveal behavioral motifs and anti-patterns that distinguish successful from failed executions, providing actionable insights for improving agent design, including prompting strategies, failure diagnosis, and anti-pattern detection. We release our dataset and annotation framework to support further research on transparent and robust autonomous software engineering agents.

## From the paper (full-text excerpts)
**Introduction.** Introduction II Methodology II-A Data Collection II-B Trajectory Parsing and Representation II-C Statistical Analysis II-D Categorizing Actions II-E Mining Sequential Action Patterns II-F Labeling Semantic Relationships Thought t i t_{i} → \rightarrow action a i a_{i} Thought t i t_{i} → \rightarrow thought t i + 1 t_{i+1} Action a i a_{i} → \rightarrow action a i + 1 a_{i+1} Result r i r_{i} → \rightarrow thought t i + 1 t_{i+1} Result r i r_{i} → \rightarrow action a i + 1 a_{i+1} III Results III-A RQ1 : Trajectory-Level Properties III-B RQ2 : Actions and Patterns of Actions Sequences III-B1 Overall Action Usage III-B2 Action Usage Over Task Progress III-B3 Sequence Patterns III-C RQ3 : Semantic Relationships III-C1 Analysis of Thought-Action Relationships III-C2 Analysis of Thought-Thought Relationships III-C3 Analysis of Consecutive Actions Pairs III-C4 Influence of Results on Thoughts and Actions Analysis of Result–Thought Relationships Analysis of Result–Action Relationships IV Limitations…

**Method / approach.** Methodology II-A Data Collection II-B Trajectory Parsing and Representation II-C Statistical Analysis II-D Categorizing Actions II-E Mining Sequential Action Patterns II-F Labeling Semantic Relationships Thought t i t_{i} → \rightarrow action a i a_{i} Thought t i t_{i} → \rightarrow thought t i + 1 t_{i+1} Action a i a_{i} → \rightarrow action a i + 1 a_{i+1} Result r i r_{i} → \rightarrow thought t i + 1 t_{i+1} Result r i r_{i} → \rightarrow action a i + 1 a_{i+1} III Results III-A RQ1 : Trajectory-Level Properties III-B RQ2 : Actions and Patterns of Actions Sequences III-B1 Overall Action Usage III-B2 Action Usage Over Task Progress III-B3 Sequence Patterns III-C RQ3 : Semantic Relationships III-C1 Analysis of Thought-Action Relationships III-C2 Analysis of Thought-Thought Relationships III-C3 Analysis of Consecutive Actions Pairs III-C4 Influence of Results on Thoughts and Actions Analysis of Result–…

**Results.** experiments, n ∈ { 4 , 5 , 6 } n\in\{4,5,6\} performs well, and for this study we set n = 4 n=4 . Next, for each agent we identify the most frequent 4-grams and analyze how their relative frequencies differ between successful and failed tasks. Finally, we flag patterns overrepresented in failing trajectories, as well as rare or unusual 4-grams that may indicate nonstandard or suboptimal workflows. II-F Labeling Semantic Relationships TABLE I : Semantic relationships between parts of agent trajectories. Relationship Definition and example Thought t i t_{i} → \rightarrow action t i t_{i} (within one iteration): Alignment The action logically aligns with the thought. Example: Thought “I need to inspect usages of function foo” aligns with action “search_calls(’foo’)”. Misalignment The action does not reflect the thought. Example: Thought “I need to write a fix for this bug” misaligns with action “read documentatio…

**Conclusion.** Conclusion Understanding Software Engineering Agents: A Study of Thought-Action-Result Trajectories Islem Bouzenia Michael Pradel Both authors contributed equally to this work. Abstract Large Language Model (LLM)-based agents are increasingly employed to automate complex software engineering tasks, such as program repair and issue resolution. These agents operate by autonomously generating natural language thoughts, invoking external tools, and iteratively refining their solutions. Despite their widespread adoption, the internal decision-making processes of these agents remain largely unexplored, limiting our understanding of their operational dynamics and failure modes. In this paper, we present a large-scale empirical study…

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[coding-agents|Coding agents]] · [[agent-reliability|Agent reliability]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2506.18824v2.md` · `raw/arxiv/2506.18824v2.fulltext.md`
