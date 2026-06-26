# Introducing ChatGPT agent: bridging research and action

Source: https://openai.com/index/introducing-chatgpt-agent/
Author: OpenAI
Date: July 17, 2025
Category: Product / Release
Captured: 2026-06-22
Vendor stake: OpenAI launching/marketing its own agentic product (ChatGPT agent). Benchmark figures (HLE, FrontierMath, BrowseComp, SpreadsheetBench) are self-reported / OpenAI-elicited, some graded by third parties (e.g. Epoch AI).

---

ChatGPT now thinks and acts, proactively choosing from a toolbox of agentic skills to complete tasks for you using its own computer.

At the core of this new capability is a unified agentic system. It brings together three strengths of earlier breakthroughs: Operator's ability to interact with websites, deep research's skill in synthesizing information, and ChatGPT's intelligence and conversational fluency. It is described as a natural evolution of Operator and deep research.

Example tasks: briefing on upcoming calendar/client meetings using recent news; planning and buying ingredients for a meal; analyzing competitors and building a slide deck — handling complex tasks end-to-end.

## Tools / how it works
ChatGPT agent is equipped with a suite of tools:
- a **visual browser** that interacts with the web through a graphical-user interface
- a **text-based browser** for simpler reasoning-based web queries
- a **terminal**
- **direct API access**
- plus ChatGPT **connectors** (e.g. Gmail, GitHub) so it can access relevant context.

It can fluidly shift between reasoning and action, preserving context across tools on its own virtual computer. Built for interruptible, collaborative workflows: the user stays in control and can take over the browser at any point. Activated via "agent mode" in the tools dropdown for Pro, Plus, and Team users.

## Benchmarks (OpenAI's own framing of SOTA)
- **Humanity's Last Exam:** new pass@1 SOTA at 41.6; rises to 44.4 with an 8-attempt parallel rollout.
- **FrontierMath:** with tool use (terminal for code execution), 27.4% accuracy, outperforming both previous models by a wide margin.
- **BrowseComp:** new SOTA of 68.9%, 17.4 percentage points higher than deep research.
- **SpreadsheetBench:** when given the ability to edit spreadsheets directly (.xlsx), 45.5%, compared to Copilot in Excel's 20.0%.
- Also claims outperformance on DSBench, WebArena, internal investment-banking modeling, and "economically valuable knowledge-work tasks" — comparable to or better than humans in roughly half of cases, beating o3 and o4-mini.

## Safety
"This release marks the first time users can ask ChatGPT to take actions on the web," raising the overall risk profile. Heavy emphasis on prompt-injection defenses (training, monitoring, explicit user confirmation). Model-mistake mitigations: explicit user confirmation, active supervision ("Watch Mode"), proactive refusal of high-risk tasks (e.g. bank transfers). "We've made the decision to treat ChatGPT agent as High Biological and Chemical capabilities under our Preparedness Framework, activating the associated safeguards" — OpenAI's most comprehensive safety stack to date.

## Availability
Pro users 400 messages/month; Plus and Team 40/month; Enterprise/Education later; not yet in EEA/Switzerland. The standalone Operator preview will be sunset.

Tags: Product · Release · ChatGPT · 2025
