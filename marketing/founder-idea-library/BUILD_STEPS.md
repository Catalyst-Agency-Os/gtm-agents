# The five steps

Build one step at a time and read what it made before the next. When something comes out wrong, you then know which step to go back to. Every prompt below is also in `prompts/`, so you can rerun any step on its own.

What you're building is a library of everything your founder says on calls, `ideas.md`, with the call and minute behind every idea. It grows with every call, and every piece of content draws from it. The drafts sound like the person they're for. Every claim traces to a timestamp in the call. It runs on calls your team already records. And whoever signs off can approve it in minutes, because every line shows where it came from.

## 1. Open the folder in Cowork

Open the Claude desktop app, switch to Cowork and choose this folder as the one to work in. Cowork reads `CLAUDE.md` first, without being told to. That file carries the one rule everything else depends on, which is to work only from what was said on the call and never invent.

Check the two inputs are in place before step 2. The transcript of a call goes in `transcript/`, named with the date of the call, such as `2026-09-29-podcast.txt`. Three posts written by the person this content is for go in `templates/voice.md`. That's usually your founder, or whichever expert is on the call.

## 2. Pull the ideas out

This step writes a short brief of the call, with the timestamp of every item, and adds each idea to `ideas.md`, the library that grows with every call.

```
Read the call in transcript/ in full. Do not summarize and do not
add anything that isn't in the transcript. Using templates/brief.md as
the shape, write brief.md with, in the speaker's own words wherever
possible:

1. The single core argument, in one sentence.
2. The 3 to 7 points that support it.
3. The 3 most quotable lines, exactly as spoken.
4. The 1 specific story, example or number that's most memorable.
5. The most surprising claim made.
6. Who this is for, in one sentence.
7. The one next step a listener could take.

After every item, add the timestamp where it was said, like [12:40].
Swap the name of any customer, prospect or person other than the
speaker for their role or type of company. If something is unclear,
mark it [CONFIRM] instead of guessing.

Then copy templates/ideas.md to ideas.md if it isn't there yet. Add
every point, story, number and quotable line from brief.md to it,
under the theme it belongs to, with the call's name and timestamp. If
an idea is already there, add this call as another source instead of
a new entry.
```

Read `brief.md` when it lands. Pick one quotable line and find it at its timestamp in the transcript. Anything tagged `[CONFIRM]` is something to fix in the brief now, before a draft carries it. Then open `ideas.md` and read how it sorted the ideas by theme.

## 3. Give it their voice

The voice file is built from posts the person actually wrote, never from a description of how they'd like to sound.

```
Copy templates/voice.md to voice.md in this folder. Read the three
posts in it, written by the person this content is for. Study how they
write, how long their sentences run, how they open and close, how they
punctuate, the words they use and the ones they never use. Then write
the rules section of voice.md so another writer could follow it and
sound like them, and fill in the Words I never use section. Quote a
line from their posts as the example for each rule.
```

Read the rules aloud. If one doesn't sound like them, fix that line in `voice.md`. Every post they publish and like later goes back into this file, so it gets sharper every month.

## 4. Write the week, with sources

One idea per draft, each one built for where it's going. Then a review sheet for whoever signs off.

```
Using brief.md and voice.md, write a week of drafts into
drafts/week-of-[today's date].md:

- 3 LinkedIn posts, each on a different point from brief.md, about
  as long as the posts in voice.md, with the hook inside the first 140
  characters, because that's what shows before "see more" on a phone.
- 1 X thread of 6 to 8 posts, each under 280 characters, where post 1
  makes a claim that stands on its own.
- 1 newsletter section of about 200 words, opening in the first
  person, with one link out written as [your link] for me to fill in.

Follow voice.md exactly. Use only what's in brief.md. Mark any line
that doesn't come straight from brief.md, even a short linking line,
or where you simplified the argument, with [SIMPLIFIED] so I can check
it stayed true. Keep who or what every number was measured on. Carry
any [CONFIRM] item into a draft only with its tag still on it.

Then write review.md for whoever signs off. Put every [CONFIRM] and
[SIMPLIFIED] at the top. Then, for each draft, list every claim,
number and quote in it, with its timestamp and the exact words said
at that point in the transcript. Last, in ideas.md, mark each idea
you used with the draft it went into.
```

Read one LinkedIn draft next to one of the real posts in `voice.md`. Then send `review.md` with the drafts to whoever signs off. They read the flagged lines first and check any claim against what was said, so a yes takes minutes and doesn't turn into a rewrite.

## 5. Save it, and run the month

This step turns a good conversation into something you run on every new call, then runs it on a month of calls at once.

```
Turn steps 2 to 4 into a skill called transcript-to-week. Write it as
skills/transcript-to-week/SKILL.md, with a name and a one line
description at the top. It reads the call it's given, or else the
newest transcript in transcript/, by the date in its file name, or by
file date when the name has none. It writes everything for that call
into its own folder, runs/<transcript name>/, so no run overwrites
another. In that folder it writes brief.md with a timestamp on every
item, the week of drafts using voice.md with the same tags, and
review.md. It adds the call's ideas to ideas.md the way step 2 does,
moves any idea said on a second call to the top section, and marks
the ideas each draft used. It ends every run with three
lines: which transcript it read, how many new ideas went into
ideas.md, and how many [CONFIRM] and [SIMPLIFIED] tags need a look.
It never publishes anything.
```

A finished version ships as `skills/transcript-to-week/SKILL.example.md`, so compare yours with it. Then connect two things in Claude's settings, under connectors. Circleback reads your recorded meetings, and Parallel Search finds what's already published. In Circleback, give last month's calls one tag, so Claude reads those and nothing else. If your calls live somewhere else, put them in `month/` instead, one file per call with its date in the name. Change `[your tag]` to that tag's name, and run this.

```
Using the Circleback connector, find my meetings from last month
tagged [your tag], and only those. Take the four most recent. For each one,
oldest first, read its transcript and pull the ideas out the way step
2 does, into runs/<call name>/brief.md, with timestamps written as
[mm:ss] and every person written as their role, never their name. If
Circleback isn't connected, use the calls in month/ instead. Add the
ideas to ideas.md. Move every idea said on more than one call into
the "Said on more than one call" section at the top of ideas.md.
Then, using ideas.md and voice.md, write month-plan.md, a plan for
the next four weeks. For each week, one LinkedIn post, one newsletter
topic and one page topic AI could quote, each drawn from ideas.md
with the call and timestamp it came from. Plan only from ideas not
yet used, starting with any said on more than one call. Last, for
each page topic, use Parallel search to find the three pages that
answer that question best today. Under the topic, add their links and
one line on what they leave out that this idea covers. If one of
those pages gives a different number for the same study, mark that
idea [CONFIRM].
```

Read `month-plan.md` first, then open `ideas.md`. The ideas your founder said on more than one call sit in the section at the top, because those are the ones they believe most. Under each page topic in the plan sit the pages that already answer it and the gap your founder's idea fills, so you aren't writing the fortieth version of the same article. The month run writes a brief for each call and skips the drafts, so the plan has every idea to choose from. To run it in any Cowork session, add the skill to your Claude account where skills live in settings, by uploading the folder. Cowork loads the skills turned on for your account each time a session starts, and "run transcript-to-week" is then enough for each new call. If you can't find where skills live on your plan, ask Claude in Cowork.

### If you want it on a schedule

Ask Cowork to make a scheduled task that runs transcript-to-week every week, on the day your newest recording usually lands. This folder sits on your computer, so the task runs only while the computer is awake and the Claude app is open. Run it once on demand from the scheduled list first and read what it writes. If that run stops to ask permission, choose always allow for reading and writing files in this folder, because a weekly run that stops on a question waits for a click nobody gives.

## You now have

- `ideas.md`, the library of everything your founder says on calls, sorted by theme, each idea with the call and minute behind it
- `brief.md`, the ideas from one real call, each with the timestamp where it was said
- `voice.md`, the voice of the person the content is for, as rules with examples from their own posts
- A week of drafts in `drafts/`, each built for where it's going
- `review.md`, every claim with its source, for a sign-off that takes minutes
- The `transcript-to-week` skill, which does all of it again on the next call and adds it to the library
- `month-plan.md`, next month's posts, newsletter topics and page topics, drawn from the library, with each page topic checked against what's already published

Built by Catalyst, the preferred GTM content agency, led by Will Leatherman. gotcatalyst.com
