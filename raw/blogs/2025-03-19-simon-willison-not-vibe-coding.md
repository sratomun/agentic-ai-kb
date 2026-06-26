---
title: "Not all AI-assisted programming is vibe coding (but vibe coding rocks)"
author: Simon Willison
outlet: Simon Willison's Weblog
url: https://simonwillison.net/2025/Mar/19/vibe-coding/
date: 2025-03-19
captured: 2026-06-22
source_type: blog
---

# Not all AI-assisted programming is vibe coding (but vibe coding rocks)

*Full text captured verbatim for the radar. Immutable.*

Vibe coding is having a moment. The term was coined by Andrej Karpathy just a few weeks ago (on February 6th, 2025) and has since been featured in the New York Times, Ars Technica, the Guardian and countless online discussions.

I'm concerned that the definition is already escaping its original intent. I'm seeing people apply the term "vibe coding" to all forms of code written with the assistance of AI. I think that both dilutes the term and gives a false impression of what's possible with responsible AI-assisted programming.

Vibe coding is *not* the same thing as writing code with the help of LLMs!

To quote Andrej's original tweet in full (with Simon's emphasis added):
> There's a new kind of coding I call "vibe coding", where you fully give in to the vibes, embrace exponentials, and **forget that the code even exists**. It's possible because the LLMs (e.g. Cursor Composer w Sonnet) are getting too good. Also I just talk to Composer with SuperWhisper so I barely even touch the keyboard.
>
> I ask for the dumbest things like "decrease the padding on the sidebar by half" because I'm too lazy to find it. I "Accept All" always, I don't read the diffs anymore. When I get error messages I just copy paste them in with no comment, usually that fixes it. The code grows beyond my usual comprehension, I'd have to really read through it for a while. Sometimes the LLMs can't fix a bug so I just work around it or ask for random changes until it goes away.
>
> **It's not too bad for throwaway weekend projects, but still quite amusing**. I'm building a project or webapp, but it's not really coding—I just see stuff, say stuff, run stuff, and copy paste stuff, and it mostly works.

Simon: "When I talk about vibe coding I mean **building software with an LLM without reviewing the code it writes**."

#### Using LLMs for code responsibly is not vibe coding
The job of a software developer is not (just) to churn out code and features. We need to create code that demonstrably works, can be understood by other humans (and machines), and supports continued development in the future. We need to consider performance, accessibility, security, maintainability, cost efficiency. Software engineering is all about trade-offs.

"My golden rule for production-quality AI-assisted programming is that I won't commit any code to my repository if I couldn't explain exactly what it does to somebody else." If an LLM wrote the code, and you reviewed it, tested it thoroughly and could explain how it works to someone else — that's not vibe coding, it's software development. The usage of an LLM is immaterial.

#### Let's not lose track of what makes vibe coding special
Vibe coding grants millions of new people the ability to build their own custom tools without a CS degree — it shaves the steep initial learning curve down to almost flat. It's also the best tool experienced developers have to build intuition for what LLMs can and cannot do (Simon published 80+ vibe-coded experiments).

#### When is it OK to vibe code?
- Projects should be **low stakes** — consider the harm if it has bugs/security holes, especially if others will use it.
- Consider **security** — watch for secrets/API keys; think about data privacy.
- Be a **good network citizen** — outbound requests increase load/cost (Simon likes Claude Artifacts' sandbox).
- Is **your money on the line**? Horror stories of vibe-coded features racking up thousands in usage charges.

#### How do we make vibe coding better?
Safe vibe coding for beginners starts with a sandbox. Claude Artifacts restrict code to a locked-down iframe (approved libraries only, no network requests) — fantastic for safety but limits capability. Plenty of room for innovation; Simon hopes for "a cambrian explosion in tooling."

Don't confuse vibe coding with all other uses of LLMs for code.
