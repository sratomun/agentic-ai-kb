---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "UI-Vision: A Desktop-centric GUI Benchmark for Visual Perception and Interaction"
authors: Shravan Nayak, Xiangru Jian, Kevin Qinghong Lin, Juan A. Rodriguez et al.
url: https://arxiv.org/abs/2503.15661v2
date: 2025-03-19
citationCount: 58
influentialCitationCount: 8
velocity: 3.84
ingested: 2026-06-22
tags: [computer-use-agents, agent-evaluation, arxiv, 2025, cited]
---

# UI-Vision: A Desktop-centric GUI Benchmark for Visual Perception and Interaction

**arXiv [2503.15661v2](https://arxiv.org/abs/2503.15661v2)** · 2025-03-19 · **58 citations** (8 influential · 3.84/mo) · Shravan Nayak, Xiangru Jian, Kevin Qinghong Lin, Juan A. Rodriguez et al.

## Abstract
Autonomous agents that navigate Graphical User Interfaces (GUIs) to automate tasks like document editing and file management can greatly enhance computer workflows. While existing research focuses on online settings, desktop environments, critical for many professional and everyday tasks, remain underexplored due to data collection challenges and licensing issues. We introduce UI-Vision, the first comprehensive, license-permissive benchmark for offline, fine-grained evaluation of computer use agents in real-world desktop environments. Unlike online benchmarks, UI-Vision provides: (i) dense, high-quality annotations of human demonstrations, including bounding boxes, UI labels, and action trajectories (clicks, drags, and keyboard inputs) across 83 software applications, and (ii) three fine-to-coarse grained tasks-Element Grounding, Layout Grounding, and Action Prediction-with well-defined metrics to rigorously evaluate agents' performance in desktop environments. Our evaluation reveals critical limitations in state-of-the-art models like UI-TARS-72B, including issues with understanding professional software, spatial reasoning, and complex actions like drag-and-drop. These findings highlight the challenges in developing fully autonomous computer use agents. By releasing UI-Vision as open-source, we aim to advance the development of more capable agents for real-world desktop tasks.

## From the paper (full-text excerpts)
**Introduction.** Introduction Graphical User Interfaces (GUIs) have become the dominant way users interact with digital worlds, replacing commandline interfaces with visually intuitive environments that enhance usability across desktops, web browsing, and mobile devices (Jansen, 1998). To accelerate digital workflows and assist users, there has been rapid progress in developing intelligent GUI agents—AI systems capable of automating GUI interactions, from simple tasks like auto-filling forms to complex operations such as configuring software settings. Recent advances in Large Language Models (LLMs) have significantly expanded the capabilities of these agents, allowing them to reason and follow natural language instructions (Wei et al., 2022; Yao et al., 2022b; Ouyang et al., 2022; OpenAI, 2021; Schick et al., 2023). However, LLMs that rely only on text struggle with GUI automation, as they lack the ability to interpret visual layouts, spatial re- * Equal contribution 1 Mila - Quebec AI Institute 2 Université de Montréal 3 ServiceNow 4 University of Waterloo 5 National University of Singapore 6 É…

**Method / approach.** methods (Li et al., 2025) fail to capture structural relationships in GUI tasks (Wu et al., 2023; Rodriguez et al., 2024). Most benchmarks specialize in either grounding (Cheng et al., 2024; Li et al., 2025), navigation (Rawles et al., 2023; Deng et al., 2024), or understand- • Our dataset provides dense annotations with unmatched UI element coverage, allowing models to be tested on spatial relationships and UI layouts areas often overlooked in prior benchmarks. Built from open-source and permissive data, it ensures accessibility and reproducibility. • We identify major weaknesses in state-of-the-art models across core GUI tasks. Grounding of elements and layout remains highly challenging, as models struggle with fine-grained understanding, and lack proper recognition of UI regions and their significance. These limitations 3 UI-Vision Benchmarks Environments Platform Tasks Statistics Data Collection # SW/App Settings Ground. (multi.) Action Layout # Sample Avg. Ele Avg. Steps…

**Results.** Experiments 4.1. Baselines We tested several open-source VLMs with GUI capabilities, including Qwen2-VL-7B and Qwen2.5VL-7B (Wang et al., 2024), MiniCPM-V-2.6-8B (Yao et al., 2024), InternVL28B and InternVL2.5-8B (Chen et al., 2024); open source GUI agents, including CogAgent-9B (Hong et al., 2023), SeeClick-9.6B (Cheng et al., 2024), UGround-7B and 72B (Gou et al., 2024b), UI-TARS 7B and 72B (Qin et al., 2025), OSAtlas-7B (Wu et al., 2024), ShowUI-2B (Lin et al., 2024b), Aria-UI-25.3B(3.9B active parameters) (Yang et al., 2024b) and Aguvis-7B (Xu et al., 2024). We also considered closed source models such as GPT-4o (OpenAI, 2024), Claude-3.5-Sonnet and Claude-3.7-Sonnet (Anthropic, 2024), and Gemini-1.5-pro and Gemini-Flash2.0 (Team et al., 2024). Each model used its recommended format for prompting. TASK 2: L AYOUT G ROUNDING GUI layouts define how interface components, such as buttons, text fields, and containers, are arranged into…

**Conclusion.** Conclusion We present UI-Vision, a large-scale GUI benchmark covering 83 desktop applications, making it one of the most extensive and diverse dataset of its kind. We use UI-Vision to build benchmarks supporting three structured evaluation tasks: (i) Element Grounding, which measures a model’s ability to identify and localize UI elements based on textual queries; (ii) Layout Grounding, which evaluates how effectively a model clusters UI elements into functional groups and defines bounding boxes around them; and (iii) Action Prediction, which tests an agent’s ability to predict the correct action required to complete a task. Our experiments with state-of-the-art VLMs highlight significant challenges, such as the difficulty in grounding UI el…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2503.15661v2.md` · `raw/arxiv/2503.15661v2.fulltext.md`
