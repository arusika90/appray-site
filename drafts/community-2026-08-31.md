# Community drafts, 31 August 2026

Three ready to post drafts, built around the new blog post ("How to prove a feature
before you build it"). All are drafts only. Nothing here has been posted, submitted,
or automated. Mariia posts these herself, if and when she wants to, and should read
each one and adjust to taste first, tone, exact numbers, whether the link belongs at
all, before using it.

---

## 1. Reddit, r/SaaS

**Why this subreddit:** r/SaaS runs on story led posts that ask a real question and
keep the product itself secondary, and it explicitly tightened self promotion rules
in 2026 to once every 60 days, so a post needs to earn its place with an actual
question rather than a pitch. This one does: it disagrees with a technique
(fake door testing) that gets recommended constantly in that community, and asks
whether anyone else has felt the same way about it. That is the kind of post that
survives there. Post as a text post, once, and don't link the app anywhere except
the one line naming it.

**Suggested title:**
I ran a fake door test once and didn't like what it did to the people who clicked it

**Body:**

I make a small iOS app called Appray, so keep that in mind while you read this. Not
a launch post. Just something I keep thinking about.

Early on I put a button in a test build that said "Sync across devices" and did
nothing when you tapped it, just logged the tap. Standard fake door test, the kind
that gets recommended everywhere, including on here. Eleven taps out of nineteen
testers over three weeks. Sounds like real interest until you remember testers tap
every button in a small build because that's what testers do. Nobody wrote in asking
where the sync feature had gone. Nobody was annoyed it didn't work. The number
told me nothing I could act on.

What actually bothered me wasn't the weak signal, it was that someone taps a button
in good faith and gets a silent log line back. That's a small lie told to a person
who trusted the thing enough to try it. I know the standard defence, mild harm for a
useful number, and I mostly buy it in the abstract. I still didn't want to keep doing
it to someone.

What's worked better for me since: counting asks that show up on their own, in a
person's own words, without me prompting for them. Two people asking for the same
underlying thing within a few days of each other, in different language, has told me
more than any test I've engineered. And asking someone to name the specific past
moment they needed the feature, not a hypothetical future one, filters out almost
all the polite "yeah that'd be cool" responses.

Curious whether anyone else has run fake door tests and come away feeling similar
about them, or whether I'm overthinking a technique that's genuinely harmless at the
scale most of us operate at.

---

## 2. Quora, answering an existing question

**Question found (real, currently open on Quora):**
"How do experienced creators validate a digital product idea before spending weeks
building it?"
https://www.quora.com/How-do-experienced-creators-validate-a-digital-product-idea-before-spending-weeks-building-it

This is a close match for the blog post's actual topic and is phrased exactly the
way people search for this problem, which is why it's worth answering directly.
Answer the question as asked, keep the product mention to one line.

**Answer draft:**

I make Appray, a decision tool that specifically forces this question for a living,
so I've had to turn "validate before building" from a slogan into something I
actually do every time, not just for the big features.

Two things have done most of the work.

First, I stopped trying to manufacture demand signals and started just counting the
ones that show up unprompted. If two or three people mention the same underlying
want, in their own words, without me having asked a survey question, that's worth
more than fifty responses to something I wrote myself. A survey answer is shaped by
the question you asked. An email someone sent you on their own is shaped by nothing
but the actual problem.

Second, I ask for something small and real in return for attention, rather than a
click. Not necessarily money, though that's the strongest version. A real email
address on a specific waiting list works. So does asking someone to describe the
exact past moment they needed the thing. If they can name a specific day and what
they were doing, that's a real need. If they describe a general future where it
would obviously come in handy, it usually isn't, no matter how sincerely they mean
it. People are honest about the future in a way that has very little to do with what
they'll actually do later.

I tried a fake door test once, a button that did nothing but log a tap, and got a
number that looked like interest but predicted nothing. What actually predicted the
next feature I built was two unrelated people describing the same fear, four days
apart, in completely different words.

---

## 3. Indie Hackers, reply to an existing thread

**Thread found (real, currently open on Indie Hackers):**
"Use the Fake Door Test to validate your SaaS product before building it."
https://www.indiehackers.com/post/use-the-fake-door-test-to-validate-your-saas-product-before-building-it-709eadf520

This is the exact technique the new blog post pushes back on, so a reply here reads
as genuine disagreement from experience rather than a plug. Post as a reply/comment
on that thread, not a new post. If the thread has gone stale or is locked, use the
same content as a short standalone IH post instead, with one line at the top noting
it grew out of this thread.

**Reply draft:**

I make Appray (a Build/Kill/Prove decision tool for founders), so this technique is
close to home for me, and I want to push back a little from the other side of it.

I ran a version of this early on, a button that said "Sync across devices" and did
nothing but log the tap. Got a number, 11 taps out of 19 testers over three weeks,
that looked like a real signal. It wasn't. Testers tap everything in a small build.
Nobody followed up afterwards asking where the feature went, which told me the click
wasn't attached to an actual want.

What I didn't expect was how it felt to run. Someone taps a button in good faith and
gets nothing back but a silent log line. I know the usual defence, low harm for a
useful number, and I think that's mostly true. I still stopped after one round
because I didn't want Appray built on that kind of small deception even in service
of a good number.

What's replaced it for me: counting asks that arrive on their own, unprompted, and
asking anyone who wants a feature to name the specific past moment they needed it
rather than a hypothetical future one. Two people describing the same underlying
problem in different words, a few days apart, has been a far better predictor for me
than any click I've engineered. Not saying fake doors don't work for anyone, just
that the honest version turned out to be about as cheap and I trust it more.
