# Community drafts, 10 September 2026

Three ready-to-post drafts, built around the new blog post ("Should I build an
Android version?"). All are drafts only. Nothing here has been posted, submitted,
or automated. Mariia posts these herself, if and when she wants to, and should
read each one and adjust to taste first (tone, exact numbers, whether the link
belongs at all) before using it. Every draft states plainly that Mariia makes
Appray.

---

## 1. Reddit — r/iOSProgramming

**Why this subreddit:** r/iOSProgramming is where iOS developers talk shop, and
"should I go cross-platform" is one of its recurring, welcomed threads, especially
from solo developers with real numbers rather than a theoretical question. None of
the last four rounds of drafts used this subreddit (r/EntrepreneurRideAlong,
r/SaaS, r/microsaas and r/startups were used on the four most recent rounds), so
it's clear of any self-promotion cooldown. It also fits the topic better than a
general startup subreddit would, since the actual decision is a native rewrite in
a second language, which this audience understands the cost of better than most.
Post as a text post.

**Suggested title:**
19 emails asking for Android, and a decision framework that made me realise most of them weren't actually asking for that

**Body:**

I make Appray, a small iOS-only app, so keep that in mind. Not a launch post,
just a decision I've been putting off and finally sat down with properly this
week.

Since launch I've had 19 emails asking, in some form, why there's no Android
version. My instinct for months was to lump them together as "people who want
Android" and file the whole thing under someday. This week I actually read all 19
properly instead of skimming for the word Android, and they split into two piles
I'd been treating as one.

Twelve are from people who simply don't own an iPhone. No smaller fix exists for
that, the app either runs on their phone or it doesn't. Seven are from people who
switched phones, or carry an iPhone for work and Android personally, and want
their data to follow them. That second group isn't actually asking for a native
Android app. They're asking not to lose their data because of which pocket their
phone is in, which a plain export file solves for a rounding error of the cost of
a second native build in a language I don't currently know.

The bit I mostly want other solo iOS devs' opinion on: I ran a landing page for
three weeks (one paragraph, no Android yet, an email field for when it exists) as
a cheap way to measure real demand instead of guessing from a moderately upset
inbox. 41 signups against roughly 4,000 App Store page views in the same window.
Small, real, and not enough on its own to justify a rewrite for an app that
hasn't proven it can support its own founder full time on one platform yet.

Curious whether anyone else here has run something similar before committing to a
second platform, or has a better way to separate "wants Android" from "wants their
data portable" before treating every Android email as the same request.

---

## 2. Quora — answering an existing question

**Question found (real, currently open on Quora):**
"Is it worth developing an app for both iOS and Android at the same time?"
https://www.quora.com/Is-it-worth-developing-an-app-for-both-iOS-and-Android-at-the-same-time

This is a close match for the blog post's actual dilemma (not "which platform
first" in the abstract, but whether a shipped iOS app is worth doubling for
Android), so answering it directly is a genuine fit rather than a forced one.
Confirm the question is still open before posting. Keep the product mention to
one line near the end.

**Answer draft:**

I make Appray, an iOS-only app, so I'm mid-way through actually answering this for
my own product rather than in the abstract, which changed my answer from what I
would have guessed a year ago.

The revenue maths that gets quoted for this question is usually right: a paid,
no-ads app in a smaller niche tends to earn a fraction on Android of what it earns
on iOS, sometimes five to ten times less, because the audiences have different
habits around paying for things. I don't think that number is wrong. What it
doesn't tell you is whether the requests you're getting are actually about
revenue, or about something smaller you've been lumping in with the big decision.

I had 19 emails asking about an Android version. Reading them properly instead of
counting them, 12 were people who genuinely can't use the app at all without one.
Seven turned out to be people who wanted their data to follow them between an
iPhone and an Android phone they also carry, which a plain export file solves for
a fraction of the cost of a full native rewrite. Two different problems were
arriving in the same kind of email, and I'd spent months answering both of them
with the same no.

Before committing to "worth it" or "not worth it" as one decision, I'd separate
what's actually being asked, and if there's real doubt about total demand, a
simple landing page collecting emails for a few weeks is a cheap way to measure it
against your existing platform's traffic, rather than guessing from how loud your
inbox feels.

---

## 3. Indie Hackers — reply to an existing thread

**Thread found (real, currently open on Indie Hackers):**
"No one cares about android apps"
https://www.indiehackers.com/post/no-one-cares-about-android-apps-6dc504e8de

This thread argues close to the opposite of a nuanced answer, so a reply with a
real, currently-live example (the landing page test, the split between the two
kinds of requests) adds something rather than just agreeing or disagreeing in the
abstract. Post as a reply/comment on that thread. If it's gone stale or is locked,
use the same content as a short standalone IH post with one line at the top noting
it grew out of this question.

**Reply draft:**

I make Appray (a Build/Kill/Prove decision tool for founders, iOS only so far),
and I've been going back and forth on exactly this for my own app, so I'll add a
real data point rather than just an opinion.

19 people have emailed me asking about Android since launch. I'd been treating
that as one undifferentiated pile of "people who want Android" until this week,
when I actually read all 19 instead of counting them. Twelve genuinely can't use
the app without one, full stop. Seven turned out to want something smaller, their
data following them between an iPhone and an Android phone they also carry, which
a plain export file solves without a second native app at all.

I don't think "no one cares" is quite right, but I don't think the revenue case
for a full rewrite is either, at least not yet for something the size of my app. I
ran a landing page for three weeks instead of guessing, one paragraph, no Android
yet, email field for later. 41 signups against about 4,000 App Store page views in
the same window. Real, small, not enough to justify four to six months of a second
native build for an app that hasn't proven it can support its founder full time on
one platform.

The part I'd add to this thread: before deciding Android does or doesn't matter,
it's worth splitting the requests you're actually getting into what they're really
asking for. Not all of them are the big ask they sound like.
