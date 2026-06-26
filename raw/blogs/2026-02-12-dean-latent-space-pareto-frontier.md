# RAW CAPTURE — immutable

- **source_url:** https://www.latent.space/p/jeffdean
- **title:** Owning the AI Pareto Frontier — Jeff Dean
- **speaker:** Jeff Dean (Chief Scientist, Google DeepMind & Google Research)
- **hosts:** Shawn Wang (swyx) + Alessio Fanelli — Latent Space podcast
- **published:** 2026-02-12
- **captured:** 2026-06-22 via web_fetch (full verbatim auto-transcript; minor ASR garbles in proper nouns/numbers)
- **note:** Verbatim Dean quotes extracted from the published full transcript, grouped by theme with original timestamps. Host turns omitted except where needed for context.

---

## Pareto frontier framing
- [00:01:04] "it's not just one thing. It's like a whole bunch of things up and down the stack... to help make [us] able to make highly capable large models, as well as... software techniques to get those large model capabilities into much smaller, lighter weight models that are... much more cost effective and lower latency, but still... quite capable for their size."
- [00:02:03] "we always want to have models that are at the frontier or pushing the frontier because... that's where you see what capabilities now exist that didn't exist at the sort of slightly less capable last year's version... At the same time... we want to do is always have kind of a highly capable sort of affordable model that enables a whole bunch of... lower latency use cases... It's not like an either or choice."

## Distillation
- [00:03:52] "distillation was originally motivated because we... had a very large image data set... 300 million images... if you create specialists for different subsets of those image categories... train on an enriched stream of data after you do pre-training... You get much better performance. If you then treat that whole set of maybe 50 models you've trained as a large ensemble, but that's not a very practical thing to serve... distillation really came about from the idea of... squish it into something that actually fits in a form factor that you can actually serve."
- [00:06:01] "one of the key advantages of distillation is that you can have a much smaller model and you can have a very large... training data set... because you're now getting the logits from the much larger model in order to sort of coax the right behavior out of the smaller model that you wouldn't otherwise get with just the hard labels... you can get... very close to your largest model performance with distillation approaches."
- [00:06:01] "for multiple Gemini generations now, we've been able to make the sort of flash version of the next generation as good or even substantially better than the previous generation's pro. And... we're going to keep trying to do that because that seems like a good trend to follow."
- [00:07:12] "we have a lot of different kinds of models. Some are internal ones that are not necessarily meant to be released or served. Some are... our pro scale model and we can distill from that as well into our Flash scale model."

## Flash / efficiency / latency
- [00:08:10] "one of the things that is quite nice about the Flash model is not only is it more affordable, it's also a lower latency. And... latency is actually a pretty important characteristic for these models because we're going to want models to do much more complicated things that are going to involve... generating many more tokens... not just write me a for loop, but like write me a whole software package to do X or Y or Z."
- [00:09:59] "If your distribution of what people are asking... the models to do is stationary... But... as the models become more capable, people ask them to do more... now... can you analyze all the... renewable energy deployments in the world and give me a report on solar panel deployment... That's a... more complicated task than people would have asked a year ago. And so you are going to want more capable models to push the frontier."

## Benchmarks
- [00:11:26] "the best kinds of benchmarks are ones where the initial scores are like 10 to 20 or 30%, maybe, but not higher... once it hits kind of 95%... you get very diminishing returns... it's either the case that you've now achieved that capability, or there's also the issue of leakage in public data... we have a bunch of held out internal benchmarks... where we know that wasn't represented in the training data at all."

## Long context / "illusion of attending to trillions of tokens"
- [00:15:01] "long context is useful, but it's way too short today... what you would really want is, can I attend to the internet while I answer my question?... I [don't] think that's going to be solved by purely scaling the existing solutions, which are quadratic... if you could give the illusion that you can attend to trillions of tokens, that would be amazing... on a personal Gemini level, you could attend to all of your personal state with your permission... your emails, your photos, your docs, your plane tickets."
- [00:20:47] "you're going to attend to trillions of tokens, but you're going to want to identify... what are the 30,000 ish documents... And then how do you go from that into what are the 117 documents I really should be paying attention to... the final model is the thing that looks [at] the 117 things... that is really enables you to give the illusion of attending to trillions of tokens." (search-ranking analogy)

## Multimodality / AI for science
- [00:16:55] "it's also really useful to have Gemini know about non-human modalities... Like LIDAR sensor data from... Waymo vehicles or... robots or... various kinds of health modalities, x-rays and MRIs and imaging and genomics information... there's probably hundreds of modalities of data... even if you haven't trained on all the LIDAR data or MRI data... at least including a little bit of it is actually quite useful... it [tells] the model that this is a thing."
- [00:18:36] "Vision and Motion are quite important things... there's a reason evolution has evolved eyes like 23 independent ways, because it's such a useful capability for sensing the world around you."

## Energy / picojoules / batching / hardware co-design
- [00:32:09] "how much state will you need to bring in from memory... how expensive is that data motion relative to the cost of... an actual multiply in the matrix multiply unit? And that cost is actually really, really low... depending on your precision... it's like sub one picojoule."
- [00:32:52] "it's all going to be about energy and how do you make the most energy efficient system... moving data from the SRAM on the other side of the chip... can be... a thousand picojoules... this is why your accelerators require batching. Because if you move... the parameter of a model from SRAM... into the multiplier unit, that's going to cost you a thousand picojoules. So you better make use of that... many, many times... that's where the batch dimension comes in."
- [00:35:57] "we have a lot of interaction between... the TPU chip design architecture team and the... higher level modeling... experts, because you really want to... co-design what should future TPUs look like based on where we think the... ML research puck is going... a hardware designer... is trying to design a chip starting today and that design might take two years before it even lands in a data center... So you're trying to predict two to six years out [what] ML computations [people] will want to run."
- [00:37:12] "sometimes you can put in speculative features that maybe won't cost you much chip area, but if it works out, it would make something... 10 times as fast. And if it doesn't work out, well, you burned a little bit of tiny amount of your chip area."
- [00:38:43] "I'm a big fan of very low precision because... that saves you a tremendous amount of time... it's picojoules per bit that you're transferring and reducing the number of bits is a really good way to... reduce that... people have gotten a lot of... mileage out of having very low bit precision things, but then having scaling factors that apply to a whole bunch of those... weights."
- [00:39:50] "speculative decoding is a way that you can get... [you] predict eight tokens out and that enables you to... increase the effective batch size... by a factor of eight... and then you maybe accept five or six of those tokens. So you get a five X improvement in the amortization of moving weights... into the multipliers."

## Unified vs specialized / symbolic / "era of unified models"
- [00:47:02] "humans manipulate symbols, but we probably don't have like a symbolic representation in our heads... We have some distributed representation that is neural net like... So it never made sense to me to have like completely separate... discrete... symbolic things, and then a completely different way of... thinking about those things."
- [00:48:06] "switching to a single unified model... is roughly the production model with a little bit more inference budget... it shows you that the capabilities of that general model have improved dramatically... now you don't need the specialized model... I think now the era of unified models that do everything is really upon us." (re: IMO going from AlphaProof/AlphaGeometry to one Gemini)
- [00:49:39] "general models... will win out over specialized ones in most cases."

## Knowledge vs reasoning / retrieval as a tool
- [00:50:38] "you do want the model to be most effective at reasoning if it can retrieve things... having the model devote precious parameter space to remembering obscure facts that could be looked up is actually not the best use of that parameter space... combining retrieval with... reasoning and making the model really good at doing multiple stages of retrieval... is going to be a... pretty effective way of making the model seem much more capable."
- [00:52:01] "we're not going to train Gemini on my email. Probably we'd rather have a single model that... we can then use... being able to retrieve from my email as a tool and have the model reason about it."

## Vertical / modular models
- [00:52:37] "vertical models are interesting... you want them to start from a pretty good base model, but then you can... [enrich] the data distribution for that particular vertical domain... some combination of specialized models, maybe more modular models... it'd be nice to have... those 200 languages, plus this awesome robotics model, plus this awesome healthcare... module that all can be knitted together to work in concert."

## RL on non-verifiable domains / capability leaps
- [00:42:21] "how do you get RL to work for non-verifiable domains? I think it's a pretty interesting open problem... the improvements that you're seeing in both math and coding... if we could apply those to other less verifiable domains... that would really make the models improve quite a lot."
- [00:44:56] "two years ago, we were struggling with GSM 8K problems... 'Fred has two rabbits. He gets three more rabbits. How many rabbits does he have?' That's a pretty far cry from the kinds of mathematics that the models can [do], and now you're doing IMO and Erdős problems in pure language... a really, really amazing jump in capabilities in... a year and a half."

## Origin of Gemini (the one-page memo)
- [01:07:41] "I actually wrote a one-page memo saying we were being stupid by fragmenting our resources... within Google Research... on large language models... multimodal models in other parts of brain... And then Legacy DeepMind had... Chinchilla models and Flamingo models... I said, this is just stupid. Why don't we combine things and have one effort to train an awesome single unified model that is multimodal from the start... And that was the origin of the Gemini effort."
- [01:08:58] "these two organizations really are like twins... there's also the NASA interpretation of the early Gemini project being an important thing on your way to the Apollo project. So it seemed like a good name. Twins coming together."

## AI agents / coding / "50 interns" / crisp specification
- [01:10:07] "the coding tools are... getting vastly better... you can sort of delegate... pretty complex things to these tools... there's going to be more of a style of having lots of independent... software agents off doing things on your behalf... if you have a team of 50 interns, how would you manage that if they were people?... it's not, do you want 50 interns? You might, if they're really good."
- [01:12:25] "that is probably within the realm of possibilities that lots of people could have 50 interns... you would probably want them to form small sub teams, so you don't have to interact with 50 of them. You can interact with five... teams."
- [01:14:26] "whenever people were taught how to write software, they were taught that it's really important to write specifications super clearly, but no one really believed that... if you specify what software you want the agent to write for you, you'd better be pretty darn careful... people will get really good at crisply specifying things rather than leaving things to ambiguity. And that is actually probably not a bad thing... being able to crisply specify what it is you want is going to be really important."

## Predictions
- [01:21:29] "let me make two predictions... a personalized model that knows you and knows all your state and is able to retrieve over all state you have access to, that you opt into is going to be incredibly useful... can something attend to everything I've ever seen?... I think... more and more specialized hardware is going to enable much lower latency models and much more capable models for affordable prices."
- [01:22:36] "you could do many more parallel rollouts. You could generate way more code... being able to do that at 10,000 tokens per second would be awesome."
- [01:22:58] "it may not end up with 10,000 tokens of code... It may be a thousand tokens of code... with 9,000 tokens of reasoning behind it, which would actually be probably much better code to read."
- [01:20:52] "you would use DeepThink all the time if it weren't for cost and latency... if the latency improvement was 20X... there's no reason you wouldn't want that. But... then you'd probably have a model that is even better. That would take you 20X longer, even on that new hardware."
- [00:59:22] "I did an undergrad thesis on... parallel neural network training... back in 1990... I always felt... they were the right abstraction... but we just needed way more compute... When I started working on neural nets at Google in... late 2011... I really just felt like we should scale up the size of neural networks we can train using... large amounts of parallel computation."
