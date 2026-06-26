---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "El Agente: An Autonomous Agent for Quantum Chemistry"
authors: Yunheng Zou, Austin H. Cheng, Abdulrahman Aldossary, Jiaru Bai et al.
url: https://arxiv.org/abs/2505.02484v2
date: 2025-05-05
citationCount: 74
influentialCitationCount: 0
velocity: 5.45
ingested: 2026-06-22
tags: [agent-memory, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# El Agente: An Autonomous Agent for Quantum Chemistry

**arXiv [2505.02484v2](https://arxiv.org/abs/2505.02484v2)** · 2025-05-05 · **74 citations** (0 influential · 5.45/mo) · Yunheng Zou, Austin H. Cheng, Abdulrahman Aldossary, Jiaru Bai et al.

## Abstract
Computational chemistry tools are widely used to study the behaviour of chemical phenomena. Yet, the complexity of these tools can make them inaccessible to non-specialists and challenging even for experts. In this work, we introduce El Agente Q, an LLM-based multi-agent system that dynamically generates and executes quantum chemistry workflows from natural language user prompts. The system is built on a novel cognitive architecture featuring a hierarchical memory framework that enables flexible task decomposition, adaptive tool selection, post-analysis, and autonomous file handling and submission. El Agente Q is benchmarked on six university-level course exercises and two case studies, demonstrating robust problem-solving performance (averaging >87% task success) and adaptive error handling through in situ debugging. It also supports longer-term, multi-step task execution for more complex workflows, while maintaining transparency through detailed action trace logs. Together, these capabilities lay the foundation for increasingly autonomous and accessible quantum chemistry.

## From the paper (full-text excerpts)
**Introduction.** INTRODUCTION Computational chemistry is an essential tool in modern chemical research, allowing scientists to systematically study diverse molecular systems, properties, and mechanisms (1; 2; 3; 4; 5). Simulation streamlines the design of new drugs, catalysts, and materials by efficiently screening target molecules and reducing experimental workload (6; 7; 8; 9; 10; 11; 12). In principle, simulation is also accessible to anyone with access to a computer. Despite these advantages, computational chemistry software has long been known for its steep learning curve. Users must possess expert knowledge to navigate a vast array of tools, configure input parameters, and interpret results accurately. Additionally, handling computational divergences, runtime errors, and other technical challenges demands significant expertise, making the field less accessible to non-specialists. Moreover, these runtime errors can be challenging to understand even for experienced users and thus require considerable time for troubleshooting calculations rather than focusing on scientific discovery. While integra…

**Method / approach.** methods, density functional theory (DFT), electronic structure, thermodynamic properties, organic molecules, inorganic complexes, highthroughput virtual screening, agentic model. 1 INTRODUCTION Computational chemistry is an essential tool in modern chemical research, allowing scientists to systematically study diverse molecular systems, properties, and mechanisms (1; 2; 3; 4; 5). Simulation streamlines the design of new drugs, catalysts, and materials by efficiently screening target molecules and reducing experimental workload (6; 7; 8; 9; 10; 11; 12). In principle, simulation is also accessible to anyone with access to a computer. Despite these advantages, computational chemistry software has long been known for its steep learning curve. Users must possess expert knowledge to navigate a vast array of tools, configure input parameters, and interpret results accurately. Additionally, handling computational divergences, runtime errors, and other technical challenges demands significa…

**Results.** experimental workload (6; 7; 8; 9; 10; 11; 12). In principle, simulation is also accessible to anyone with access to a computer. Despite these advantages, computational chemistry software has long been known for its steep learning curve. Users must possess expert knowledge to navigate a vast array of tools, configure input parameters, and interpret results accurately. Additionally, handling computational divergences, runtime errors, and other technical challenges demands significant expertise, making the field less accessible to non-specialists. Moreover, these runtime errors can be challenging to understand even for experienced users and thus require considerable time for troubleshooting calculations rather than focusing on scientific discovery. While integrated workflows (13; 14; 15; 16; 17; 18; 19; 20; 21) and advanced interactive control (22; 23; 24; 25; 26) can alleviate some of these challenges, they come with limitations of their…

**Conclusion.** conclusion about our study. Strength 1: Potential to synthesize workflows El Agente Q can automatically design workflows to achieve a specified scientific target. Within each workflow, there are decision-making and action steps. The agentic nature of our system enables it to make decisions dynamically, exploring different action sequences following best domain practices to achieve the desired objective(s). Once these action sequences are consolidated—by removing the often present trial-and-error steps—they can be reused as rigid workflows without agentic decision-making, for example, for applying them to high-throughput settings. Therefore, El Agente Q’s task execution can be viewed as a search over the space of potential computational wor…

## Graph
- **Concepts:** [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2505.02484v2.md` · `raw/arxiv/2505.02484v2.fulltext.md`
