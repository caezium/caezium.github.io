#### Source: https://mbuffett.com/posts/programming-advice-younger-self/



# A Bunch of Programming Advice I’d Give To Myself 15 Years Ago


I finally have the feeling that I’m a decent programmer, so I thought it would be fun to write some advice with the idea of “what would have gotten me to this point faster?” I’m not claiming this is great advice for everyone, just that it would have been good advice for me.

## If you (or your team) are shooting yourselves in the foot constantly, fix the gun

I can’t tell you how many times I’ve been on a team and there’s something about the system that’s very easy to screw up, but no one thinks about ways to make it harder to make that mistake.

When I was doing iOS development, used CoreData, and subscribed to changes from a bunch of views. The subscription callback came on the same thread that the change was triggered from. Sometimes that was the main thread, and sometimes it was a background thread. Importantly in iOS development, you can only make UI updates on the main thread, or your app crashes. So a new subscription could be working fine, but then it would break when someone triggered a change from a background thread, or if you add a UI update later on.

This was just something people transparently accepted, and often came up in reviews for newer people on the team. Every now and then, one would slip through, and we’d go add a `DispatchQueue.main.async` when we saw the crash report.

I decided to fix it, and it took ten minutes to update our subscription layer to call subscribers on the main thread instead, which eliminated a whole class of crashes, and a bit of mental load.

I’m not trying to be like “look at these idiots not fixing an obvious issue with the codebase, when it was obvious to me”, because it would have been obvious to anyone who thought about it for a few minutes. These things stick around a weird amount, because there’s never a natural time to address them. When you’re first getting onboarded, you’re not trying to change anything big. So you may think it’s weird, but you shouldn’t go changing a bunch of things you’re still learning about. Then when you’ve been on the team for a while, it sort of fades into the background.

It’s a mindset shift. You just need to occasionally remind yourself that you are capable of making you and your team’s life easier, when these sorts of things are hanging around.

## Assess the trade-off you’re making between quality and pace, make sure it’s appropriate for your context

There’s always a trade-off between implementation speed and how confident you are about correctness. So you should ask yourself: how okay is it to ship bugs in my current context? If the answer to this doesn’t affect the way you work, you’re being overly inflexible.

At my first job, I was working on greenfield projects around data processing, which had good systems in place to retroactively re-process data. The impact of shipping a bug was very minor. The proper response to that environment is to rely on the guardrails a bit, move faster because you can. You don’t need 100% test coverage or an extensive QA process, which will slow down the pace of development.

At my second company, I was working on a product used by tens of millions of people, which involved high-value financial data and personally identifiable information. Even a small bug would entail a post-mortem. I shipped features at a snail’s pace, but I also think I may have shipped 0 bugs that year.

Usually, you’re not at the second company. I’ve seen a lot of devs err on the side of that sort of programming though. In situations where bugs aren’t mission critical (ex. 99% of web apps), you’re going to get further with shipping fast and fixing bugs fast, than taking the time to make sure you’re shipping pristine features on your first try.

## Spending time sharpening the axe is almost always worth it

You’re going to be renaming things, going to type definitions, finding references, etc _a lot_; you should be fast at this. You should know all the major shortcuts in your editor. You should be a confident and fast typist. You should know your OS well. You should be proficient in the shell. You should know how to use the browser dev tools effectively.

I can already tell people are gonna be in the comments like “you can’t just spend all day tweaking your neovim config, sometimes you need to chop the tree too”. I don’t think I’ve ever seen someone actually overdo this though; one of the biggest green flags I’ve seen in new engineers is a level of care in choosing and becoming proficient with their tools.

## If you can’t easily explain why something is difficult, then it’s incidental complexity, which is probably worth addressing

My favorite manager in my career had a habit of pressing me when I would claim something was difficult to implement. Often his response was something along the lines of “isn’t this just a matter of sending up X when we Y”, or “isn’t this just like Z that we did a couple months ago”? Very high level objections, is what I’m trying to say, not on the level of the actual functions and classes we were dealing with, which I was trying to explain.

I think conventional wisdom is that it’s just annoying when managers simplify things like this. But a shockingly high percentage of the time, I’d realize when he was pressing me, that most of the complexity I was explaining was incidental complexity, and that I could actually address that first, thus making the problem as trivial as he was making it sound. This sort of thing tends to make future changes easier too.

## Try to solve bugs one layer deeper

Imagine you have a React component in a dashboard, that deals with a `User` object retrieved from state, of the currently logged in user. You see a bug report in Sentry, where `user` was `null` during render. You could add a quick `if (!user) return null`. Or you could investigate a bit more, and find that your logout function makes two distinct state updates – the first to set the user to `null`, the second to redirect to the homepage. You swap the two, and now no component will ever have this bug again, because the user object is never `null` while you’re within the dashboard.

Keep doing the first sort of bug fix, and you end up with a mess. Keep doing the second type of bug fix, and you’ll have a clean system and a deep understanding of the invariants.

## Don’t underestimate the value of digging into history to investigate some bugs

I’ve always been pretty good at debugging weird issues, with the usual toolkit of `println` and the debugger. So I never really looked at git much to figure out the history of a bug. But for some bugs it’s crucial.

I recently had an issue with my server where it was leaking memory seemingly constantly, and then getting OOM-killed and restarted. I couldn’t figure out the cause of this for the life of me. Every likely culprit was ruled out, I couldn’t reproduce it locally, it felt like throwing darts blindfolded.

I looked at the commit history, and found it started happening after I added support for Play Store payments. Never a place I would have looked in a million years, it’s just a couple http requests. Turns out it was getting stuck in an infinite loop of fetching access tokens, after the first one expired. Maybe every request only added a kB or so to memory, but when they’re retrying every 10ms on multiple threads, that adds up quick. And usually this sort of thing would have resulted in a stack overflow, but I was using async recursion in Rust, which doesn’t stack overflow. This _never_ would have occurred to me, but when I’m forced to look into a specific bit of code that I know _must_ have caused it, suddenly the theory pops up.

I’m not sure what the rule is here for when to do this and when not to. It’s intuition based, a different sort of “huh” to a bug report that triggers this sort of investigation. You’ll develop the intuition over time, but it’s enough to know that sometimes it’s invaluable, if you’re stuck.

Along similar lines, try out `git bisect` if the problem is amenable to it — meaning a git history of small commits, a quick automated way to test for the issue, and you have one commit you know is bad and one that’s good.

## Bad code gives you feedback, perfect code doesn’t. Err on the side of writing bad code

It’s really easy to write terrible code. But it’s also really easy to write code that follows absolutely every best practice, which has been unit, integration, fuzz, and mutation-tested for good measure – your startup will just run out of money before you finish. So a lot of programming is figuring out the balance.

If you err on the side of writing code quickly, you’ll occasionally get bitten by a bad bit of tech debt. You’ll learn stuff like “I should add great testing for data processing, because it’s often impossible to correct later”, or “I should really think through table design, because changing things without downtime can be extremely hard”.

If you err on the side of writing perfect code, you don’t get any feedback. Things just universally take a long time. You don’t know where you’re spending your time on things that really deserve it, and where you’re wasting time. Feedback mechanisms are essential for learning, and you’re not getting that.

To be clear I don’t mean bad as in “I couldn’t remember the syntax for creating a hash map, so I did two inner loops instead”, I mean bad as in:

> Instead of a re-write of our data ingestion to make this specific state unrepresentable, I added a couple asserts over our invariants, at a couple key checkpoints

> Our server models are exactly the same as the DTOs we would write, so I just serialized those, instead of writing all the boilerplate, we can write DTOs later, as needed

> I skipped writing tests for these components because they’re trivial and a bug in one of them is no big deal

## Make debugging easier

There’s so many little tricks I’ve acquired over the years on making software easier to debug. If you don’t make any effort to make debugging easy, you’re going to spend unacceptable amounts of time debugging each issue, as your software gets more and more complex. You’ll be terrified to make changes because even a couple new bugs might take you a week to figure out.

Here’s some examples of what I mean:

- For the backend of Chessbook
    - I have a command to copy all of a user’s data down to local, so I can reproduce issues easily with only a username
    - I trace every local request with OpenTelemetry, making it very easy to see how a request spends its time
    - I have a scratch file that acts as a pseudo-REPL, which re-executes on every change. This makes it easy to pull out bits of code and play around with it to get a better idea what’s going on
    - In the staging environment, I limit parallelism to 1, so that it’s easier to visually parse logs
- For the frontend
    - I have a `debugRequests` setting which prevents optimistic loading of data, to make it easier to debug requests
    - I have a `debugState` setting that will print out the entire state of the program after every update, along with a pretty diff of what changed
    - I have a file full of little functions that get the UI into specific states, so that as I’m trying to fix bugs, I don’t have to keep clicking in the UI to get to that state.

Stay vigilant about how much of your debugging time is spent on setup, reproduction, and cleanup afterwards. If it’s over 50%, you should figure out how to make it easier, even if that will take slightly longer this time. Bugs should get _easier_ to fix over time, all else being equal.

## When working on a team, you should usually ask the question

There’s a spectrum of “trying to figure out everything for yourself” to “bugging your coworkers with every little question”, and I think most people starting their careers are too far on the former side. There’s always someone around that has been in the codebase longer, or knows technology X way better than you, or knows the product better, or is just a more experienced engineer in general. There’s so many times in the first 6 months of working somewhere, where you could spend over an hour figuring something out, or you could get an answer in a few minutes.

Ask the question. The only time this will be annoying to anyone, is if it’s clear you could have found the answer yourself in a few minutes.

## Shipping cadence matters a lot. Think hard about what will get you shipping quickly and often

Startups have limited runway. Projects have deadlines. When you quit your job to strike out on your own, your savings will only last you for so many months.

Ideally, your speed on a project only compounds over time, until you’re shipping features faster than you could have imagined. To ship fast you need a lot of things:

- A system that isn’t prone to bugs
- Quick turnaround time between teams
- A willingness to cut out the 10% of a new feature that’s going to take 50% of the engineering time, and the foresight to know what those pieces are
- Consistent reusable patterns, that you can compose together for new screens/features/endpoints
- Quick, easy deploys
- Process that doesn’t slow you down; flaky tests, slow CI, fussy linters, slow PR reviews, JIRA as a religion, etc.
- About a million other things

Shipping slowly should merit a post-mortem as much as breaking production does. Our industry doesn’t run like that, but that doesn’t mean you can’t personally follow the north star of Shipping Fast.