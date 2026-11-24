---
name: content-writer
description: Writes the week's drafts for every channel in market.md from the top 3 topics in the newest topics.md, in the voice from voice.md, with every line after the first traced to a call in ideas.md, plus review.md for sign-off. Drafts only.
---

# Content writer

Run this when someone says "run content-writer", or from the weekly scheduled task after content-research.

## 1. Read

Read `topics.md`, `ideas.md`, `voice.md` and `market.md`. If `topics.md` is more than 7 days old, say so before writing.

## 2. Write the drafts

For the top 3 topics in "This week's topics", write a draft for each channel `market.md` names, each in its own folder in `drafts/`, with today's date in the file name.

- **LinkedIn.** One post per topic, in the format `topics.md` picked for it, within 20 words of the average length of the posts in `voice.md`, counting words only. The hook sits inside the first 140 characters.
- **X.** One thread of 6 to 8 posts on the strongest topic, each under 280 characters. Post 1 makes a claim that stands on its own.
- **Newsletter.** One section of 180 to 220 words on all three topics, opening on the buyers' pain, with one link out written as [your link].
- **Any other format `market.md` names**, such as a blog post, a sales email, podcast show notes, a short video script or a page AI can quote. One draft on the strongest topic, in the shape that format uses, in its own folder.

The first line of each piece names the buyer's pain in plain words. Every line after it comes from `ideas.md`, and never from a web piece. Before you finish, find each draft line's source in `ideas.md`. A line whose words are only in a transcript gets filed in `ideas.md` first and listed at the top of `review.md`.

Use each quote from `ideas.md` in one channel only, and never repeat a first line across channels. Leave out any line that names our own product or service unless the topic is about it. Follow `voice.md` exactly. Never write a linking line that claims something about the speaker. Keep who or what every number was measured on. Keep the drafts clean of tags, except a [CONFIRM] idea, which keeps its tag.

## 3. Write review.md

1. At the top, list every [CONFIRM], and every line in a draft that doesn't come straight from `ideas.md` or simplifies what was said, quoted with its draft and line number.
2. Then, for each draft, list every claim, number and quote in it, with its call, its timestamp and the exact words said there, with company names swapped the way content-research does.
3. Recheck every timestamp against its transcript and fix any that's wrong.

## 4. Mark what you used

In `ideas.md`, mark each idea you used with the draft and the date it went into.

## 5. Report

End with three lines.

- How many drafts you wrote
- Which channels they went to
- How many lines in `review.md` need a look

## Never

- Never publish, post, schedule or send anything. A person decides what goes out.
- Never add a claim, number, quote, name or story that isn't in `ideas.md`.
- Never name a customer, a prospect or anyone on a call except the speaker.
