# The five steps

Build one step at a time and read what it made before the next. When something comes out wrong, you then know which step to go back to. Every prompt below is also in `prompts/`, so you can rerun any step on its own.

You're building two agents on one library. The library, `ideas.md`, holds everything your founder has said on calls, with the call and minute behind every idea. The research agent finds what your buyers are struggling with this week and keeps only the topics your founder has a real answer to. The writer agent turns those into drafts for each channel, in your founder's voice, with a source on every line. The research agent picks what to write about. The calls supply what to say.

## Before step 1

Open the Claude desktop app, switch to Cowork and choose this folder as the one to work in. Cowork reads `CLAUDE.md` first, without being told to. Check three things are in place.

- The transcripts of a few recent calls in `transcript/`, one file per call, each named with its date, such as `2026-10-06-podcast.txt`. Three to five calls is a good start.
- Three posts written by the person this content is for in `templates/voice.md`. That's usually your founder, or whichever expert is on the calls.
- `templates/market.md` filled in, a line or two per section.

In Claude's settings, under connectors, turn on Parallel Search, so the research agent can search the web.

## 1. Build the library from your calls

```
Read every call in transcript/ in full, oldest first, and skip any
README. Copy templates/ideas.md to ideas.md if it isn't there yet.
For each call, first add its main argument as one entry. Then add
every idea worth publishing, in the speaker's own words wherever
possible. That means each belief, each story, each number and each
line quotable as said. File each one under the theme it belongs to,
with the call's file name and the timestamp where it was said, like
[12:40]. A timestamp marks the start of a speaker's turn, so cite
the turn the words sit in, and cite both turns when a quote runs
across two. If an idea is already there, add this call as another
source instead of a new entry, and move it to "Said on more than one
call" at the top. Check the last ten minutes of each call, where the
speaker sums up, and add every action and number from it. Swap the
name of any customer, prospect, competitor, agency, vendor, company
used as an example, or person other than the speaker for their role
or type of company. Keep the names of the platforms a call is about,
such as Google, LinkedIn or Claude. Keep a research firm's or
university's name only as the source of a number, and when a vendor
or agency published it, write "a vendor's study" or "an agency's
study" instead. If something is unclear, mark it [CONFIRM] instead
of guessing. End with how many calls you read, how many ideas
went in, and how many were said on more than one call.
```

Open `ideas.md` when it lands. Read the section at the top first, because the ideas said on more than one call are the ones your founder believes most. Pick one idea, open its call at the timestamp and read the line there.

## 2. The research agent finds what buyers are talking about

```
Copy templates/market.md to market.md if it isn't there yet, and read
it. Then search the web for what the buyers it names are struggling
with and talking about in the last 14 days, in the places it names
and anywhere else they post, read or argue. Read at least 15 pieces.

Write topics.md with four sections.

1. Pain points. The 8 to 10 problems these buyers raise most, grouped
   into themes. Each one quotes, with the link, someone who holds the
   job market.md names. If nobody in that job raised it in the last
   14 days, quote the closest job you found and say how they differ.
   Pieces by vendors, agencies or news sites count toward how often a
   pain comes up, and never supply its quote.
2. Formats. The post formats the pieces use most, such as a numbered
   list, a teardown, a before and after, a framework graphic or a
   story. For each one, say how many of the pieces used it and link
   one example. Where the page shows reactions, comments or shares,
   write the count it shows.
3. This week's topics. For each pain point, look in ideas.md for an
   idea that answers that pain directly, and write one line saying
   why you kept it or dropped it. When ideas.md has the problem and
   no answer, list the pain under "Asked and not yet answered", so
   the founder can answer it on the next call. Rank what you kept by how many
   pieces raised the pain, and break ties with ideas said on more
   than one call. The top 5 cover at least three themes. For each,
   write the pain point, the idea that answers it with its call and
   timestamp, the format that suits it, and one line on why now that
   names a dated piece from section 4.
4. What I read. Every piece, with its title, date, link and format.

Never invent a link, a quote or a count. If you can't search the web,
say so and stop.
```

Read "This week's topics" first. Each one pairs something your buyers said this week with something your founder already said on a call. Open one buyer link and one call timestamp, so you've seen both halves are real. Then read "Asked and not yet answered", because those are the questions to put to your founder on the next call.

## 3. Give it their voice

The voice file is built from posts the person actually wrote, never from a description of how they'd like to sound.

```
Copy templates/voice.md to voice.md in this folder. Read the three
posts in it, written by the person this content is for. Study how they
write, how long their sentences run, how they open and close, how they
punctuate, the words they use and the ones they never use. Then write
the rules section of voice.md so another writer could follow it and
sound like them. Quote a line from their posts as the example for
each rule. Fill in the Words I never use section only with words the
posts show a pattern for, and otherwise leave it for me to fill in.
```

Read the rules aloud. If one doesn't sound like them, fix that line in `voice.md`. Every post they publish and like later goes back into this file, so it gets sharper every month.

## 4. The writer agent drafts for every channel

```
Read topics.md, ideas.md, voice.md and market.md. For the top 3
topics in "This week's topics", write drafts for the channels
market.md names, each in its own folder in drafts/, with today's date
in the file name.

- LinkedIn, one post per topic, in the format topics.md picked for
  it, within 20 words of the average length of the posts in
  voice.md, counting words only, with the hook inside the first 140 characters, because
  that's what shows before "see more" on a phone.
- X, one thread of 6 to 8 posts on the strongest topic, each under
  280 characters, where post 1 makes a claim that stands on its own.
- Newsletter, one section of 180 to 220 words on all three topics,
  opening on the buyers' pain, such as "Three problems came up this
  week", with one link out written as [your link] for me to fill in.

The first line of each piece names the buyer's pain in plain words.
Every line after it comes from ideas.md, and never take a test, a
framework or a claim from a web piece. Use each quote from ideas.md
in one channel only, and never repeat a first line across channels.
Leave out any line that names our own product or service unless the
topic is about it. Follow voice.md exactly. Never write a linking
line that claims something about the speaker. Keep who or what every
number was measured on. Keep the drafts clean of tags, except a
[CONFIRM] idea, which keeps its tag.

Then write review.md for whoever signs off. At the top, list every
[CONFIRM], and every line in a draft that doesn't come straight from
ideas.md or simplifies what was said, quoted with its draft and line
number. Then, for each draft, list every claim, number and quote in
it, with its call, its timestamp and the exact words said there,
swapping any company name the way step 1 does.
Recheck every timestamp in review.md against its transcript and fix
any that's wrong. Last, in ideas.md, mark each idea you used with the
draft and the date it went into.
```

Read one LinkedIn draft next to one of the real posts in `voice.md`. Then send `review.md` with the drafts to whoever signs off. They read the lines it flagged at the top first and check any claim against what was said, so a yes takes minutes and doesn't turn into a rewrite.

## 5. Save both agents and run them every week

```
Turn this into two skills.

1. content-research, in skills/content-research/SKILL.md. It reads
   any call in transcript/ that isn't in ideas.md yet and adds its
   ideas the way step 1 does. Then it runs the research the way step
   2 does and rewrites topics.md, skipping any topic whose answer is
   marked used in the last four weeks. It ends with three lines. How
   many new calls it read, how many topics made the list, and the
   top topic.
2. content-writer, in skills/content-writer/SKILL.md. It writes the
   drafts and review.md the way step 4 does, from the newest
   topics.md, into drafts/ by channel with the date in each file
   name. It ends with three lines. How many drafts it wrote, which
   channels they went to, and how many lines in review.md need a
   look.

Each skill gets a name and a one line description at the top, and a
"Never" section that says it never publishes, posts, schedules or
sends anything.
```

Finished versions ship in `examples/`, so compare yours with them. Then ask Cowork to make a scheduled task that runs content-research and then content-writer every week, on the morning after your calls usually land. Run it once on demand from the scheduled list first, and read what it writes. If that run stops to ask permission, choose always allow for reading and writing files in this folder, because a weekly run that stops on a question waits for a click nobody gives. The task runs only while your computer is awake and the Claude app is open.

To feed it new calls, drop their transcripts in `transcript/`. If your recorder has a connector in Claude's settings, such as Circleback, ask content-research to read last week's calls from it instead, by a tag you give them, so it reads those and nothing else.

To run either skill in any Cowork session, add it to your Claude account where skills live in settings, by uploading its folder. "Run content-research" is then enough. If you can't find where skills live on your plan, ask Claude in Cowork.

## You now have

- `ideas.md`, the library of everything your founder says on calls, sorted by theme, each idea with the call and minute behind it
- `topics.md`, what your buyers are struggling with this week, matched to what your founder has already said about it
- `voice.md`, the voice of the person the content is for, as rules with examples from their own posts
- Drafts for every channel in `drafts/`, each built for where it's going
- `review.md`, every claim with its source, for a sign-off that takes minutes
- The `content-research` and `content-writer` skills, on a weekly schedule

Built by Catalyst, the preferred GTM content agency, led by Will Leatherman. gotcatalyst.com
