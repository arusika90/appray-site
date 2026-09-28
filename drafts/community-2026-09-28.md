# Community drafts — 28 September 2026

Three drafts, built around the new blog post ("I built the feature people asked for most.
Then came four months of silence."). All are drafts only. Nothing here has been posted,
submitted, or automated. Mariia posts these herself, if and when she wants to, and should
read each one and adjust to taste first (tone, exact numbers, whether the link belongs at
all) before using it.

---

## 1. Reddit — r/SaaS

**Why this subreddit:** r/SaaS runs on metrics talk, funnels, adoption curves, feature usage
dashboards. This post works there precisely because it argues the opposite of the community's
default instinct: that request volume and actual usage are different claims, and that a
dashboard can make you feel certain about something you haven't actually checked. It also
introduces a real constraint most SaaS builders never have to work around, a product with no
analytics on principle, which tends to generate genuine discussion rather than the usual
metrics tool recommendations. Post as a text post, not a link post, so the story reads first.

**Suggested title:**
34 people asked for a feature, I built it, then had zero way to know if it worked

**Body:**

I make a small iOS app called Appray, a decision tool for founders, so this isn't really a SaaS
story, but the mistake in it is one I think applies more broadly than my situation.

Since launch, 34 separate emails asked for a way to export a verdict out of the app, PDF, share
sheet, anything. Second most requested thing after an Android version. I built it, PDF export,
one button, shipped it in a March update.

Here's the thing I hadn't thought through. Appray has zero analytics. No accounts, nothing
tracked, nothing leaves the device, on purpose, it's a whole selling point. Which is fine right
up until you ship a feature and want to know if it's actually being used. Most of you would open
a dashboard and have an answer in ten seconds. I had a button that could've been tapped forty
times or zero times and both were consistent with everything I could observe, which was nothing.
Four months went by and I genuinely read the silence as a good sign, the quiet you get when
something just works, before it occurred to me that silence and success look identical when you
have no instrumentation at all.

So I did the only thing available to me. Went back through the original 34 emails, picked 12
people I still had live addresses for, and just asked them directly. Did you use it, be honest
either way.

7 replied. 2 used it repeatedly and were glad it existed. 3 used it exactly once, right after it
shipped, then never touched it again, not because it was broken but because once the decision
was made they didn't need a document about it anymore, the deciding was the whole job. And 2 had
completely forgotten they'd asked for it and didn't remember the feature existed, despite having
opened the app since.

That last group is the one I can't stop thinking about. The request and the need weren't the
same thing measured twice, they were two different things that happened to arrive wearing the
same words. People asked for export in the moment they wanted proof the exercise had been
serious. That feeling is real. It just doesn't reliably survive as long as the feature does.

Not killing the feature, it costs nothing to keep and it clearly does its job for a few people.
But I've stopped treating "X people asked for it" as evidence a shipped feature is working. It's
evidence the feature was worth building. Those aren't the same claim.

Curious whether anyone here has caught themselves doing the same thing with a feature you do
have dashboards for. Genuinely wondering if having the data just makes it easier to fool yourself
a different way, mistaking a chart with no context for an actual answer.

---

## 2. Quora — answering an existing question

**Question found (verified live via search):** "Why should I remove features that are not
popular?" https://www.quora.com/Why-should-I-remove-features-that-are-not-popular

This fits well because the underlying question the asker has, is unpopularity actually a good
enough reason to cut something, is the exact question this week's story complicates. My answer
argues that "not popular" needs a second check before it becomes a decision, using this week as
a real example rather than a general framework. Confirm the question is still open and hasn't
been merged into another one before posting, Quora questions shift around over time.

**Answer draft:**

I'm a solo founder, I make an iOS app called Appray, so take this as one person's experience
rather than a rule, but I'd push back gently on "not popular" as a clean enough reason on its
own, because I nearly got it wrong myself this year in the opposite direction.

Second most requested feature in Appray's inbox behind an Android version was a way to export a
result out of the app, 34 emails since launch asking for some version of it. I built it, shipped
it in March. Then four months of complete silence, no complaints, no more requests, which I
first read as everything working fine.

Here's my complication: my app has no analytics at all, nothing tracked, nothing leaves the
device, so I had no dashboard to check "popular" against in the first place. I had to go find
out by hand, emailed 12 of the original 34 people directly and asked if they'd actually used it.
Of the 7 who replied, 2 used it a lot, 3 used it once and never again, and 2 had completely
forgotten they'd ever asked for it.

The 3-once-and-done group is the part I'd actually offer you. They weren't wrong to ask, and the
feature wasn't unpopular in any meaningless sense, it did exactly what they needed at exactly
one moment each. It just didn't need to be used repeatedly to have been worth building. If I'd
had a dashboard showing near zero repeat usage and used that alone to decide whether to remove
it, I'd have cut something that was quietly doing its job.

So before removing something on popularity alone, I'd check what the feature's job actually is.
Some features are meant to be used constantly and low usage really is the signal to cut. Others
exist for a single, real moment per person, export, a one time report, an emergency setting, and
judging those by frequency will always make them look unpopular even when they're working
exactly as intended. The fix isn't a different number, it's figuring out which kind of feature
you're looking at before you trust the number you've got.

**Before posting:** double check the question is still open and the URL above still resolves to
it, then post as is or trim the opening paragraph depending on how Quora is threading answers
that day.

---

## 3. Indie Hackers — post in "I made" / product discussion

**Framing:** search Indie Hackers first for an active thread on feature analytics, usage
tracking, or "how do you decide what to cut," and post this as a reply to add a dated, specific
story to it, since IH tends to reward replies that extend a real discussion over cold posts. If
nothing current fits, this also works as a short standalone post in the general or "I made"
category, since it's a concrete lesson rather than a launch announcement.

**Body:**

Small, slightly embarrassing thing from this week, posting in case it's useful to anyone building
something with deliberately no telemetry.

I make Appray, an iOS app that helps founders decide whether to build, kill, or prove a feature.
No accounts, nothing tracked, nothing leaves the device, that's a core part of the pitch. 34
emails since launch asked for a way to export a verdict out of the app. Second highest request
count I've had for anything, after wanting an Android version. Built it, shipped it in March,
one button, PDF export off the verdict screen.

Then nothing. No bug reports, no more requests, four months of quiet. I read that as things
working, the way you do when nobody's complaining. Took me embarrassingly long to notice that
with zero analytics, quiet and success are indistinguishable, and I'd built exactly the kind of
product where I couldn't just check.

Ended up emailing 12 of the original 34 people directly and asking if they'd actually used it.
7 replied. 2 used it a lot. 3 used it exactly once and never again, right after it shipped, not
because it broke but because once they'd made their decision they didn't need the document
anymore, the deciding was the whole job and the PDF was just something to hold onto during it.
And 2 had completely forgotten asking for it and didn't remember it existed.

Not killing it, it costs nothing to maintain and clearly does its job for some people. But I've
stopped reading "X people asked for this" as proof a shipped feature is working. It's proof the
feature was worth building. I'd been quietly treating those as the same sentence for four
months.

Mostly writing this down because I think it generalises past my specific no-analytics situation.
Even people with full dashboards can look at a usage number without knowing whether the feature's
job was meant to be used once or used constantly, and score it against the wrong bar. Curious if
anyone else has a story like this from the other direction, killed something because the numbers
looked bad, then found out later it was doing exactly what it was supposed to for a smaller group.
