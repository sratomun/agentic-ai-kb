# RAW CAPTURE — New prompt injection papers: Agents Rule of Two and The Attacker Moves Second

- **Author:** Simon Willison
- **Outlet:** simonwillison.net
- **URL:** https://simonwillison.net/2025/Nov/2/new-prompt-injection-papers/
- **Date:** 2025-11-02
- **Fetched:** 2026-06-22 (via web_fetch)
- **Format:** paper review (two papers)

## Provenance / framing
Part of his "Prompt injection" series. Reviews two papers: Meta AI's "Agents Rule of Two" (blog, Oct 31 2025) and "The Attacker Moves Second" (arXiv 2510.09023, Oct 10 2025, 14 authors incl. OpenAI/Anthropic/Google DeepMind).

## Key quotes (verbatim)
### Agents Rule of Two (Meta AI)
- The Rule (quoting Meta): "until robustness research allows us to reliably detect and refuse prompt injection, agents **must satisfy no more than two** of the following three properties within a session": [A] process untrustworthy inputs, [B] access to sensitive systems/private data, [C] change state or communicate externally.
- "I like this *a lot*."
- "I've spent several years now trying to find clear ways to explain the risks of prompt injection attacks to developers… It's frustratingly difficult."
- "The one problem with the lethal trifecta is that it only covers the risk of data exfiltration: there are plenty of other, even nastier risks… The Agents Rule of Two neatly solves this, through the addition of 'changing state' as a property."
- "It's also refreshing to see another major research lab concluding that prompt injection remains an unsolved problem, and attempts to block or filter them have not proven reliable enough to depend on."
- Update (his pushback): "the Venn diagram above marks the combination of untrustworthy inputs and the ability to change state as 'safe', but that's not right. Even without access to private systems or sensitive data that pairing can still produce harmful results."

### The Attacker Moves Second
- Paper bypassed "12 recent defenses… with attack success rate above 90% for most; importantly, the majority of defenses originally reported near-zero attack success rates."
- "the 'Human red-teaming setting' scored 100%, defeating all defenses" (500-participant competition, $20,000 prize fund).
- "static example attacks… are an almost useless way to evaluate these defenses. Adaptive attacks are far more powerful."
- Three adaptive techniques: gradient-based (least effective), reinforcement-learning (effective vs black-box), search-based (LLM generate + LLM-as-judge).
- Paper's optimistic conclusion vs Willison's verdict: "Given how totally the defenses were defeated, I do not share their optimism that reliable defenses will be developed any time soon."
- "I think it makes a strong case for Meta's Agents Rule of Two as the best practical advice for building secure LLM-powered agent systems today in the absence of prompt injection defenses we can rely on."

## Tags on the post
definitions, security, openai, prompt-injection, anthropic, nicholas-carlini, paper-review, lethal-trifecta
