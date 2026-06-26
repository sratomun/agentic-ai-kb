---
type: source
source_type: blog
title: "New prompt injection papers: Agents Rule of Two and The Attacker Moves Second"
author: Simon Willison
outlet: simonwillison.net
url: https://simonwillison.net/2025/Nov/2/new-prompt-injection-papers/
resource: https://simonwillison.net/2025/Nov/2/new-prompt-injection-papers/
date: 2025-11-02
stake: Independent practitioner/educator — minimal commercial stake
ingested: 2026-06-22
tags: [perspective, agent-security, agent-evaluation]
---

# New prompt injection papers: Agents Rule of Two and The Attacker Moves Second

**Blog** · Simon Willison (simonwillison.net) · 2025-11-02 · [link](https://simonwillison.net/2025/Nov/2/new-prompt-injection-papers/)

**The take (attributed):** Willison endorses Meta's **"Agents Rule of Two"** as the best *practical* security advice available today, and reads "The Attacker Moves Second" as fresh evidence that prompt-injection defenses are nowhere near reliable — so build for "no robust defense exists" rather than hope one arrives.

**Stake:** Independent — reviewing others' research, not his own product; he both praises and pushes back on the papers.

## Argument
- **Agents Rule of Two (Meta AI, Oct 31 2025):** "until robustness research allows us to reliably detect and refuse prompt injection, agents must satisfy *no more than two* of the following three properties within a session" — [A] process untrustworthy inputs, [B] access to sensitive systems/private data, [C] change state or communicate externally. Willison: "I like this *a lot*." He notes it improves on his own lethal-trifecta frame: the trifecta only covers *data exfiltration*, whereas adding "changing state" as a property captures "plenty of other, even nastier risks." He also pushes back — the paper marks (untrustworthy input + change state) as "safe," but "that's not right. Even without access to private systems or sensitive data that pairing can still produce harmful results."
- He reads it as another major lab "concluding that prompt injection remains an unsolved problem, and attempts to block or filter them have not proven reliable enough to depend on."
- **The Attacker Moves Second (arXiv 2510.09023, 14 authors incl. OpenAI/Anthropic/Google DeepMind):** broke "12 recent defenses… with attack success rate above 90% for most; importantly, the majority of defenses originally reported near-zero attack success rates." A 500-participant human red-teaming competition ($20k prize fund) "scored 100%, defeating all defenses." Lesson: "static example attacks… are an almost useless way to evaluate these defenses. Adaptive attacks are far more powerful" (gradient-based weakest, RL effective vs black-box, search-based via LLM-generate + LLM-as-judge).
- Where he splits from the paper: it ends optimistically; he doesn't — "Given how totally the defenses were defeated, I do not share their optimism that reliable defenses will be developed any time soon." Net recommendation: the Rule of Two "as the best practical advice for building secure LLM-powered agent systems today in the absence of prompt injection defenses we can rely on."

## Why it matters / where it cuts
Decision-relevant for anyone shipping agents: the empirical state of the art is that published defenses fall to *adaptive* attacks almost completely, so the safe design posture is structural restriction (the Rule of Two / trifecta-avoidance), not filtering. This is the opinion-layer read on the same evidence the radar's [[agent-evaluation]] and [[agent-security]] research carries, and it sharpens [[debate-prompt-injection-solvable]] — the "manage, don't solve" position now has a clean operational rule attached.

## Graph
- **Author:** [[simon-willison]]
- **Concepts:** [[agent-security]] · [[agent-evaluation]] · [[tool-use]]
- **Entities:** [[tool-description-poisoning]] · [[anthropic]] · [[openai]]
- **Debate:** [[debate-prompt-injection-solvable]]
- **Raw:** `raw/blogs/2025-11-02-simon-willison-new-prompt-injection-papers.md`
