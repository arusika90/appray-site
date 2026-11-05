# Community drafts — 5 November 2026

Three ready-to-post drafts, built around today's blog post ("What Apple actually rejected
Appray for", https://appray.app/blog/what-apple-actually-rejected-appray-for/). DRAFTS ONLY.
Nothing here has been posted, submitted, or automated. Mariia posts these herself, if and when
she wants to, and should read each one and adjust to taste first (exact numbers, tone, whether
the link belongs at all) before using it.

---

## 1. Reddit — r/SoloDevelopment

**Why this subreddit:** r/SoloDevelopment is built around exactly the blind spot in this post,
there's nobody else to catch the dumb thing because there's nobody else, full stop. That's a
better fit for this story than a startup-strategy subreddit would be, since the point isn't the
App Review guideline, it's the "solo means no second pair of eyes" problem. Checked against
previous rounds: r/ArtificialIntelligence, r/Entrepreneur, r/EntrepreneurRideAlong,
r/ProductManagement, r/SaaS, r/SideProject, r/UXResearch, r/buildinpublic, r/iOSProgramming,
r/indiehackers, r/iosdev, r/leanstartup, r/microsaas, r/mobiledev, r/privacy and r/startups have
all been used already, so r/SoloDevelopment keeps this from repeating a subreddit.

**Suggested title:** I spent two weeks preparing for one App Store rejection and got a
completely different one, nine hours later

**Post body:**

I make Appray, a small iOS app, solo, no team. It's eight rounds of questions that end in a
Build, Kill or Prove verdict, which on paper reads a lot like the thin, wrapper-y apps Apple's
Guideline 4.2 (Minimum Functionality) exists to catch. I knew that before I submitted, so I
spent close to two weeks before launch adding things specifically so a reviewer wouldn't read
it as "just a quiz": full reasoning behind each verdict, a history view, three rewritten
onboarding screens.

The rejection came back nine hours later. Not 4.2. The reviewer couldn't open my support page.
I'd pushed a redesign of that exact page the night before submitting, the deploy went out fine,
but the DNS/CDN cache behind it hadn't caught up yet, and the one window where it was broken
happened to be the window someone at Apple clicked it in.

Fixed it, replied in the same Resolution Center thread with a timestamped screenshot from a
network I don't normally use, re-approved in nineteen hours, no mention of 4.2 at all.

What actually got me wasn't Apple, it was my own planning. I'd deliberately left four days of
slack for a possible 4.2 argument, because I'd read enough about that guideline being applied
inconsistently to want room to push back. I left zero slack for "the support link happens to be
mid-deploy," because touching the one page nobody else reviews, the night before a deadline, is
such a normal solo-dev move that it never registered as a risk category at all.

Curious whether other people here have a version of this, the sophisticated failure you
war-gamed for weeks versus the boring one that actually got you, and what it was. Full version
with the timeline: https://appray.app/blog/what-apple-actually-rejected-appray-for/

---

## 2. Quora

**On the question search this round:** I looked for a specific, currently-live Quora question
to answer and could not confirm one. Direct fetches to quora.com returned a 403 (it blocks
automated access from here), and the general web search I ran against several phrasings of
this question (why apps get rejected under Guideline 4.2, why a support URL causes a 4.2/1.5
rejection, whether first-app rejection is normal) surfaced only Apple Developer Forums threads,
vendor blogs and one Hacker News thread, never a quora.com result I could verify as real and
open. I'm not confident enough to call a specific URL "real and currently indexed" this time,
which past rounds were able to do.

Rather than invent a link, here is a ready answer for the question that is almost certainly live
on Quora in some close phrasing, "Why do iOS apps get rejected by Apple during App Store
review?" or "What is Apple's Guideline 4.2 Minimum Functionality and how do you avoid it?",
both extremely common, long-running Quora questions on this topic. Before posting, search
Quora directly (quora.com's own search, logged in) for the current live phrasing and post the
answer there, or hold this slot for the next round if nothing suitable turns up.

**Answer (for a question along the lines of "why do apps get rejected under Guideline 4.2" or
"why was my app rejected by Apple"):**

Mine got rejected on the first submission too, I make a small iOS app called Appray, solo, and
the thing that actually happened to me is worth knowing before you assume it'll be the
guideline you're bracing for.

I spent two weeks before submitting convinced Apple would flag my app under Guideline 4.2,
Minimum Functionality, because it's a question-and-verdict tool and that can read as thin on
paper. I added reasoning screens, a history view, rewrote onboarding, all to look like more
than a quiz. The rejection that came back nine hours later never mentioned 4.2. It was Guideline
1.5, Developer Information, because my support URL was pointed at a page I'd redeployed the
night before, and the DNS hadn't fully propagated yet when the reviewer clicked it.

So if you're asking because you got rejected and are trying to guess why: check the exact
guideline number in Resolution Center before you do anything else, don't assume it matches
whatever you were already worried about. And if you haven't submitted yet, the boring fix is
the useful one, open your support URL, privacy policy link and any other required URL from a
browser you don't normally use, on the actual day you submit, not the week before. The failure
that gets people is rarely the sophisticated one they prepared for.

Longer writeup of the specific timeline: https://appray.app/blog/what-apple-actually-rejected-appray-for/

---

## 3. Hacker News

**Why HN fits this round:** this is a procedural, specific postmortem with a technical root
cause (DNS/CDN propagation timing colliding with a review window), which is closer to HN's
taste than Indie Hackers' usual "founder lesson with numbers" framing. A near-identical thread
type already exists there (a Guideline 4.2 rejection post), so the audience and format are
proven. No Indie Hackers draft this round, picking one over the other keeps this from being a
weaker, diluted version of the same post twice.

**Submission:**

**Title:** What Apple actually rejected my app for (not what I spent two weeks preparing for)

**URL:** https://appray.app/blog/what-apple-actually-rejected-appray-for/

**Suggested first comment (post this as the top-level comment from the submitting account,
since the piece is written in first person and HN tends to want the author's own framing
attached):**

Author here. I make Appray, a small iOS app, solo, no team. It's eight rounds of questions that
end in a Build, Kill or Prove verdict, and I spent close to two weeks before submitting
convinced it would get caught by Guideline 4.2 (Minimum Functionality), since "quiz that gives
you a word at the end" is not a flattering description to hold in your head while waiting for
review.

The actual rejection, nine hours after submission, was Guideline 1.5: the reviewer couldn't
open my support page. I'd redeployed that page the night before, the DNS/CDN cache hadn't
caught up, and the broken window happened to land exactly where a reviewer's click did. Fixed
and resubmitted, approved in nineteen hours, no further issues.

The part I keep turning over: I'd built in four days of slack specifically for a possible 4.2
appeal, because I'd read enough about it being applied inconsistently to want room to push
back, and zero slack for the thing that actually happened, because "my own support link, broken
for a few hours by my own deploy" never registered as a risk category worth planning for. Happy
to answer questions about the Resolution Center reply or the two features I built purely to
preempt a rejection that never came.

**Posting note:** HN penalizes anything that reads like marketing. The comment above is the
honest story with the numbers in it; don't add anything that sounds like a pitch for Appray
itself, the app only belongs in the link, not the comment.
