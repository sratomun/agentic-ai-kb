---
type: source
source_type: news
title: Anthropic Disables Fable 5 & Mythos 5 After U.S. Export-Control Directive
outlet/authors: Fortune / Jeremy Kahn
url: https://fortune.com/2026/06/13/anthropic-disables-fable-mythos-export-controls-national-security-threat/
date: 2026-06-12
ingested: 2026-06-21
depth: full-text
tags: [frontier-models, export-control, regulation, geopolitics, anthropic, national-security]
---

# Anthropic Disables Fable 5 & Mythos 5 After U.S. Export-Control Directive

**Why it matters:** The U.S. government just used national-security export controls to force a frontier lab to pull its top models for *all* users — including foreign nationals inside the U.S. and the lab's own non-citizen employees. For a senior AI exec running global operations from Brazil, this is the concrete version of a risk that used to be theoretical: access to the best models is now a geopolitical lever, and "deployed everywhere" is no longer a safe planning assumption for agent reasoning capability across borders.

## What happened
Late Friday (received 5:21 pm ET, June 12, 2026 per Anthropic's blog post; Fortune published June 13), the U.S. Commerce Department invoked national-security export controls to bar Anthropic from distributing its newest models — Fable 5 and Mythos 5 — to any foreign national. Because the directive covered anyone outside the U.S. *and* any foreign national inside it (including Anthropic's own non-citizen staff), Anthropic said it had no choice but to disable the models entirely. Less powerful Claude models, including Claude Opus 4.8, were unaffected. Anthropic called the action "a misunderstanding" and said it is working to restore access.

## Details (numbers, names, dates)
- **Models pulled:** Fable 5 (built on the underlying Mythos 5 model) and Mythos 5; all access disabled. Claude Opus 4.8 and other lesser Claude models unaffected.
- **Stated trigger:** Officials told Anthropic the decision followed discovery of a technique to bypass Fable 5's safeguards — guardrails designed to block access to Mythos's powerful cybersecurity capabilities.
- **Anthropic's rebuttal:** It argues the jailbreak is narrow (unlocks Mythos cybersecurity capability in one specific instance, not universally) and that the same technique could elicit similar capability from other public models, including OpenAI's GPT-5.5, which face no comparable controls. It says recalling a model deployed "to hundreds of millions of people" over a narrow jailbreak would, if applied industry-wide, "essentially halt all new model deployments for all frontier model providers." It maintains the government should be able to block unsafe deployments via a process that is "transparent, fair, clear, and grounded in technical facts," which this was not.
- **Corporate stakes:** Anthropic confidentially filed for an IPO earlier in June 2026; a recent round valued it at $965 billion. Fortune notes the decision could dampen investor enthusiasm.
- **Political backdrop:** In February, President Trump ordered federal agencies to stop using Anthropic models after it refused Pentagon contract terms allowing use "for any lawful purpose" (Anthropic sought carve-outs against autonomous weapons and mass domestic surveillance). In early March the Pentagon labeled Anthropic a "supply chain risk," barring military and defense-contractor use; Anthropic is challenging that in federal court. Advisors David Sacks and Emil Michael have publicly attacked the company; Sacks called it "woke," "leftist," and engaged in "regulatory capture."
- **Reaction:** Policy expert Dean Ball called it "cartoonish" and questioned an administration that would export chips to China but ban Britons from top U.S. models. Cybersecurity researcher Peter Girnus: "If you describe your product as a munition in every press release, eventually a government takes you at your word." Gary Marcus warned it could push Chinese-born researchers back to China and make U.S. AI firms look like a risky bet. Ball also speculated AI-safety proponents might welcome a de facto slowdown.

## So what
Two planning takeaways. First, model availability is now a sovereign-risk variable: an enterprise standardizing agent reasoning on a single frontier model can have that capability yanked overnight by export action, and non-U.S. staff/operations (Brazil included) are squarely in the blast radius — multi-model fallback and graceful degradation stop being nice-to-haves. Second, the "munitions" framing matters: labs that market frontier capability as dangerous are handing regulators the legal hook to restrict it, which will keep injecting unpredictability into vendor roadmaps and IPO valuations. Track whether access is restored, whether Commerce formalizes a repeatable process, and whether peers (OpenAI/GPT-5.5) get pulled into the same net.

**Connects to:** [[anthropic]] [[frontier-model-governance]]
**Raw:** `raw/news/2026-06-12-anthropic-export-controls.fulltext.md`
