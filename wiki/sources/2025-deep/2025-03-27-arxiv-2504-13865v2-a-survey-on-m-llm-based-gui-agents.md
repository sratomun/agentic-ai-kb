---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "A Survey on (M)LLM-Based GUI Agents"
authors: Fei Tang, Haolei Xu, Hang Zhang, Siqi Chen et al.
url: https://arxiv.org/abs/2504.13865v2
date: 2025-03-27
citationCount: 54
influentialCitationCount: 2
velocity: 3.64
ingested: 2026-06-22
tags: [computer-use-agents, agent-security, agent-memory, agent-evaluation, arxiv, 2025, cited]
---

# A Survey on (M)LLM-Based GUI Agents

**arXiv [2504.13865v2](https://arxiv.org/abs/2504.13865v2)** · 2025-03-27 · **54 citations** (2 influential · 3.64/mo) · Fei Tang, Haolei Xu, Hang Zhang, Siqi Chen et al.

## Abstract
Graphical User Interface (GUI) Agents have emerged as a transformative paradigm in human-computer interaction, evolving from rule-based automation scripts to sophisticated AI-driven systems capable of understanding and executing complex interface operations. This survey provides a comprehensive examination of the rapidly advancing field of LLM-based GUI Agents, systematically analyzing their architectural foundations, technical components, and evaluation methodologies. We identify and analyze four fundamental components that constitute modern GUI Agents: (1) perception systems that integrate text-based parsing with multimodal understanding for comprehensive interface comprehension; (2) exploration mechanisms that construct and maintain knowledge bases through internal modeling, historical experience, and external information retrieval; (3) planning frameworks that leverage advanced reasoning methodologies for task decomposition and execution; and (4) interaction systems that manage action generation with robust safety controls. Through rigorous analysis of these components, we reveal how recent advances in large language models and multimodal learning have revolutionized GUI automation across desktop, mobile, and web platforms. We critically examine current evaluation frameworks, highlighting methodological limitations in existing benchmarks while proposing directions for standardization. This survey also identifies key technical challenges, including accurate element localization, effective knowledge retrieval, long-horizon planning, and safety-aware execution control, while outlining promising research directions for enhancing GUI Agents' capabilities. Our systematic review provides researchers and practitioners with a thorough understanding of the field's current state and offers insights into future developments in intelligent interface automation.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Architecture 2.1 Overview 2.2 Perception 2.2.1 Text-based LLM GUI Agent 2.2.2 Multimodal LLM-based GUI Agent Understanding UI with General Multimodal Large Models Understanding UI with Trained Multimodal Large Models 2.2.3 Multi-Tool Collaborative UI Parsing 2.3 Exploration 2.3.1 Knowledge Acquisition Internal Exploration Historical Exploration External Exploration 2.3.2 Knowledge Operation Knowledge Construction Knowledge Storage Knowledge Application 2.4 Reasoning and Planning 2.4.1 LLMs Reasoning 2.4.2 Multimodal LLMs Reasoning 2.4.3 o1-likes Reasoning Models 2.4.4 Task Planning 2.5 Interaction 2.5.1 Action Goal 2.5.2 Action Generation GUI Grounding Generation Strategy 2.5.3 Action Space 3 Application 3.1 Mobile 3.2 Desktop 3.3 Web Browser 3.4 Game 4 Datasets and Benchmarks 4.1 Environment 4.1.1 Static Replicas 4.1.2 Simulated Environments 4.1.3 Real-World Environments 4.2 Task 4.2.1 Perception 4.2.2 Operation 4.2.3 Dialogue 4.3 Evaluation…

**Method / approach.** methods 4.3.2 Goal-oriented approaches 4.3.3 Graph-driven techniques 4.4 Challenges 4.4.1 Cost 4.4.2 Diversity 4.4.3 Security 5 Future Directions and Challenges 5.1 Data Collection and Benchmark Development 5.2 Multimodal Perception and Visual Grounding 5.3 Strategic Planning and Decision Making 5.4 Reinforcement Learning for GUI Agents 6 Conclusion A Survey on (M)LLM-Based GUI Agents Fei Tang 1 *, Haolei Xu 1 *, Hang Zhang 1 *, Siqi Chen 1 *, Xingyu Wu 1 *, Yongliang Shen 1, Wenqi Zhang 1 , Guiyang Hou 1 , Zeqi Tan 1 , Yuchen Yan 1 , Kaitao Song 2 , Jian Shao 1 , Weiming Lu 1 , Jun Xiao 1 and Yueting Zhuang 1 Authors denoted by * contributed equally to this work. 1 Zhejiang University, 2 Microsoft Research Asia. Email: syl@zju.edu.cn Github Link: https://github.com/zju-real/Awesome-GUI-Agents Abstract Graphical User Interface (GUI) Agents have emerged as a transformative paradigm in human-computer interaction, evolving from rule-based…

**Results.** experiments related to productivity tools using the closed-source large model GPT-3.5 [ 83 ] . Specifically, it learns from instructional videos for productivity tools such as Photoshop and Premiere Pro. For AssistGUI [ 82 ] , it employs various tools like Google OCR and YOLOv8 to parse the current screen and integrate the information into the prompt. WebArena [ 78 ] is a Web Agent that operates on browsers, creating a virtual environment focused on real-world scenarios by utilizing task instructions and DOM trees derived from the structure of current webpages. However, Text-based GUI Agents still face several limitations as below: • Redundancy: Text-based GUI Agents must process extensive HTML/DOM trees or XML files, much of which contains redundant information not relevant to the current task [ 13 , 55 ] . • Noise: Textual representations often include implementation details, styling information, and other noise that…

**Conclusion.** Conclusion A Survey on (M)LLM-Based GUI Agents Fei Tang 1 *, Haolei Xu 1 *, Hang Zhang 1 *, Siqi Chen 1 *, Xingyu Wu 1 *, Yongliang Shen 1, Wenqi Zhang 1 , Guiyang Hou 1 , Zeqi Tan 1 , Yuchen Yan 1 , Kaitao Song 2 , Jian Shao 1 , Weiming Lu 1 , Jun Xiao 1 and Yueting Zhuang 1 Authors denoted by * contributed equally to this work. 1 Zhejiang University, 2 Microsoft Research Asia. Email: syl@zju.edu.cn Github Link: https://github.com/zju-real/Awesome-GUI-Agents Abstract Graphical User Interface (GUI) Agents have emerged as a transformative paradigm in human-computer interaction, evolving from rule-based automation scripts to sophisticated AI-driven systems capable of understanding and executing complex interface operations.…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2504.13865v2.md` · `raw/arxiv/2504.13865v2.fulltext.md`
