# Community drafts — 12 October 2026

Ready-to-post drafts for the blog post "Appray used to run on GPT-4. I pulled it after three
weeks." (https://appray.app/blog/appray-used-to-run-on-gpt-4/). DRAFTS ONLY. Nothing here has
been posted. Mariia reviews and posts these herself.

## 1. Reddit — r/ArtificialIntelligence

**Why this subreddit:** It's a large, general-audience sub for real experiences with AI
capabilities and limitations, not a vendor pitch board, and this story is specifically about
discovering GPT-4's non-determinism the hard way inside a shipping product. Note r/Entrepreneur,
r/EntrepreneurRideAlong, r/SaaS, r/microsaas, r/startups, r/iOSProgramming, r/ProductManagement,
r/indiehackers, r/SideProject and r/mobiledev have all been used in previous rounds of these
drafts, so r/ArtificialIntelligence keeps this from repeating a subreddit.

**Suggested title:** I ran the same 8 answers through GPT-4 forty times. Got 14 different verdicts.

**Post body:**

I make Appray, a small iOS app that argues a feature idea through eight rounds of questions and
ends in a Build, Kill or Prove verdict. Solo founder, based in Croatia. For the first three weeks
of building it, that verdict wasn't a rule, it was a GPT-4 API call.

It worked well enough, fast to build, four days from nothing to a working prototype, and it
sounded confident every single time. The problem showed up almost by accident. I was retyping the
same eight answers into the app for demo copy, not pasting them, and got three different verdicts
across three runs: Kill, then Prove, then Build with a full paragraph justifying it.

So I ran the exact same input, character for character, forty times in a row. Fourteen of the
forty came back different from the majority verdict. Not hedged, not "it depends," flat
contradictions delivered with the same even, confident tone each time. That's the part I keep
coming back to: confidence in the output told me nothing about whether the input had actually
been understood consistently.

I ended up rewriting the whole verdict engine as a plain decision tree in Swift, no model
involved, nineteen explicit rules. Took five weeks instead of four days, and it's genuinely worse
than GPT-4 was at handling answers that don't fit neatly into a category. But it gives the same
answer every time, and I can point to the exact rule that fired. For a product whose entire pitch
is "the same situation gets the same answer," that mattered more than I expected it to going in.

Not anti-AI as a blanket position, it's useful for the parts of the job that don't need to be
repeatable (drafting interview questions, say). Just don't let it be the verdict if the verdict is
supposed to mean something consistent.

Full write-up with the actual forty-run test is here if useful:
https://appray.app/blog/appray-used-to-run-on-gpt-4/

Anyone else here built something on an LLM and then had to rip it back out once consistency
turned out to matter more than you'd planned for?

---

## 2. Quora — answering an existing question

**Question found (real, currently live):** "Do you validate your startup business ideas with
ChatGPT?" https://www.quora.com/Do-you-validate-your-startup-business-ideas-with-ChatGPT

**Answer:**

I'm Mariia, I make a small iOS app called Appray, and I can answer this from an angle most people
replying here probably haven't: I actually tried building the core decision logic of my product
on top of GPT-4, not just using it for brainstorming, and ended up pulling it out.

Short version: for three weeks, Appray's verdict (whether a feature idea is a Build, Kill or
Prove) came straight out of a GPT-4 call. It worked, until I noticed I was getting different
verdicts for the exact same input depending on small, meaningless differences in how I'd typed
the answers. I tested it properly: forty runs of the identical input, and fourteen came back
contradicting the majority verdict, with zero hedging in the language, just flat confident
disagreement with itself.

That's the real risk with using ChatGPT (or any LLM) to validate an idea: it will give you an
answer that sounds certain, and that certainty tells you nothing about whether you'd get the same
answer tomorrow, or if you'd phrased the question slightly differently today. If you're using it
to generate questions to ask real customers, spot an angle you hadn't thought of, or organize your
own notes, it's genuinely useful for that. If you're using its verdict as the validation itself,
you're trusting a coin that looks confident about which side it landed on.

The thing that actually validates an idea is still the boring thing: real people, real commitment,
repeated use or money changing hands. AI can speed up getting to that conversation. It can't
replace having it.

I wrote up the full story, including the forty-run test, here:
https://appray.app/blog/appray-used-to-run-on-gpt-4/

Posting note: reconfirm the question is still open before posting, Quora questions get merged or
go stale. If so, a close substitute is any live thread asking whether ChatGPT can validate a
business idea or app idea, the forty-run test is the actual answer worth keeping regardless of
which exact question it lands under.

---

## 3. Indie Hackers — reply to an existing thread

**Why this framing fits:** There's a live Indie Hackers post specifically about AI
non-determinism breaking products, with a builder and commenters already discussing the exact
problem Appray ran into. Replying there puts this in front of people already mid-conversation
about it, rather than competing for attention with a fresh post.

**Thread to reply to:** "Building with AI? Here's the problem." —
https://www.indiehackers.com/post/building-with-ai-heres-the-problem-ba45abdb20

**Reply:**

Hit this exact wall, from the product side rather than the tooling side. I make Appray (solo
founder, Rijeka, Croatia), a small iOS app that turns eight interview answers into a Build, Kill
or Prove verdict on a feature idea. For the first three weeks, that verdict was a GPT-4 call, not
a rule.

It felt fine until I retyped the same answers for demo copy instead of pasting them and got a
different verdict three times running. So I tested it properly: identical input, forty runs,
fourteen came back contradicting the majority, every one delivered in the same confident tone as
the rest. No hedging, just flat disagreement with itself.

Rewrote the whole thing as a decision tree in Swift, nineteen explicit rules, no model. Took five
weeks instead of four days and it's worse than GPT-4 at handling messy, not-quite-yes-or-no
answers. But it's the same answer every time the input's the same, which turned out to be the
actual requirement I hadn't written down anywhere, because I'd assumed it.

Full writeup, including the forty-run test, here if it's useful to anyone working through the
same tradeoff: https://appray.app/blog/appray-used-to-run-on-gpt-4/
