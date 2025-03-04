#### Source: https://mbuffett.com/posts/maintaining-motivation/

# Managing My Motivation, as a Solo Dev
One of the biggest sticking points of being a solo dev is maintaining motivation. I’ve been keeping a journal entry about how to hack my motivation, what works and what doesn’t. Here are the things that have worked.

### Convert external sources to motivation

I’ve always known that I’m more extrinsically than intrinsically motivated, so I have a couple systems that help to give me bursts of external motivation. For example, the Money Bots, which pop up every time someone subscribes.

![](https://mbuffett.com/motivation/money_bots.png)

I’m a push notification ascetic, but these pop up right on my home screen. It’s a small burst of motivation every time. There’s a bit of a hedonic treadmill effect; initially a single new subscriber was a massive hit of dopamine/energy, and that’s reduced over time, but they still fuel me.

In a similar vein, I signed up for a service that notifies me whenever someone mentions Chessbook. This is simultaneously useful for marketing, since engaging on socials can help a lot, but it’s also motivating whenever I see people talking (hopefully positively) about the thing I’ve built.

There’s also a `#pump-up` channel with a feed of milestones we’ve hit, like $X MRR, 2,000 discord users, churn rate <6%, motivating stuff like that.

### Leave tasks unfinished

I can’t overstate how much this one helps me. I try to leave a task 90% finished at the end of a working session. It feels slightly worse than closing out the work, but it makes starting the next day 10x easier. Having a quick win when I start coding is a massive boost, and it immediately gets me into the flow state. It can’t be _too_ easy though, if all I have left is to run `git commit`, that’s not enough. Ideally it’s something where I know exactly what I need to do, that will take 5-10 minutes.

### Use the thing myself, as much as possible

I try to use my own product as much as I can. When someone submits a bug report about some jank, sometimes it’s easy to classify it as a small issue. Then I run into it myself, realize that it really affects the experience, and go fix it right away. Felt pain is way more salient than communicated pain.

To digress, this also gives me way better product ideas, the best ones I’ve had didn’t come from sitting down and thinking about what people may want, they came from realizing what I myself want.

### Address the pain, instead of pushing through

There’s always some parts that suck. A neglected area of the codebase, dealing with third parties, releasing new versions of native apps, etc. If I know I’ll have to deal with one of these as part of a task, it can feel much harder to motivate myself to get started.

The trick, is that you can almost always make these less painful.

For example, recently I felt a lot of friction starting a new task because it needed 4+ new endpoints, and that always involved a lot of boilerplate. I have to write the types on the backend, write the same types on the frontend, make sure I get the payload correct, make sure I get the path correct, and nothing is type-checked so usually it doesn’t work the first time. So before starting, I found a RPC library called [RSPC](https://www.rspc.dev/), which generates types for me, and makes writing and calling a new backend function from the frontend almost as easy, and just as type-safe, as calling another async frontend function.

Not only did this remove the pain point, but I was actively excited to use this new system. I converted a source of friction into a motivation multiplier.

This is one that’s easy to forget if you’ve worked in bigger companies where you can’t address the pain points of day-to-day development. You’ve probably acquired a sense of futility in trying to address these things. There’s either deadlines to hit, or people to get sign-off from, or you need to write a technical doc on your approach before you get to try it. Being able to just go fix and improve whatever you want is one of the greatest points of being a solo dev, so remind yourself that you can take advantage of it at any time.

### Do nothing

I get sucked into high-tech Skinner Boxes all the time. Reddit, Twitter, YouTube, etc. The best way I’ve found to get out of this is to do it in two steps. First I go from Reddit to doing nothing, then I get to work.

Going straight from Reddit to focused work is very hard, but doing nothing is much easier, and eventually your brain calms down and it doesn’t feel nearly as hard to start writing some code.

I really mean doing nothing; I’ll just sit in front of my screen for a few minutes and as if by magic, the consumption-fueled dopamine-overload fog will lift, and I can get excited about creation and problem-solving again.

### Update my users

This is a two-for-one, I can both update my users, and motivate myself by looking back on progress. I often reach the end of the month, and find myself thinking “did I even get anything done?”, but then you can write your update for the month, and see that you did get a lot done.

![](https://mbuffett.com/motivation/update.png)

Obviously this cuts both ways though, if you really didn’t get much done you’ll see that too, but facing the truth that you’re not getting enough done can be motivating too.

### Get a partner

This may seem contradictory to the title, but I only said solo _dev_. I have a partner, who’s way better at everything product/design/copy/etc.

I won’t list all the benefits of having a partner, but I now believe they’re essential, and in any future projects I’ll be making sure to find a partner that complements my skillset while being aligned on the problem. It’s a night and day difference.

The motivation piece here is mostly around accountability. It’s the same reason that people have gym partners, just having someone that expects you to show up can be powerful. Also if you have a weekly meeting and find you have nothing to talk about, you’re probably not getting enough done, and it’s a salient reminder.

The other piece is that your motivation and your partner’s motivation will ebb and flow, and it won’t happen in lock-step. It’s very helpful to have someone else still motivated about the project, when you’re not.

### No zero days, to avoid listless guilt

Some days when I’m not getting anything done, I’ve got this lingering guilt that I’m having a “zero day”. This prevents me from fully enjoying whatever activity I’m doing. I’ve tried just giving myself permission to enjoy whatever I’m doing, but it just doesn’t work. Ostensibly I’m taking time off and recharging, but it doesn’t feel like that at all – it feels like pushing through. This can lead to a negative feedback loop, where I’m constantly trying to recharge, but just getting more tired.

I’ve found the only way is to get some good work done first, then I can be fully immersed in whatever fun slacking-off activity I dive into.

### If I’ve got it, use it

Sometimes I’ll be going to bed thinking about a problem, and get the motivation which comes in the moment of figuring things out. I could write it down and get to it in the morning, but most of the time I’ll just get up and work until 4am instead. This is also one of the great parts of being a solo dev. I don’t need to be up at 9am to be available on Slack, so I can use my motivation whenever it strikes me, even if that’s in the middle of the night.

This probably doesn’t generalize, but again this is more of a journal entry adapted into a blog post, than it is advice. I’ve always done better with the looser approach of trying to maximize the opportunities for flow state work, than forcing myself to work 9-5 every day, rain or shine.

### You have ADHD, getting yourself to work shouldn’t be this hard

True 😄