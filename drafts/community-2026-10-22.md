# Community drafts — 22 October 2026

Ready-to-post drafts for the blog post "Appray has no analytics. Here's how I know what to fix
anyway." (https://appray.app/blog/no-analytics-how-i-know-what-works/). DRAFTS ONLY. Nothing here
has been posted. Mariia reviews and posts these herself.

## 1. Reddit — r/privacy

**Why this subreddit:** r/privacy is full of people who specifically want products that collect
nothing, and who are also sharp enough to ask the follow-up question nobody else asks: fine, but
how do you build anything good if you can't see how people use it. That's exactly the trade-off
this post is about, told honestly instead of as a marketing line. Note r/Entrepreneur,
r/EntrepreneurRideAlong, r/SaaS, r/microsaas, r/startups, r/iOSProgramming, r/ProductManagement,
r/indiehackers, r/SideProject, r/mobiledev, r/buildinpublic, r/UXResearch and
r/ArtificialIntelligence have all been used in previous rounds of these drafts, so r/privacy keeps
this from repeating a subreddit, and it fits this specific post better than any of those would.

**Suggested title:** My app sends zero data anywhere. Here's the actual cost of that decision.

**Post body:**

I make Appray, a small iOS app that walks someone through eight rounds of questions and gives a
Build, Kill or Prove verdict on a feature idea. Solo founder, Rijeka, Croatia. The App Store page
says no account, no sign in, nothing leaves your device, and I mean that literally, no analytics
SDK either, because an analytics SDK is a thing that sends events off the phone regardless of how
the privacy policy describes it.

What I don't think gets said enough in privacy-minded spaces is what that actually costs you as
the person building the thing. I have no idea how many people finish the eight rounds versus quit
partway. I have no idea which verdict comes back most. When I shipped a local notification that
reminds people to check back on a test two weeks later, I genuinely did not know for four months
whether it was firing correctly on everyone's phone, because finding that out the normal way means
a crash reporter or an event log phoning home, and I'd ruled that out on purpose.

The way I actually found out: I started adding one line to the bottom of unrelated support
emails, asking whether the reminder had shown up for them. Fifteen people, over six weeks, nine
said yes. That's not a dashboard, it's a trickle, and it took six weeks to learn what a graph
would have told me in an afternoon.

Worse, I nearly made a bad call the other direction. Three App Store reviews, out of around forty,
said the interview felt long, and I spent two days building a shorter version before I caught
myself: those forty reviews are entirely people who finished. Someone who quits on round four
never leaves a review. I was about to cut something based on the opinions of the only people who
didn't actually have the problem.

I'd still make the same choice again. But I think privacy-first products get talked about like
the trade-off is free, and it isn't. You give up a lot of visibility, you make some decisions
slower and some probably wrong for longer than they should be, and the honest version of
"we don't track you" includes admitting that cost rather than pretending there's a clever
privacy-preserving substitute that gives you the dashboard back for free.

Longer version with both specific mistakes: https://appray.app/blog/no-analytics-how-i-know-what-works/

---

## 2. Quora — answering an existing question

**Question found (real, currently indexed on Quora):** "How will you measure the success of the
mobile app?" https://www.quora.com/How-will-you-measure-the-success-of-the-mobile-app

**Answer:**

I'm Mariia, I make a small iOS app called Appray, and I'm answering this from an unusual position:
my app has no analytics at all, by design, because its whole pitch is that nothing leaves your
device. So I can't give you the standard answer about retention curves and funnel drop-off,
because I don't collect any of that about my own product.

What I use instead, for what it's worth to anyone in a similar spot or just curious whether it's
possible: App Store Connect still gives you aggregate downloads, impressions and crash counts
without any tracking code of your own, so you're not completely blind even at zero. Beyond that,
I treat support emails as data, I've started tacking an extra question onto replies about
something unrelated when I need to know if a specific feature is working, and I occasionally ask
a small group of people to use the app on a video call and just narrate out loud what they're
doing, which catches things a chart wouldn't show you anyway, like where someone's wording is
confusing rather than just where they clicked.

The honest limitation: this is slower, and it can mislead you. I nearly cut a core part of my app
because of three reviews complaining it was too long, out of forty total, before I realized that
all forty reviews came from people who'd finished it. The people who quit earlier for that exact
reason never show up in a review at all. If you do have analytics, that particular trap is easy to
avoid. Without them, you have to go looking for the people who aren't telling you anything, which
is a different and slower kind of measuring success, not really a substitute for the kind involving
numbers.

Write-up with the full story: https://appray.app/blog/no-analytics-how-i-know-what-works/

Posting note: reconfirm the question is still open before posting, Quora questions get merged or
go stale. If it's gone, "how do you measure product success without tracking users" or "is it
possible to run an app without analytics" are close live substitutes for the same answer.

---

## 3. Indie Hackers — reply to an existing thread

**Why this framing fits:** There's a live Indie Hackers post arguing that founders don't need more
dashboards, they need better product judgment, and that a click count alone can't tell you whether
a feature actually helped anyone. That's the exact argument this blog post makes from the opposite
direction: not "dashboards are overrated" as a general claim, but "here is what it actually costs
you when you have zero dashboard at all, including the one time it almost got a feature cut by
mistake." Replying there adds a real, lived data point to a thread that's otherwise mostly opinion.

**Thread to reply to:** "Founders don't need more dashboards, they need better product judgment" —
indiehackers.com

**Reply body:**

This matches something I live with daily, from the extreme end of it. Appray, my iOS app, has
literally no analytics, no event tracking, nothing, because the product's whole promise is that
nothing leaves your device. So I don't get to choose between "trust the dashboard" and "trust my
judgment," I only have judgment, and I can tell you it's not a clean substitute.

The clearest example: I shipped a feature, a local reminder notification two weeks after a certain
verdict, and had no way to confirm it was actually firing for people. Took four months and a
habit of tacking one extra question onto unrelated support email replies before I had even rough
confidence it worked for most people. A dashboard would have told me that in a day.

The part that actually worries me, though, is the opposite failure: I almost cut a whole section
of the app because three out of around forty App Store reviews said it felt too long. What I
didn't account for until later is that all forty of those reviews came from people who finished
the product. The people who quit early for that exact reason don't leave reviews, they just leave.
Judgment without any data at all doesn't just move slower, it can be confidently wrong in a
direction a dashboard would have caught immediately.

So I'd push back gently on the framing: better judgment is necessary, but it's not actually a
replacement for seeing the drop-off, it's a worse, slower way of approximating what the drop-off
would have told you directly, and it's worth being honest with yourself about which one you're
doing.

I wrote the longer version of both mistakes here, if useful to anyone else choosing this trade-off
on purpose: https://appray.app/blog/no-analytics-how-i-know-what-works/

Mariia, solo founder, Appray.
