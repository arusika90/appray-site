# Community drafts — 1 October 2026

Three drafts, built around today's blog post ("Should I translate Appray into other
languages?"). All are drafts only. Nothing here has been posted, submitted, or automated.
Mariia posts these herself, if and when she wants to, and should read each one and adjust to
taste first (tone, exact numbers, whether the link belongs at all) before using it.

---

## 1. Reddit — r/mobiledev

**Why this subreddit:** r/mobiledev is a long-running community (since 2010) for developers
building iOS, Android and cross-platform apps, where implementation-level problems get genuine
discussion rather than just marketing advice. This post fits because it isn't the usual
"which languages should I localize into" question, it's a specific engineering problem that
anyone who generates UI text dynamically (not just from a fixed strings file) will eventually
hit: grammatical case breaks template-based text the moment you insert a word you don't control.
That's a narrow, concrete hook likely to get real replies from people who've solved it, rather
than generic localization-tool recommendations. Post as a text post.

**Suggested title:**
Why I can't just drop my app into a translation tool: grammatical case breaks my templates

**Body:**

I make a small iOS app called Appray, a Build/Kill/Prove decision tool for founders, so this
isn't a huge app, but the problem is one I think any of you doing dynamic UI text will hit
eventually.

Appray's interview isn't static copy. It generates follow-up questions by inserting whatever
text the user typed into a sentence template, something like "Who specifically asked for
{feature}?" becomes "Who specifically asked for the CSV export?" using the user's own words. In
English that's a trivial string insert, because English barely inflects nouns for case.

I have 26 support emails from German, Croatian and Italian users (all written in fluent English,
which is its own story), and I started looking seriously at localizing. Store listing
translation is easy, static text, done once. The interview engine is not. Croatian has seven
grammatical cases. The ending on an inserted noun phrase changes depending on the preposition
before it and the noun's gender, and I don't know the gender in advance because the user typed
the phrase, not me. German is gentler, three genders and four cases, but you still need to know
whether something is der, die or das before you can put an article in front of it, and an
arbitrary English phrase a stranger typed doesn't arrive with that metadata attached.

I spent most of a weekend trying to dodge this by rewriting templates so nothing needed to
decline, things like "Regarding {feature}, who asked for it first?" Technically works.
Reads like a government form in every language I tried it in, including English, which defeats
the point of a tool whose whole job is to feel like it's actually talking to you.

So for now: store listing translated, in-app interview still English-only, decision on hold
until I have an actual plan for case-aware templates rather than a workaround that makes the
product worse to use.

Has anyone here actually solved this properly, for a language with real declension, without
either hardcoding a huge rule table or just writing around the problem like I did? Genuinely
curious whether there's a known approach I haven't found, or whether everyone just avoids
inserting user text into grammatically live positions.

---

## 2. Quora — answering an existing question

**Question found (verified live via search):** "What languages are worth localizing your app
into other than English? Would you do all languages at once, or continuously add more?"
https://www.quora.com/What-languages-are-worth-localizing-your-app-into-other-than-English-Would-you-do-all-languages-at-once-or-continuously-add-more

This fits well because the asker is weighing exactly the decision this week's post is about,
which languages are worth it and whether to commit all at once. My answer gives a real,
numbers-based example of staging the decision (translate the store listing first, hold the
in-app translation until there's a reason to believe it pays off) rather than a general list of
"top 5 languages to localize into." Confirm the question is still open before posting, Quora
questions occasionally get merged or closed.

**Answer draft:**

I'm a solo founder, I make a small iOS app called Appray, so this is one data point rather than
a rule, but I'd push back gently on doing "all languages at once" even if you can afford the
translation cost, because the cost that actually bit me wasn't the translation, it was finding
out afterward that the market didn't move.

Here's what I actually looked at before deciding. App Store Connect gives every developer a free
breakdown of downloads by country already, no analytics SDK needed. For my app that's the US at
51%, Germany second at 9%, ahead of the UK at 7%. So Germany looked like a real target. But
nobody in Germany had actually asked me for a German version, the support emails I do get in
German are written in careful English.

Rather than translate the whole app on a guess, I translated only the App Store listing into
German last week, description and screenshot captions, which is static text and costs an
afternoon, not an engineering project. That's the part of localizing that reliably moves
downloads on its own, because the App Store surfaces apps differently once there's local-language
metadata attached, independent of whether the app itself is translated. I'm watching whether
German downloads move over the next month before deciding whether the much more expensive step,
translating the actual product, is worth doing at all.

So my answer to "all at once or continuously add": neither, really. Stage it by cost. Store
listings are cheap and reversible, do the ones your download data already supports. Treat full
in-app translation as a separate, much bigger decision you only make once a translated listing
has actually proven the market responds, not as the same project with more languages bolted on.

---

## 3. Indie Hackers

**Why this framing fits:** Indie Hackers rewards posts that show the actual decision-making
process behind a founder's choice, with real numbers, rather than a how-to guide. This story
has a clean Build/Kill/Prove shape (translate the store listing as a cheap Prove step before
committing to the expensive in-app work) which is exactly the kind of staged, numbers-led
reasoning the community responds well to. Post to the main feed, not as a product pitch.

**Suggested title:**
I almost localized my whole app on a guess. Translated the App Store listing instead.

**Body:**

Quick one from building Appray, a decision tool for founders (Build/Kill/Prove verdicts on
features, no AI, nothing leaves the device).

26 support emails in the last ten months have come in German, Croatian or Italian, always
written in fluent, careful English. None of them has ever asked me to translate the app. That
combination made me assume localizing wasn't worth thinking about, until I actually looked at
App Store Connect's free country breakdown: US 51%, Germany 9% (second place, ahead of the UK
at 7%), Croatia under 1%.

So there's a real German market and real German-speaking users, and the request still isn't
coming. I think the job isn't "I can't read this," it's something closer to wanting to do honest
self-interrogation in your first language rather than your second, which doesn't show up in a
support inbox because nobody writes an email explaining their own cognition to a stranger.

Full in-app translation for Appray is genuinely expensive to do right, the interview generates
questions from templates that insert the user's own words, and languages with grammatical case
(Croatian has seven, German has four plus three genders) break that the moment you insert a word
you don't control the gender or case of. I burned a weekend confirming this before admitting it
needs an actual engineered solution, not a weekend hack.

Instead I did the cheap version first: translated the store listing only (description,
screenshot captions) into German, an afternoon of work, zero changes to the product. That's the
part of localizing that moves the needle on its own in a lot of cases I read about researching
this, because the App Store itself treats a listing with local-language metadata differently in
local search, independent of what language the app is actually in.

Now I wait a month and check whether German downloads move. If they do, that's a real signal the
market will tolerate an English product it found in its own language, which tells me the in-app
work might be worth the engineering cost. If nothing moves, I've learned that cheaply instead of
mid-way through a much bigger build.

Basically treating "should I localize" the same way I'd treat any other feature here: cheapest
possible test first, commit to the expensive version only once the cheap one says something.

---

**Status note for Mariia:** store listing translation is real (confirm the exact German copy
before quoting it anywhere), the download numbers above are the ones cited in today's blog post,
double check them against the live App Store Connect dashboard before posting any of these,
since they may have moved since the post was written.
