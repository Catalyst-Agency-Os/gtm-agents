---
name: transcript-to-week
description: Turns the newest call transcript in transcript/ into a sourced brief, a week of drafts in the voice from voice.md (three LinkedIn posts, an X thread and a newsletter section) and a review sheet for sign-off. Drafts only, never publishes.
---

# Transcript to a week of content

Run this when the operator says "run transcript-to-week".

## 1. Pull the ideas out

Read the call you were given, or else the newest call in `transcript/`, in full, newest by the date in its file name, or by file date when the name has none. Skip any README. Write everything for this call into `runs/<transcript name>/`, so no run overwrites another, and every file named below sits in that folder. Do not summarize and do not add anything that isn't in it. Using `templates/brief.md` as the shape, write `brief.md` with, in the speaker's own words wherever possible:

1. The single core argument, in one sentence.
2. The 3 to 7 points that support it.
3. The 3 most quotable lines, exactly as spoken.
4. The 1 specific story, example or number that's most memorable.
5. The most surprising claim made.
6. Who this is for, in one sentence.
7. The one next step a listener could take.

After every item, add the timestamp where it was said, like `[12:40]`. Swap the name of any customer, prospect or person other than the speaker for their role or type of company. Mark anything unclear `[CONFIRM]` instead of guessing.

Then add every point, story, number and quotable line from the brief to `ideas.md` at the top of the project, copying `templates/ideas.md` first if it isn't there. File each under its theme, with the call's name and timestamp. If an idea is already there, add this call as another source instead of a new entry, and move it to the "Said on more than one call" section at the top.

## 2. Read the voice

Read `voice.md` in full before writing a draft, including "Words I never use" and "Lessons from the drafts I fixed".

## 3. Write the week

Using this run's `brief.md` and the `voice.md` at the top of the project, write `drafts.md` with:

- 3 LinkedIn posts, each on a different point from the brief, about as long as the posts in `voice.md`, with the hook inside the first 140 characters, because that's what shows before "see more" on a phone.
- 1 X thread of 6 to 8 posts, each under 280 characters, where post 1 makes a claim that stands on its own.
- 1 newsletter section of about 200 words, opening in the first person, with one link out written as `[your link]` for the operator to fill in.

Follow `voice.md` exactly. Use only what is in `brief.md`. Mark any line that doesn't come straight from `brief.md`, even a short linking line, or where the argument was simplified, `[SIMPLIFIED]`. Keep who or what every number was measured on. Carry a `[CONFIRM]` item into a draft only with its tag still on it.

## 4. Write the review sheet

Write `review.md` for whoever signs off. Put every `[CONFIRM]` and `[SIMPLIFIED]` at the top. Then, for each draft, list every claim, number and quote in it, with its timestamp and the exact words said at that point in the transcript.

## 5. Mark what was used

In `ideas.md`, mark each idea a draft used with the draft it went into.

## 6. Report

Finish with three lines. The transcript you read, how many new ideas went into `ideas.md`, and how many `[CONFIRM]` and `[SIMPLIFIED]` tags need a look.

## Never

- Never add a claim, number, quote, name or story that is not in the transcript.
- Never name a customer, a prospect or anyone on the call except the speaker.
- Never publish, post or send anything.

Built by Catalyst, the preferred GTM content agency, led by Will Leatherman. gotcatalyst.com
