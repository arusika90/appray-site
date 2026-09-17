# Community drafts — 17 September 2026

Three drafts, built around the new blog post ("What I actually do with every feature request
that comes in"). All are drafts only. Nothing here has been posted, submitted, or automated.
Mariia posts these herself, if and when she wants to, and should read each one and adjust to
taste first (tone, exact numbers, whether the link belongs at all) before using it.

**Note on this run:** web search was unavailable for the whole session, so unlike previous
community drafts I could not search live to find or verify a real, currently open question or
thread to reply to. Draft 1 (Reddit) and draft 3 (Ask HN) don't depend on that, they're original
posts to a named community rather than replies, so they're ready as they are. Draft 2 (Quora) is
different: I've written the answer but could not confirm a specific live question exists to post
it under. Read that section's note before using it.

---

## 1. Reddit — r/indiehackers

**Why this subreddit:** r/indiehackers is where solo and small-team builders post process detail
rather than launch announcements, and "here's the actual system, warts included" is exactly what
does well there. The post admits a real screwup (a pattern missed for eight weeks across three
channels), which fits the sub's appetite for honesty over polish. Post as a text post.

**Suggested title:**
My entire feature roadmap is a plain text note with about forty lines in it, and I think that's the whole trick

**Body:**

I make a small iOS app called Appray, so keep that in mind reading this. Not a launch post,
just something about how I actually run the backlog that I've been meaning to write down.

Early on I built a proper roadmap board. Columns, drag and drop, vote counts on cards. Used it
for about three weeks and quietly stopped opening it. The problem wasn't the tool, it was what
the tool did to my head. The second a request has a card sitting in a column called
"Considering," it looks like a decision has half been made already. I caught myself defending
things I'd never actually agreed to build, purely because deleting a card felt more final than
deleting a line of text.

So now it's a plain note. Nothing in it looks like a commitment, so nothing in it costs anything
to remove. Requests come in through four channels, roughly in order of how much I trust them:
App Store reviews, support emails, my own notes while using the app myself, and the odd mention
on Reddit or Mastodon. None of it arrives labelled as a feature request, most of it is a
complaint or one line at the end of a five star review, and turning that into something
actionable is most of the actual work.

When I sit down to go through it, I'm not ranking anything by impact or effort. Three questions
per line: who is actually asking, is this the same story from more than one person who doesn't
know the others, and would I have thought of this myself if nobody had asked. That third one is
the one I trust least, my own ideas show up feeling urgent and fully formed with zero outside
prompting, and those are usually the ones that are fun to build rather than needed.

Where it actually failed me: for most of the summer I had a line reading "export, send to
accountant," attributed to one June email. Filed under watch, don't build, correctly, by the
system's own logic. It should have moved in July when a review mentioned the same thing in
different words. I didn't connect the two. It only became obvious in August when a third person
asked almost word for word what the June person had asked, close enough that I went and searched
my own inbox. Three requests, three channels, eight weeks, and a system built to catch exactly
this still missed it because I was reading each channel in isolation instead of cross checking
new lines against old ones. Built the export in four days once I finally saw it. Fixed my own
process to search existing lines before filing a new one, which is obvious in hindsight and
wasn't obvious while I was living inside three separate inboxes.

Curious how others here track this without it turning into either a spreadsheet nobody updates
or a public vote that just tells you who campaigns hardest.

---

## 2. Quora — answering an existing question

**Could not verify this run.** Normally I'd search Quora, find a currently open question that
matches the post's actual argument, and write the answer to fit it exactly, the way the last few
rounds of these drafts did. Web search was down for this entire session, so I can't confirm a
specific question is live right now or that its URL is still valid.

**Before posting this one:** search Quora yourself for something close to "How do I prioritize
feature requests from users?" or "How do you decide which feature to build next?", pick a
question that's actually open (not closed or merged), and check the answer below still reads as
a direct response to what was actually asked, adjusting the opening line if needed.

**Answer draft (to post once you've matched it to a real question):**

I make Appray, a decision tool that forces founders to weigh exactly this for a living, so I've
had to turn "read the feedback" into something closer to an actual process, mostly by getting it
wrong first.

The biggest change: I stopped ranking by importance and started asking three separate questions
about each request. Who is actually asking. Is this the same story from more than one person who
doesn't know the others. Would I have thought of this myself if nobody had asked. A single
person's request rarely becomes a build on its own, not because it doesn't matter but because
one description can be a misunderstanding, a one off situation, or a job only that person has.
The same story arriving from strangers who've never spoken to each other is the strongest signal
I've found, stronger than any vote count a roadmap tool ever showed me.

The mistake that taught me the most: a request for exporting data showed up in an email in June,
a differently worded App Store review in July, and a near identical email in August, three
channels, eight weeks apart, and I didn't connect the first two because I was reading each
channel separately instead of checking new requests against old ones. By the time I noticed the
pattern it had been sitting there for two months in three different places in my head. I built
the feature in four days once I actually saw it. Now I keep everything in one plain note
regardless of which channel it arrived through, and I search it before filing anything new.

I'd also add: don't build a public roadmap or voting board if you can avoid it. It changes what
people write. Instead of describing what actually happened to them, they start campaigning for
an outcome they've already decided on, and campaigning is a worse source of truth than a
complaint written by someone who has no idea you're reading it as data.

---

## 3. Hacker News — Ask HN

**Framing:** a fresh Ask HN submission rather than a reply to an old thread, since this is a
process question that ages fine as a standalone post and doesn't need a specific existing
discussion to attach to. Ask HN posts that state a real, specific mistake tend to get genuine
engagement rather than getting flagged as promotional. Keep the product mention to one line.

**Suggested title:**
Ask HN: How do you track and prioritize feature requests without a roadmap tool?

**Body:**

Genuinely asking, because my own answer to this is embarrassingly low tech and I'm not sure if
that's fine or if I'm about to hit its limits.

I make an iOS app (Appray, a decision tool for founders, so I'm not a neutral party here) and
every feature request lands in a plain text note. No board, no priority score. I tried a proper
board early on, columns and vote counts, and abandoned it after three weeks because the moment a
request has a card, it starts looking like a half made decision, and I found myself defending
things I'd never actually agreed to build just because deleting a card felt more final than
deleting a line.

What I actually check per request: who's asking, whether it's the same story from people who
don't know each other, and whether I'd have thought of it myself with nobody asking. That last
one is the one I trust least, my own ideas always feel urgent regardless of whether anyone needs
them.

Where this broke down: an export feature request came in through three different channels
(email, an App Store review, another email) over eight weeks, worded differently each time, and
I didn't connect them because I was reading each channel in isolation instead of searching old
requests before filing new ones. Took a third near identical message before I caught the
pattern. Built the feature in four days once I saw it.

For people who've been doing this longer than four months: does the plain note approach stop
working at some scale, and what did you replace it with when it did?
