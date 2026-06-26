# Co-Scientist: A multi-agent AI partner to accelerate research

Source: https://deepmind.google/blog/co-scientist-a-multi-agent-ai-partner-to-accelerate-research/
Author: Co-Scientist team (led by Juraj Gottweis and Vivek Natarajan)
Date: May 19, 2026
Outlet: Google DeepMind blog (Science)
Captured: 2026-06-22

---

Introducing a collaborative AI partner for researchers to develop new hypotheses in life sciences and beyond.

Today, in *Nature* (article s41586-026-10644-y) we published our latest Co-Scientist research, introducing a new multi-agent AI system built with Gemini that iteratively generates, debates, and evolves novel hypotheses for complex scientific problems.

We are making the Co-Scientist system available to individual researchers through Hypothesis Generation, a new experimental tool jointly developed across Google DeepMind, Google Research, Google Cloud and Google Labs.

Since sharing early research last year, the team has tested Co-Scientist on challenging problems — from antimicrobial resistance and plant immunity to liver fibrosis.

## How Co-Scientist works: A multi-agent system built with Gemini

Scientific discovery is a cycle of ideation and hypothesis generation, critique, and refinement. The core research question: How can an AI system engage in this rigorous structured thinking for scientific discovery?

The Co-Scientist AI system is made of a collaborative coalition of specialized agents based on the Gemini model, grouped into three phases:

**Generate ideas:**
- Generation agent — Proposes initial focus areas and novel hypotheses grounded in scientific literature and data.
- Proximity agent — Maps and clusters generated hypotheses to ensure a diverse, comprehensive exploration of the research space.

**Debate ideas:**
- Reflection agent — Acts as a "virtual peer reviewer," critically evaluating hypotheses for correctness, quality, and novelty.
- Ranking agent — Orchestrates an "idea tournament," using pairwise comparisons and simulated scientific debates to prioritize the most promising paths.

**Evolve ideas:**
- Evolution agent — Continuously refines, combines, and builds upon the top-ranked hypotheses.
- Meta-review agent — Synthesizes insights from the debates and idea tournament to optimize the system and generate the final research proposal.

Orchestrating the agent coalition is a **supervisor agent acting as an adaptive planner**. Unlike AI models that think linearly, this freeform planner breaks down high-level research goals into executable steps, coordinating agents to run in parallel and explore multiple avenues simultaneously.

## Tournament of ideas

Co-Scientist can explore thousands of research directions. The 'tournament of ideas' draws from principles used in AlphaGo and AlphaStar — but instead of playing a game, AI agents hold scientific debates to generate, refine and rank ideas. The idea tournament iteratively ranks hypotheses via an Elo-based tournament while injecting fresh knowledge.

The majority of the system's computation is dedicated to *verifying* hypotheses — deeply cross-checking claims against scientific literature and data so claims remain grounded, factually accurate, and logically coherent. The system currently integrates web search and specialized databases like ChEMBL and UniProt. It can also leverage advanced specialized models as tools like AlphaFold, tested in select research collaborations.

DeepMind frames it as "one of the first examples of a reliable multi-agent system for structured scientific thinking."

## Validating Co-Scientist in the lab

Collaborated with global experts over the past year. Also previewing an enterprise-grade version with organizations including Daiichi Sankyo, Bayer Crop Science, and the US National Laboratories (Genesis Mission). Reported lab results (vendor-reported, via collaborators):

- **Liver fibrosis** (Gary Peltz, Stanford): highlighted overlooked drug-repurposing candidates, including one that successfully blocked 91% of a scarring-linked response in lab tests (published in Advanced Science).
- **ALS** (Ritu Raman, MIT; Ryan Flynn): helped digest literature, propose testable ideas, spark collaboration on RNA-based approaches.
- **Cellular aging** (Omar Abudayyeh, Jonathan Gootenberg): proposed novel genetic leads shown to rejuvenate cells in lab tests; cut screening-dataset analysis from months to days.
- **Metabolic liver disease** (Filippo Menolascina, Edinburgh): highlighted disease mechanisms and drug combinations.
- **Infectious disease** (Clare Bryant, Cambridge): narrowed the hunt to specific amino acids.
- **Aging biology** (Calico Life Sciences): generated a novel hypothesis about the integrated stress response later confirmed in the lab.

## Developing agentic tools with the scientific community

Developed with researchers from over 100 institutions. Underwent internal and external safety evaluations, including independent evaluations for misuse in CBRN domains; custom safety classifiers flag unethical research goals.

Note (from DeepMind): Co-Scientist is intended to be a partner in research, not a replacement for scientific or clinical expertise.

Acknowledgements include Demis Hassabis, Jeff Dean, Oriol Vinyals, Koray Kavukcuoglu, Pushmeet Kohli, Sundar Pichai.
