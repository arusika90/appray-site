# Community drafts — 26 October 2026

Three ready-to-post drafts, built around today's blog post ("People asked for a Face ID
lock. That wasn't the actual problem.",
https://appray.app/blog/face-id-lock-request-wasnt-about-security/). DRAFTS ONLY. Nothing
here has been posted, submitted, or automated. Mariia posts these herself, if and when she
wants to, and should read each one and adjust to taste first (exact numbers, tone, whether the
link belongs at all) before using it.

---

## 1. Reddit — r/iosdev

**Why this subreddit:** r/iosdev is where people actually building iOS apps trade real
implementation detail, not just launch announcements, and this post is an implementation
story: LocalAuthentication versus a screenshot swap on `applicationWillResignActive`, which
is exactly the kind of specific, technical "here's what I actually shipped and why" post that
does well there. Note r/Entrepreneur, r/EntrepreneurRideAlong, r/SaaS, r/microsaas,
r/startups, r/iOSProgramming, r/ProductManagement, r/indiehackers, r/SideProject,
r/mobiledev, r/buildinpublic, r/UXResearch, r/ArtificialIntelligence and r/privacy have all
been used in previous rounds of these drafts, so r/iosdev keeps this from repeating a
subreddit, and it's a better fit for the technical angle than any of those would be.

**Suggested title:** Eleven users asked for Face ID lock. The fix that actually solved their
problem used zero auth APIs.

**Post body:**

I make Appray, a small iOS app, solo, no team. Over about four months, eleven separate people
emailed asking for a Face ID lock on the app. Reasonable request on its face, the app holds
whatever business idea someone's working on, and I went straight to sketching a
LocalAuthentication gate on launch before I actually reread what the emails said.

Once I read past the word "lock," eight of the eleven weren't describing a stolen phone at
all. They were describing handing an already-unlocked phone to someone else for a few
seconds, a kid grabbing it, a cofounder swiping one screen too far, or the app sitting visible
in the app switcher preview from twenty minutes earlier. A Face ID gate on open does nothing
for any of that, because in every one of those scenarios the phone is already unlocked and in
someone else's hand. Worse, it's a prompt every person pays on every single open to guard
against something that happens to a handful of people a handful of times a year.

What actually fixes the app-switcher case is the trick banking apps have used for years:
swap in a plain screen the instant the app resigns active, so the automatic screenshot iOS
takes for the switcher shows that instead of your real content, then swap back on return. No
new permission dialog, no daily friction, no auth framework at all. Took an afternoon, most of
it making sure the swap lands before the screenshot does.

Curious whether others here have hit the same gap between what a feature request names and
what it's actually solving for, and how you've caught it before building the wrong version.
Longer write-up, with the actual emails and what I built: 
https://appray.app/blog/face-id-lock-request-wasnt-about-security/

---

## 2. Quora — answering an existing question

**Question found (real, currently indexed on Quora):** "Does every app need a server?"
https://www.quora.com/Does-every-app-need-a-server

**Answer:**

No, and I run into this exact confusion a lot building Appray, a small iOS app that keeps
everything entirely on the device, no server, no account, nothing synced anywhere.

The honest line is: you need a server the moment you need something to exist independently
of any one phone, data shared across devices, other people needing to see it, or anything
that has to keep working while the app itself isn't open. If none of that applies, a lot of
what people assume requires a server doesn't.

A concrete example from my own app: people kept asking for a Face ID lock, which sounds like
backend territory, accounts, auth tokens, session handling. It isn't. iOS has a framework
called LocalAuthentication that checks Face ID and hands your app a yes or no, entirely on
the device, no network call involved. As it turned out I didn't even end up needing that
either, once I worked out what people were actually asking for was a way to stop the app's
contents showing in the switcher preview when the phone changed hands for a few seconds,
which is purely a local UI fix, nothing remote about it at all.

So the honest answer: plenty of genuinely useful app behaviour, reminders, local locks,
on-device search, offline storage, needs no server whatsoever. You need one specifically for
sync, multi-user state, or anything that has to survive the app being deleted and reinstalled.
Worth figuring out which category your feature is actually in before assuming it needs
backend work.

Write-up of the Face ID example, if useful:
https://appray.app/blog/face-id-lock-request-wasnt-about-security/

Posting note: reconfirm the question is still open before posting, Quora questions get merged
or go stale. If it's gone, "what kinds of apps don't need a backend" or "can an app work with
no server at all" are close live substitutes for the same answer.

---

## 3. Hacker News — Show HN style submission, with a first comment ready

**Why this framing fits:** This is a short, specific engineering post about a real
product decision, exactly the shape that does well as a plain link submission on HN, as long
as the submitter adds context themselves rather than letting the title alone carry it, which
is normal and expected practice there rather than self-promotion. An Indie Hackers reply
didn't fit this round, no live thread turned up that the Face ID angle would add real value
to, so this uses the HN framing the brief allows instead.

**Suggested submission title:** Eleven people asked for a Face ID lock. The fix needed no auth
API at all

**Submission URL:** https://appray.app/blog/face-id-lock-request-wasnt-about-security/

**First comment to leave on the submission (standard HN practice for the poster to add
context):**

Author here. I make Appray, a small iOS app, solo founder. Posting this because the gap
between what a feature request literally says and what it's actually solving for is something
I keep underestimating, and this was a clean enough example to write up properly.

Short version: eleven people over four months asked for a Face ID lock. I started building
exactly that, LocalAuthentication gate on app open, before rereading the emails properly.
Most of them weren't worried about a stolen phone, they were describing an already-unlocked
phone changing hands for a few seconds, which a launch-time Face ID prompt does nothing for.
The actual fix was swapping in a blank screen the instant the app backgrounds, so the
automatic app-switcher screenshot iOS takes doesn't show real content, the same trick banking
apps use. No new permission, no daily friction, about an afternoon of work.

Happy to get into the implementation detail if anyone's curious, or hear where this kind of
mismatch has bitten others.

Posting note: confirm there isn't already a very similar Show HN or discussion up before
submitting, and post at a weekday daytime slot in US time for the best chance of visibility,
per usual HN norms.

---

**Reminder for Mariia:** all three are drafts. Nothing has been posted, submitted, or
automated on Reddit, Quora, Indie Hackers, or Hacker News. Review tone and the exact numbers
against your own memory of the eleven emails before posting any of these yourself.
