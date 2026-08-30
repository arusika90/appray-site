# Community drafts — 30 August 2026

Three ready-to-post drafts, built around the new blog post ("A customer asked for a
feature. Should you build it?"). All are drafts only. Nothing here has been posted,
submitted, or automated. Mariia posts these herself, if and when she wants to, and
should read each one and adjust to taste first (tone, exact numbers, whether the
link belongs at all) before using it.

---

## 1. Reddit — r/EntrepreneurRideAlong

**Why this subreddit:** it's built around following real founders in real time,
text posts only (no link-only submissions), and it's one of the few large
subreddits where a story-led post that mentions your own product in context,
rather than as the headline, tends to survive rather than get removed. The
culture rewards "here's what actually happened," which is what this story is.
Post as a text post, not a link post.

**Suggested title:**
A customer asked me to build accounts and sync. I built something else instead.

**Body:**

I make a small iOS app called Appray, so take the following with whatever grain
of salt that requires. This isn't a launch post, just something that happened
last month that I think is a useful example for anyone getting feature requests
from actual users for the first time.

In July someone emailed me twice in the same week asking why the app doesn't
have an account. Not a bug, nothing they needed that day, just wanting their
work to still be there if they lost their phone.

My first instinct was to say yes. Someone had paid for the thing and taken the
time to write to me, and the request sounded completely reasonable. Saying no
to that feels rude in a way that saying no to your own idea never does.

But "add an account" wasn't actually the ask. The ask, once I sat with it, was
"I'm afraid of losing this." An account system would have meant a login screen,
password resets, a server, and a real conversation about data breaches, on an
app whose entire selling point is that nothing leaves your device. All to fix a
fear that a one-tap PDF export solves in three days instead of three weeks,
without touching the thing that made someone choose the app in the first place.

The test I use now, for anyone building something people actually pay for: when
a request comes in, ask what it's a proxy for, not whether it sounds reasonable.
And ask if it would still be worth building if only one or two people ever
mention it again. Most requests fail one of those quietly. A few pass both, and
those are the ones worth an afternoon.

I got this wrong once too, in the other direction, building a small tagging
system off one email before the pattern showed up anywhere else. Happy to go
into that one in the comments if anyone wants it.

---

## 2. Quora — answering an existing question

**Question found (real, currently open on Quora):**
"How do you decide what features to build (or kill)?"
https://www.quora.com/How-do-you-decide-what-features-to-build-or-kill

This is a near-exact match for Appray's own Build / Kill / Prove language, which
is why it's worth answering directly rather than writing a generic post. Answer
the question as asked, keep the product mention to one line near the end.

**Answer draft:**

I make Appray, an app that specifically forces this decision for a living, so
I've had to turn "build or kill" from a feeling into an actual process, because
my gut is wrong at least a third of the time.

Two checks have done most of the work for me:

First, what is the request actually a proxy for. Nobody asks for a feature
because they want that exact feature, they ask because of something underneath
it. A user of mine asked for cloud accounts. What they actually wanted was to
stop worrying about losing their data if they dropped their phone. The account
system I almost built would have cost three weeks and compromised the privacy
promise of the whole product. A one-tap export cost three days and solved the
actual fear.

Second, would this still be worth doing if it stayed rare. Two people asking
in a week is not a trend, it's two people. If the honest answer is "no, I was
about to redesign around a sample size of two," that's a kill, or at least a
"prove it first" rather than an immediate build. If the fix is cheap and the
underlying fear is one anyone could have regardless of how many voices you've
heard it from, it can pass even on a small sample.

Where this goes wrong for most people, including me at times, is skipping
straight from "someone asked" to "I should build it," because saying no to a
customer who took the time to write feels worse than it actually is. The
customer isn't attached to the specific implementation they suggested. They're
attached to the problem going away.

---

## 3. Indie Hackers — reply to an existing thread

**Thread found (real, currently open on Indie Hackers):**
"A prospective customer asked for a feature! Should I build it?"
https://www.indiehackers.com/post/a-prospective-customer-asked-for-a-feature-should-i-build-it-eb800fdc70

This is close enough to the blog post's exact topic that a comment reply reads
as genuine participation rather than a plug. Post as a reply/comment on that
thread, not a new post. If it feels more natural as a fresh IH post instead
(e.g. if the thread has gone stale or is locked), use the same content as a
short standalone post and add one line at the top noting it grew out of
someone else's question on this exact topic.

**Reply draft:**

I make Appray (a Build/Kill/Prove decision tool for founders), so this is
close to home for me. The short version of what's worked: don't evaluate the
feature they asked for, evaluate what they're afraid of or stuck on underneath
it. A user of mine asked for account sync. What she actually wanted was to
stop worrying about losing her work. I built a one-tap export instead, three
days instead of the three weeks an account system would have cost, and it
solved the actual problem without adding a login screen to a privacy-first
app.

Second thing that's helped: ask if the request would still make sense if it
stays rare. One or two people asking is a data point, not a mandate. If the
fix is cheap and the fear behind it is universal, build it even on a small
sample. If it's expensive or changes what you promise your users, wait for
the pattern to show up more than once.

Said yes too fast once myself, building a tagging system off a single email
before more than one person had the problem it solved. It turned out to be
the right feature eventually, just built about a year earlier than the demand
justified it, which cost a week I didn't need to spend yet.
