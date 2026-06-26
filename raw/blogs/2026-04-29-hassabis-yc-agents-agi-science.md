---
source: Y Combinator — "How to Build the Future" (live episode)
title: "Demis Hassabis: Agents, AGI & The Next Big Scientific Breakthrough"
author: Demis Hassabis (in conversation with Garry Tan, YC)
url: https://www.youtube.com/watch?v=JNyuX1zoOgU
transcript_source: https://www.textpurr.com/transcript/demis-hassabis-agents-agi-the-next-big-scientific-breakthrough
date: 2026-04-29
captured: 2026-06-22
note: Immutable full-text capture (third-party transcript of the YC YouTube video). Do not edit. Timestamps preserved.
---

# Demis Hassabis: Agents, AGI & The Next Big Scientific Breakthrough (YC, How to Build the Future)

Live episode of YC's "How to Build the Future." Demis Hassabis in conversation with Garry Tan. April 29, 2026. Runtime ~40:57. Transcript via TextPurr of YouTube video JNyuX1zoOgU.

---

**[00:00] Hassabis:** Continual learning, long-term reasoning, some aspects of memory, these are still unsolved. I think all of these are going to be required for AGI. Depending on what your AGI timeline is, you know, mine's like 2030 or something like this, then if you start off on a deep tech journey today, you have to just consider AGI appearing in the middle of that journey.

**[00:21] Hassabis:** It's not bad, necessarily, but you have to take that into account. You have to have an active system that can actively solve problems for you to get to AGI. So, agents are that path, and I think we're just getting going.

**[00:39] Tan (intro):** Demis Hassabis has had one of the most unusual careers in tech. He was a chess prodigy as a kid, then designed his first hit video game, Theme Park, at 17. He then went back to school, got a PhD in cognitive neuroscience, published foundational work on how memory and imagination work in the brain, and then in 2010 co-founded DeepMind with one mission: solve intelligence. … AlphaGo beat a world champion at Go. AlphaFold cracked protein structure prediction, a 50-year grand challenge in biology, and they gave it away for free to every scientist on Earth. That work won him the Nobel Prize in chemistry last year. Today, Demis leads Google DeepMind, where he's building Gemini and pushing toward the same goal he set when he was a teenager: artificial general intelligence.

**[01:53] Tan:** You've been thinking about AGI longer than almost anyone. When you look at the current paradigm, large-scale pre-training, RLHF, chain of thought, how much of the final architecture for AGI do you think we already have, and what's fundamentally missing right now?

**[02:20] Hassabis:** The components that you just mentioned, I'm pretty sure will be part of the final architecture for AGI. … I can't see a world in which we'll sort of realize in a couple of years this was a dead end. That doesn't make sense to me. But, there still might be one or two things missing on top of what we already know works.

**[02:50] Hassabis:** So, continual learning, long-term reasoning, some aspects of memory, these are still unsolved. And how to get the systems to be more consistent across the board. I think all of these are going to be required for AGI.

**[03:04] Hassabis:** Now, it might be that the existing techniques can just scale up to that with some incremental innovation. But, it could be that there's still one or two big ideas left that need to be cracked. I don't think it's more than one or two if they are out there. And I think, you know, my betting is about 50/50 if that's the case. So, of course at Google DeepMind we work on both those things.

**[03:29] Tan:** … this idea of continual learning is so interesting because like you know, right now we're sort of cobbling it together with duct tape, you know, these dream cycles at night and things like that.

**[03:47] Hassabis:** Yeah. It's pretty cool the dream cycles, and we used to think about this with consolidation with episodic memory. It's actually what I studied for my PhD is how the hippocampus works and integrates, you know, new knowledge gracefully into the existing knowledge base. So, the brain does that amazingly well. It does it through, you know, during sleep, especially things like REM sleep, replaying back episodes that are important so that you can learn from it.

**[04:13] Hassabis:** In fact, our very first Atari program, DQN, one of the ways it was able to master Atari games was by doing experience replay. So, we sort of borrowed that from neuroscience and replayed successful trajectories many times … that's way back in 2013 now in the dark ages of AI. … and I agree with you, we're kind of using duct tape right now.

**[04:38] Hassabis:** [On just shoving everything in the context window] this seems a bit unsatisfying, right? … even though you potentially could have, you know, millions or tens of millions size context window or memory, and it can be perfect, there's still a cost to looking it up and finding the right thing that's actually relevant for the specific decision you've got to make right now. … I think there's actually a lot of room for innovation in areas like memory.

**[05:20] Hassabis:** If you think about the context window is sort of equivalent to working memory. … We got a million or you know, 10 million context windows, but the problem is that we're trying to store everything in that. … It's pretty brute force currently, and that doesn't seem right. And then the problem is if you're now trying to process live video … a million tokens isn't that much. It's only like 20 minutes. So, actually you need more if you want something that's going to understand what's going on in your life over maybe a month or two.

**[06:08] Tan:** DeepMind has historically leaned into reinforcement learning and search, AlphaGo, AlphaZero, and MuZero. How much of that philosophy is actually embedded in how you're building Gemini today? Is RL still underrated?

**[06:23] Hassabis:** Yeah, I think potentially it is. It sort of goes in waves. … we've worked on agents since the beginning of DeepMind. … systems that are able to accomplish goals on their own and make active decisions and make plans. … the question is can you generalize those models to be world models or models of language, not just models of simple games or even complex games? … you can think of a lot of the things we're doing today, all the leading models with thinking modes and chain of thought reasoning, as aspects of what was sort of pioneered with AlphaGo coming back now.

**[07:27] Hassabis:** … we're sort of relooking at some of those old ideas at scale today in a more general way. Including things like Monte Carlo tree search and other ways of augmenting the RL … a lot of those ideas both from AlphaGo and AlphaZero are really, really relevant to where we are with today's foundation models. And I think a lot of that is what we're going to see of the advances the next few years.

**[07:58] Tan:** … we're also seeing distillation working, and then smaller models can be like quite a bit faster. … you guys have incredible flash models that are like … 95% as good as the frontier and at like 1/10 the price. Is that right?

**[08:22] Hassabis:** I think that's one of our core strengths. … you have to build the biggest models to have the frontier capabilities. But, one of our biggest strengths has been distilling and packing that power into smaller and smaller models very quickly. Obviously, we invented the kind of distillation process and people like Jeff and Oriol and others, and we're still world experts in that. … we've got to serve the biggest probably AI surfaces there are.

**[08:56] Hassabis:** … search with AI overviews, then there's the Gemini app, and now increasingly every single product at Google has … Maps and YouTube and so on … billions of users, more than a dozen billion user products, and they have to be served extremely fast … So, that gives us a really important incentive to make these Flash and even smaller models, Flash-Lite models, extremely efficient.

**[09:35] Tan:** … could a 50B or 400B model be as smart as like a frontier model is today?

**[09:48] Hassabis:** Yeah, I don't think we've got to any kind of … informational limit. … the assumption we make is that, you know, a year later after one of our leading pro models or frontier models goes out, half a year later, a year later you'll have them in the really tiny, almost edge models. … you also see some of that goodness in our Gemma models …

**[10:39] Tan:** … engineers can do like 500 to 1,000 times the amount of work that they were doing like 6 months ago … 1,000x the work that a Google engineer from the 2000s was doing.

**[11:04] Hassabis:** I think it's very exciting. … the small models have many uses. One is obviously cost, but the speed can allow … if you think about coding even or other things, you can iterate a lot faster also, especially if you're collaborating with the system. … like 95%, 90%, but that's plenty good enough and actually gain back more than the 10% on the iteration speed.

**[11:34] Hassabis:** And then the other big thing I think is running these things on the edge again for efficiency reasons, but also for privacy and security reasons, too. … robots in your house. I think you're going to want very efficient, very powerful local models, which maybe are orchestrated … with some bigger models, frontier models that are in the cloud, but you only delegate to that in certain circumstances. … process all of the audio visual feed, let's say, locally and that stays local.

**[12:31] Tan:** … models currently stateless, but … what would the developer experience even be like for someone who's using a continual learning model?

**[12:46] Hassabis:** I think that not having continual learning currently is one of the things holding back agents from doing full tasks. … they're really useful for aspects of tasks right now and you can patch them together and do some really cool things, but they don't adapt well with the context that you're in. And I think that's the missing piece for them being really kind of fire and forget … they need to be able to learn about the specific context that you're going to put them in. So, I think we have to crack that to get full general intelligence.

**[13:25] Tan:** Where are we on reasoning? … models can do really impressive chain of thought now, but they still fail on things a smart undergrad wouldn't.

**[13:38] Hassabis:** There's a lot of innovation left in the thinking paradigms, I would say. … I think we're doing fairly simplistic things, fairly brute force. One could imagine … a lot of scope, for example, in monitoring the chain of thought, maybe interjecting midway through a thought process. I often get the impression with our systems and our competitor systems that they're almost overthinking. They're almost getting into sort of loops of things.

**[14:05] Hassabis:** Like, one thing I sometimes like to do is play chess against Gemini. And … all the leading foundation models are pretty poor at games … sometimes it will consider a move, it will realize it's a blunder, but it can't find anything better, so it kind of goes back to that move and does it anyway.

**[14:42] Hassabis:** So … you just shouldn't be seeing that happening in a very precise reasoning system. … it may only be one or two tweaks that are required to fix those kind of gaps … And that's why you get this kind of jagged intelligence.

**[15:01] Hassabis:** On the one hand, it can solve gold medal problems in IMO, which is super hard, but on the other hand … it can still make basic elementary maths errors if you pose the question in a certain way … there's just something to me about the almost an introspection about its own thought process that I feel like there's something maybe missing there.

**[15:32] Tan:** What does DeepMind's internal research tell you about where agent capabilities actually are right now versus … the hype out there?

**[15:39] Hassabis:** I agree with you. I think we're just at the beginning. You have to have an active system that can actively solve problems for you to get to AGI. That was always clear to us. So, agents are that path. And I think we're just getting going. … how do we best work …

**[16:01] Hassabis:** … how do you incorporate it into your workflow in a way that isn't just sort of a nice-to-have, but actually starting to do fundamental things? My impression is at the moment we're all experimenting … but we're only in maybe the last couple of months starting to find the really valuable places. And the technology is probably only getting good enough for that to be the case …

**[16:31] Hassabis:** I'd often wonder … I see a lot of people working on like setting off, you know, dozens of agents for like 40 hours, but I'm not sure I've seen the output of that yet quite justify that level of input going in. But I think it will come. So, I still think we're in the experimentation phase. We haven't seen a AAA game that tops the app store charts that was sort of live coded yet, right?

**[16:56] Hassabis:** I can do a prototype of Theme Park in half an hour now, which took me 6 months back when I was 17. … but it still needs craft and … human sort of soul into it and taste. … why haven't we seen a kid making a hit game that sells 10 million copies … something's still somehow missing. Maybe it's to do with the process or maybe it's to do with the tools. … Which I think will come in the next 6 to 12 months.

**[17:56] Tan:** … I don't think we'd see autonomous first. We would actually probably see people in this room operating at 1,000x …

**[18:07] Hassabis:** That's what you should see first. … there'll be like games companies or … other types of companies that have built some kind of best-selling app, best-selling game using these tools. That's what you should see first. And then more of that will get automated.

**[18:31] Hassabis:** … if we look at the things we've done like AlphaGo … move 37 in game two. … I was waiting for a moment like that to start the science projects like AlphaFold. We started AlphaFold like the day we got back from Seoul, which is 10 years ago now.

**[19:01] Hassabis:** But it's not enough to come up with move 37. … can it invent Go? That's what I … want a system that can invent Go if you give it a high-level description … a game you can learn the rules of in 5 minutes, but it takes many lifetimes to master. … clearly today's systems I think can't do that. So, the question is why? And I think there's something still missing there.

**[19:44] Hassabis:** [If someone in this room makes it] Then the answer would be there's nothing missing. It just was the way we were using the systems. And that might actually be the answer. It might be that today's systems are capable of that with a brilliant enough creative person using it … to almost be at one with the tools. … combine that with proper deep creativity. Something more incredible could be done.

**[20:20] Tan:** Switching gears to open source … open weights … the recent release of Gemma …

**[20:43] Hassabis:** We're huge proponents in general of open source and open science, and you mentioned AlphaFold … we put that all out there for free, and all of our science work even still today we publish in … the big journals. We wanted to create world-leading models for their sizes. … I think it's been like 40 million downloads now just in … two and a half weeks.

**[21:15] Hassabis:** And I also think it's important for there to be Western stacks on open source … a lot of the Chinese models are excellent and they're currently world-leading in open source, and we think Gemma is very competitive for its sizes …

**[21:30] Hassabis:** … there is a question of resources, talent, and compute. … nobody has enough spare compute to just make two … frontier models at maximum size … But also for now, what we've decided is that our edge models, the things we want to use for Android and glasses and robotics, it's best that they're open models because they're vulnerable anyway once you put them out on the surfaces. So they might as well be actually fully open.

**[22:19] Tan:** … Gemini was built multimodal …

**[22:45] Hassabis:** … that's still a slightly underappreciated aspect of the Gemini series, is we started it being multimodal from the start. That made it a little bit more difficult … But I believe we're going to gain from that in the long run. And I think we're seeing that now for things like world model building, so stuff like Genie that we build on top of Gemini.

**[23:11] Hassabis:** I think it's going to be really important for things like robotics. So this is why Gemini robotics … built on multimodal foundation models … We're using it increasingly in things like Waymo.

**[23:31] Hassabis:** But also if you imagine devices and digital assistants that come with you into the real world … on your phone or glasses … It needs to understand the physical world around you and intuitive physics … and I think we're far and away the strongest models on those types of problems.

**[24:00] Tan:** … the cost of inferences are dropping fast. What becomes possible when inference is essentially free …?

**[24:10] Hassabis:** Yeah, I'm not sure inference will ever be essentially free. I mean there's sort of Jevons paradox … you could imagine millions of agents, swarms of agents working together on things. … or single agents or smaller groups of agents thinking in multiple directions and then ensembling that.

**[24:41] Hassabis:** All of that will use up any inference … certainly the energy if we solve fusion or … superconductors or optimal batteries … with material science. Energy costs will be essentially zero, but there'll still be the physical creation of the chips … there'll still be rationing on the inference side.

**[25:24] Tan:** … AlphaFold 3 took us beyond proteins … How close are we to modeling full cellular systems …?

**[25:38] Hassabis:** Well, Isomorphic Labs, which we spun out from DeepMind after we did AlphaFold 2, which is going amazingly well. It's trying to build out … not just AlphaFold … the adjacent biochemistry and chemistry to design the right compounds with the right properties … We'll have some big announcements very soon …

**[26:08] Hassabis:** Eventually you want a whole virtual cell. … a full working simulation of a cell that you can perturb, and then the outputs of that would be close enough to experimental that it's useful. … And I think we're about 10 years away probably from something like a virtual cell …

**[26:38] Hassabis:** … we're working on the DeepMind science side on a virtual nucleus. Cell nucleus first, because it's relatively self-contained. The trick with all of these things is can you pick a slice of the complexity? …

**[27:14] Hassabis:** Then the other issue is just there's not enough data yet. … If we could image a live cell without killing the cell, that would be game-changing obviously, because then you could convert it into a vision problem which we would know how to solve. …

**[28:17] Tan:** … If you had to rank which scientific domain will transform the most dramatically the next 5 years …?

**[28:30] Hassabis:** They're all so exciting … to use AI as the ultimate tool. I always thought AI would be the ultimate tool for science …

**[28:53] Hassabis:** … the way we used to articulate our mission statement … there was two steps to it. Step one was solve intelligence, i.e., build AGI, and then step two was use it to solve everything else. … we did mean that …

**[29:14] Hassabis:** … specifically I was meaning solve other what I call root node problems in science. So areas of science that would unlock whole new branches or avenues of discovery. And AlphaFold is the prototypical example … over 3 million researchers around the world … use AlphaFold now. And I was told by some of my pharma executive friends that almost every drug discovered from now on will have used AlphaFold at some point …

**[29:51] Hassabis:** But, I do think it's just the beginning. … the ones you mentioned, I think we're almost at an AlphaFold one moment … materials, which I think is very exciting, all the way to mathematics.

**[30:23] Hassabis:** … of course, along with that, including the parable of Prometheus, we have to also be careful with how we use that and what we use it for, and also the misuse that can happen with those same tools.

**[30:35] Tan:** … what's the difference between a startup that actually advances the frontier … versus one that's just wrapping an API around a foundation model …?

**[30:49] Hassabis:** … One thing you have to do is obviously intercept where the AI tech is going. … But, I do think there's huge scope for combining where AI is going with some other deep technology area. … whether it's materials or medicine or other really hard areas of science.

**[31:21] Hassabis:** … those kinds of interdisciplinary teams, especially if it involves the world of atoms as well, there's not going to be a shortcut to that at least in the foreseeable future. Those areas are pretty safe from just getting swamped by whatever the next update is to the foundation models. … that's one of the more defensible areas, I would say.

**[31:42] Hassabis:** And I've always loved deep tech … nothing that's really long-lasting and worthwhile is easy. … Obviously, AI was like that back in 2010 when we started out … It was thought to just … we know it doesn't work, kind of thing, is what I was told by investors …

**[32:14] Hassabis:** But, if you have belief and conviction in your idea why it's different this time or what special combination from your background that you have … ideally you're an expert in both those areas, both the machine learning and the other area you're applying it to …

**[32:45] Hassabis:** … you've also got to work in things that you're genuinely passionate about. Like for me, I would have worked on AI no matter what happened. … I would still be working on AI today even if we were still … in a little garage somewhere and it still wasn't quite working.

**[33:24] Tan:** … what makes a scientific domain ripe for an AlphaFold style breakthrough? And is there a pattern, a certain objective function …?

**[33:35] Hassabis:** The way I … should write this up at some point when I have 5 minutes spare, but the lesson I've learned from all the Alpha projects … is I think the techniques we have and the problems I like to look for are great if the situation can be described as a massive combinatorial search space. The more massive, the better in some ways. So, no brute force or special case algorithm will solve it. And that's true of Go moves and of different configurations of proteins …

**[34:10] Hassabis:** And then, you have a clear objective function. … minimizing the free energy in the proteins or winning the game of Go. … And then, enough data and/or a simulator that can generate you lots of in-distribution synthetic data.

**[34:33] Hassabis:** If those things are true, then … you can go a long way into … finding the kind of needle in the haystack … And I think just drug discovery, by the way, is in the same way. … There is a compound out there that would solve this disease if one could find it. … as long as the laws of physics allow it, then the only question is how do you find it in an efficient way …

**[35:13] Tan:** … humans using AI to explore the space of possible hypotheses. How close are we to AI systems that can do genuine scientific reasoning, not just pattern matching …?

**[35:32] Hassabis:** We're close. … we have this system called Co-Scientist, and we have other algorithms like AlphaFold that can go a little bit beyond what the basic Gemini will do. … I've yet to see anything so far … that is a true genuine, you know, massive discovery.

**[36:04] Hassabis:** … I think it's coming. I think it may be related to this earlier thing we discussed about creativity and actually going on beyond the bounds of what's known. So, clearly that's just not pattern matching at that point because there is no pattern to match to. And it's a bit more than extrapolation. It's some kind of analogical reasoning. And I don't think these systems have that, or at least we're not using them in the right way to do that.

**[36:31] Hassabis:** … can it come up with a hypothesis that's really interesting, not just solve one? … even harder … would be to come up with a new set of Millennium Prize problems that were regarded by top mathematicians to be as … deep and meaningful and worthy of a lifetime of study …

**[37:15] Hassabis:** I don't think it's magical, though. I do think these systems will be eventually able to do that. Maybe we're missing one or two things. … sometimes I call it my Einstein test, which is, can you train a system with the knowledge cutoff of 1901 and then will it come up with what Einstein did in 1905, including special relativity … Once that is, then I think we're on the verge of these systems being able to invent something new, truly novel.

**[37:52] Tan:** … What's the thing that you know now about building at the frontier that you wish you'd known at 25?

**[38:18] Hassabis:** … going after hard problems and deep problems is no more difficult in some ways than going after a shallower, simpler, more superficial problem. … given life's very short … you might as well put your life force into something that will really make a difference …

**[38:55] Hassabis:** … I love interdisciplinary work, and I think that's going to be even more prevalent in the next few years in combinations of fields …

**[39:13] Hassabis:** … depending on what your AGI timeline is—mine's like 2030 or something like this—then if you start off on a deep tech journey today, usually you're talking about a 10-year journey … So then now you have to just consider AGI appearing in the middle of that journey. So, what does that mean? …

**[39:47] Hassabis:** … one thing I can see happening is Gemini, Claude, or one of these general systems making use of AlphaFold-like specialized systems as tools. I don't think we're going to have it just in one giant brain because it will have too much regression. If I put all the proteins into Gemini, that wouldn't make sense. … much better I think is to have really good general-purpose tool usage models that will then maybe even train those specific tools, but they would be in a separate system.

**[40:31] Hassabis:** … you need to really take that seriously and imagine what that world would look like, and then build something that would be useful if [AGI] comes in halfway through.
