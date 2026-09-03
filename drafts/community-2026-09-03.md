# Community drafts — 3 September 2026

Three ready-to-post drafts, built around the new blog post ("When to kill a feature you
already shipped"). All are drafts only. Nothing here has been posted, submitted, or
automated. Mariia posts these herself, if and when she wants to, and should read each one
and adjust to taste first (tone, exact numbers, whether the link belongs at all) before
using it.

---

## 1. Reddit — r/microsaas

**Why this subreddit:** r/microsaas is built for solo and small-team founders posting
their own product's backstory, and it explicitly wants the real numbers and the mistakes,
not a launch announcement. A post about failing to remove your own dead feature for five
weeks, with real usage numbers attached, is exactly the kind of "here's what actually
happened" post that does well there, as long as it reads as a lesson rather than a pitch.
Post as a text post.

**Suggested title:**
I built a feature 91% of users never touched, and still took five weeks to remove it

**Body:**

I make a small iOS app called Appray, so take this with whatever grain of salt that
requires. This isn't a launch post, just something that happened last month that felt
worth writing down.

About six weeks after launch I added a slider under each question in the app: how sure
are you of the answer you just gave, one to five. The idea was that an answer someone was
confident about should probably count for more than one where they were guessing. Took
about a week and a half to build, including an animation on the handle I was pretty proud
of.

Nobody touched it. I added basic logging and after a month, 91% of sliders were sitting
exactly where they opened, dead centre. Not because everyone felt exactly medium about
everything, just because a slider under a question you're already thinking hard about is
one more decision nobody asked for, and the path of least resistance is to leave it alone.

I knew this within three weeks. I didn't remove it for another two. Partly ordinary sunk
cost, I'd spent real hours on it and there's a specific reluctance to undoing something
you were proud of. Partly something dumber: cutting an idea from a list is invisible,
removing a shipped feature shows up in a changelog someone can read, and some part of me
treated that as admitting a mistake in public rather than as normal maintenance.

What actually moved me wasn't the 91% number, I'd had that for two weeks and it changed
nothing. It was a support email. Someone asked what the slider was for and whether they
were doing it wrong by leaving it centred. Third person to ask something like that. Three
people is a small sample, but it told me the feature wasn't neutral, it was quietly making
a few people stop and second-guess a control that did almost nothing.

Then I removed it and said nothing about it anywhere, which was its own small mistake. Two
of those same three people wrote back later asking if I'd pulled it on purpose or if
something broke. A silent removal reads as a bug, not a decision, even for a feature
almost nobody used. I write a changelog line for removals now, every time.

---

## 2. Quora — answering an existing question

**Question found (real, currently indexed on Quora):**
"When should you remove features from a product?"
https://www.quora.com/When-should-you-remove-features-from-a-product

This is a direct match for the blog post's exact topic, which is why it's worth answering
as asked rather than writing something generic. Keep the product mention to one line near
the end, and check the question is still open (unlocked, accepting answers) before posting,
since Quora questions occasionally get closed or merged.

**Answer draft:**

I make Appray, an app that gives founders a Build, Kill or Prove verdict on the features
they're weighing, so I've had to think about the "kill" side of this more than most.
Removing something you already shipped is a different problem from not building it in the
first place, and most of what's written about prioritisation only covers the second one.

Two things have mattered more than any framework:

Usage data tells you a feature is dead, but it rarely tells you when to act on that. I once
knew for three weeks that a feature of mine was doing almost nothing (91% of users left a
confidence slider on its default setting) and did nothing about it, because a number you
already expected doesn't feel like new information. What actually moved me was a support
email asking what the control was for. Small sample, but it told me the feature wasn't
neutral, it was quietly costing a few people a moment of confusion in an app whose entire
pitch is respecting their time.

Removing it well matters as much as removing it. I pulled the feature and said nothing
about it anywhere, on the theory that a feature nobody used didn't need an announcement.
Wrong. A couple of the people who'd asked about it wrote back later assuming something had
broken. Somebody already has a mental model that includes the thing you're cutting, however
few people that is, and silence reads as a bug rather than a decision. A one-line changelog
note costs almost nothing and prevents that.

The harder part honestly isn't the data or the announcement, it's admitting a shipped
decision was wrong on a timeline nobody is forcing on you. That's a slower, separate skill
from deciding what to leave out before you start.

---

## 3. Hacker News — Ask HN

**Framing:** this fits better as a fresh Ask HN submission than a reply to an old thread,
since the closest existing HN discussion of this topic (a 2017 thread on the sunk cost
fallacy in software) is long dead and replying there would reach nobody. Ask HN posts that
pose a genuine question and back it with a specific, concrete example tend to get real
engagement rather than getting flagged as promotional. Keep the product mention to one
line, after the actual question and story.

**Suggested title:**
Ask HN: How do you decide to kill a feature you've already shipped?

**Body:**

Curious how others handle this, because I clearly don't have a good process for it yet.

I added a feature to my iOS app (Appray, a decision tool for founders, so I'm not a
neutral party here) that turned out to do almost nothing. A confidence slider under each
question, one to five, meant to weight answers by how sure someone was. Logging showed 91%
of users left it at the default after a month. I knew this within three weeks and sat on it
for two more before removing it, mostly out of ordinary sunk cost and a weird reluctance to
put a "removed X" line in a changelog where people could see it.

What actually got me to act wasn't the usage number, it was a support email from someone
asking what the slider was for. Data told me it was dead. A person told me it was actively
costing someone a moment of confusion, which turned out to matter more.

Then I made a second mistake and removed it silently, no changelog note, reasoning that an
unused feature didn't need an announcement. Wrong: a couple of the same people who'd asked
about it wrote back later assuming something had broken.

For people who've shipped and later killed something: what actually triggers the decision
for you, and do you announce removals or let them go quiet?
