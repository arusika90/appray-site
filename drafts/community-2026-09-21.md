# Community drafts — 21 September 2026

Three drafts, built around the new blog post ("Two five-star reviews arrived the same week,
asking for opposite things"). All are drafts only. Nothing here has been posted, submitted, or
automated. Mariia posts these herself, if and when she wants to, and should read each one and
adjust to taste first (tone, exact numbers, whether the link belongs at all) before using it.

---

## 1. Reddit — r/SideProject

**Why this subreddit:** r/SideProject is full of solo builders sharing what actually happened
that week rather than launch announcements, and it rewards posts that admit an almost-mistake
over posts that claim a clean win. This story fits directly: a real product decision, a wrong
first instinct caught before shipping, and a constraint (no analytics, by design) that a lot of
that audience will recognise from their own privacy-conscious or account-free projects. Post as
a text post.

**Suggested title:**
Two 5 star reviews asked for opposite things the same week, and my app has zero analytics to break the tie

**Body:**

I make a small iOS app called Appray, a decision tool for founders, so keep that in mind reading
this. Not a launch post, just something that happened this week that felt worth writing down
before I forget how close I came to getting it wrong.

Appray's core flow is an eight round interview that ends in a verdict. Two reviews landed four
days apart, both four or five stars, both about that same interview, wanting opposite things.
One person said it felt long for something they'd only use once a month. The other said they were
glad it wasn't one of those apps that spits out an answer in ninety seconds, because they wouldn't
trust a verdict that fast for a decision this size.

My first instinct was to average it. Cut the eight rounds to six, annoy both people slightly less
than either extreme. I actually sketched out which two rounds I'd drop before I caught myself.
Six rounds serves neither person. The one who wants speed still sits through six questions they
find excessive, and the one who wants rigour now has a shorter interview backing a verdict they
already worried was too quick. Splitting the difference between two complaints doesn't produce
what either person asked for, it produces a third thing nobody asked for.

Here's the part that made this harder than it should've been: Appray doesn't collect anything.
No accounts, no analytics, nothing leaves the device. That was a deliberate choice and most days
I think it was the right one, but it meant I couldn't just look at a drop off funnel and get an
answer in ten minutes. I built the one kind of app where that shortcut doesn't exist, and then
hit the exact decision where I wanted it back.

What actually broke the tie was rereading both reviews in full instead of the one line I
remembered from each. Reviewer one's actual complaint, buried a bit further down, was about not
being able to leave the interview and come back without losing progress, not really about round
count at all. Reviewer two wanted the verdict screen to show which of their own answers had
driven it, so they could see the reasoning rather than trust a colour. Neither review was
actually about length. They'd both used "long" and "fast" as the nearest word for a completely
different problem.

Left the interview alone. Filed both real issues separately in the same plain note everything
else goes in. Neither's a build yet on one data point each, but at least they're filed as what
they actually are now.

Anyone else building something with deliberately no telemetry run into this? Curious how you
settle disagreements like this one without the easy version of the answer sitting in a dashboard
somewhere.

---

## 2. Quora — answering an existing question

**Question found (verified live via search):** "How did you, as a product manager, manage to say
no to feature requests? I am looking for real life examples and not general frameworks."
https://www.quora.com/How-did-you-as-a-product-manager-manage-to-say-no-to-feature-requests-I-am-looking-for-real-life-examples-and-not-general-frameworks

This is a strong fit because the asker explicitly rules out generic frameworks and wants a real
story, which is exactly what this week gave me. Confirm the question is still open before
posting, questions can get merged or closed on Quora over time.

**Answer draft:**

I'm not a product manager in the traditional sense, I'm a solo founder, I make an app called
Appray, and I don't have a team to defer to when a request lands, so every "no" is mine alone.
Here's a real one from this week rather than a framework.

Two reviews arrived four days apart, both four or five stars, both about the same part of the
app (an eight round interview that ends in a decision verdict), asking for opposite things. One
wanted it shorter. One wanted it longer, or at least wanted proof it wasn't rushed. My first
instinct, which I'm a little embarrassed by, was to average it, cut it down a couple of rounds
and hope that annoyed both people less. I got as far as picking which rounds to cut before I
stopped, because a compromise like that serves neither person. It produces something nobody
actually asked for while feeling, to me, like a reasonable middle ground.

What actually resolved it was going back and reading both reviews in full instead of the one
line I'd remembered getting annoyed about. Neither person was really complaining about length.
One wanted to be able to leave the interview partway and come back to it. The other wanted to
see which of their own answers had produced the verdict, essentially wanting visible reasoning,
not more questions. "Long" and "fast" were just the closest words they had for something else
entirely.

So the "no" here wasn't a no to a person, it was a no to my own first read of the situation. I
left the actual feature alone and filed the two real, different issues separately instead of
building a compromise that would have solved neither.

The general thing I'd actually pass on: when two people seem to disagree about the same feature,
reread both messages in full before you believe the disagreement is real. A surprising amount of
the time they're describing two different problems that happen to share a word like "too slow"
or "too long."

**Before posting:** double check this question is still open and the URL above still resolves to
it, then post as is or trim the opening line to fit however Quora is threading answers that day.

---

## 3. Indie Hackers — reply to an existing thread

**Framing:** search Indie Hackers for an active thread on prioritizing feedback, handling
conflicting feature requests, or building without analytics/tracking, and post this as a reply
rather than a fresh post, since IH replies that add a specific dated story to an existing
discussion tend to land better than a cold post. If nothing current fits closely, this also works
posted as a short standalone update in the "I made" or general discussion category.

**Body:**

Small thing from this week that might be useful if anyone else here has deliberately built
something with no analytics.

I make Appray, an iOS app that helps founders decide whether to build, kill, or prove a feature.
No accounts, nothing tracked, nothing leaves the device, on purpose. Two reviews landed four days
apart this week, both positive, both about the same core flow (an eight round interview before
you get a verdict), asking for opposite things. One wanted it shorter. One wanted it longer, or
at least wanted more confidence it wasn't rushed.

Normally I'd pull up a funnel and see where people actually drop off and have an answer in ten
minutes. Couldn't, because I built the one kind of product where that data doesn't exist. So I
nearly did the lazy thing instead, split the difference and cut a couple of rounds, which in
hindsight would have pleased nobody and quietly made the product worse.

What actually worked was slowing down and rereading both reviews properly instead of the single
line I remembered from each. Neither was really about length once I read the whole thing. One
wanted to resume a session instead of losing progress. One wanted to see which of their own
answers drove the result. Two different, real, small issues wearing the same complaint about
speed.

Left the interview as is, filed both properly instead of averaging them into a fix for neither.
Mostly writing this because "reread the whole message before you trust the pattern you think
you're seeing" sounds obvious written down and somehow still isn't the thing I do by default
under a bit of pressure.
