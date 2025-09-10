---
title: "Two publishers and three authors fail to understand what “vibe coding” means"
source: "https://simonwillison.net/2025/May/1/not-vibe-coding/"
author:
  - "[[Simon Willison]]"
published:
created: 2025-06-19
description: "Vibe coding does not mean “using AI tools to help write code”. It means “generating code with AI without caring about the code that is produced”. See Not all AI-assisted …"
tags:
  - "clippings"
---
## Summary
Simon Willison expresses strong frustration with two upcoming books that misinterpret the term \\"vibe coding.\\" He clarifies that \\"vibe coding,\\" as coined by Andrej Karpathy, means generating code with AI without caring about the code produced, primarily for \\"throwaway weekend projects.\\" In contrast, the books by Gene Kim & Steve Yegge and Addie Osmani define it as using AI tools to build \\"production-grade software\\" or integrating AI into professional workflows, which Willison argues is a fundamental misunderstanding. He laments this \\"semantic diffusion\\" because it squanders the potential for a valuable book on *actual* vibe coding, which could empower non-developers to automate tasks safely and effectively without needing to learn traditional programming.

## Key Points
-   **Definition of Vibe Coding:** As coined by Andrej Karpathy, \\"vibe coding\\" means generating code with AI while **forgetting that the code even exists**, often accepting AI suggestions without review, and is suitable for **throwaway weekend projects**, not production code.
-   **Misinterpretation by Books:** Two forthcoming books, *Vibe Coding* by Gene Kim and Steve Yegge, and *Vibe Coding: The Future of Programming* by Addie Osmani, incorrectly define it as using AI for building production-grade software or integrating AI into professional engineering workflows.
-   **Author's Frustration:** Simon Willison is highly critical of this misinterpretation, calling it an \\"embarrassing mistake\\" and an example of \\"semantic diffusion\\" where a clear term is misused shortly after its coining.
-   **Missed Opportunity:** This misuse prevents the term from being applied to its true potential: teaching non-developers how to use AI tools responsibly to automate personal tasks without learning to code, which the author believes is a significant market and societal benefit.

---

https://simonwillison.net/2025/May/1/not-vibe-coding/
# Original Content

1st May 2025

**Vibe coding** does not mean “using AI tools to help write code”. It means “generating code with AI without caring about the code that is produced”. See **[Not all AI-assisted programming is vibe coding](https://simonwillison.net/2025/Mar/19/vibe-coding/)** for my previous writing on this subject. This is a hill I am willing to die on. I fear it will be the death of me.

I just learned about not one but *two* forthcoming books that use vibe coding in the title and abuse that very clear definition!

**Vibe Coding** by Gene Kim and Steve Yegge (published by IT Revolution) carries the subtitle “Building Production-Grade Software With GenAI, Chat, Agents, and Beyond”—exactly what vibe coding is not.

**Vibe Coding: The Future of Programming** by Addie Osmani (published by O’Reilly Media) likewise talks about how professional engineers can integrate AI-assisted coding tools into their workflow.

I fear it may be too late for these authors and publishers to fix their embarrassing mistakes: they’ve already designed the cover art!

![[03_resources/attachments/7dad388056f196312e5de6b51f46a36e_MD5.jpg]]

I wonder if this a new record for the time from a term being coined to the first published books that use that term entirely incorrectly.

Vibe coding was only coined by Andrej Karpathy on February 6th, 84 days ago. I will once again quote [Andrej’s tweet](https://twitter.com/karpathy/status/1886192184808149383), with my own highlights for emphasis:

> There’s a new kind of coding I call “vibe coding”, where you fully give in to the vibes, embrace exponentials, and **forget that the code even exists**. It’s possible because the LLMs (e.g. Cursor Composer w Sonnet) are getting too good. Also I just talk to Composer with SuperWhisper so I barely even touch the keyboard.
> 
> I ask for the dumbest things like “decrease the padding on the sidebar by half” because I’m too lazy to find it. I “Accept All” always, I don’t read the diffs anymore. When I get error messages I just copy paste them in with no comment, usually that fixes it. The code grows beyond my usual comprehension, I’d have to really read through it for a while. Sometimes the LLMs can’t fix a bug so I just work around it or ask for random changes until it goes away.
> 
> **It’s not too bad for throwaway weekend projects, but still quite amusing**. I’m building a project or webapp, but it’s not really coding—I just see stuff, say stuff, run stuff, and copy paste stuff, and it mostly works.

Andrej could not have stated this more clearly: vibe coding is when you **forget that the code even exists**, as a fun way to build **throwaway projects**. It’s not the same thing as using LLM tools as part of your process for responsibly building production code.

I know it’s harder now that tweets are longer than 480 characters, but it’s vitally important you **read to the end of the tweet** before publishing a book about something!

#### Now what do we call books on about real vibe coding?

This is the aspect of this whole thing that most disappoints me.

I think there is a real need for a book on *actual* vibe coding: helping people who are *not* software developers—and who don’t want to become developers—learn how to use vibe coding techniques [safely, effectively and responsibly](https://simonwillison.net/2025/Mar/19/vibe-coding/#when-is-it-ok-to-vibe-code-) to solve their problems.

This is a rich, deep topic! Most of the population of the world are never going to learn to code, but thanks to vibe coding tools those people now have a path to building custom software.

Everyone deserves the right to automate tedious things in their lives with a computer. They shouldn’t have to learn programming in order to do that. **That** is who vibe coding is for. It’s not for people who are software engineers already!

There are so many questions to be answered here. What kind of projects can be built in this way? How can you avoid the traps around security, privacy, reliability and a [risk of over-spending](https://twitter.com/leojr94_/status/1901560276488511759)? How can you navigate the jagged frontier of things that can be achieved in this way versus things that are completely impossible?

A book for people like that could be a genuine bestseller! But because three authors and the staff of two publishers didn’t read to the end of the tweet we now need to find a new buzzy term for that, despite having the *perfect* term for it already.

I’m fully aware that I’ve lost at this point— [Semantic Diffusion](https://simonwillison.net/2025/Mar/23/semantic-diffusion/) is an unstoppable force. What next? A book about prompt injection that’s [actually about jailbreaking](https://simonwillison.net/2024/Mar/5/prompt-injection-jailbreaking/)?

I’d like the publishers and authors responsible to at least understand how much potential value—in terms of both helping out more people and making more money—they have left on the table because they didn’t read all the way to the end of the tweet.

**Next:**[Feed a video to a vision LLM as a sequence of JPEG frames on the CLI (also LLM 0.25)](https://simonwillison.net/2025/May/5/llm-video-frames/)

**Previous:**[Understanding the recent criticism of the Chatbot Arena](https://simonwillison.net/2025/Apr/30/criticism-of-the-chatbot-arena/)