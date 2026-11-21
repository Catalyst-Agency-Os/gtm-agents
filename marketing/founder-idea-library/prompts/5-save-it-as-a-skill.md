# Step 5, save it, and run the month

Run this once steps 2 to 4 have produced a week you're happy with.

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

Then connect two things in Claude's settings, under connectors. Riverside reads your recordings, and Parallel Search finds what's already published. Parallel is free. Riverside needs one of its paid plans, so if your calls live somewhere else, put last month's calls in `month/` instead, one file per call with its date in the name. Change `[your studio]` to the Riverside studio your calls are saved in, and run this.

```
Using the Riverside connector, find the studio [your studio] and
list only its projects. Take the four most recent recordings from last month. For each one,
oldest first, read its transcript and pull the ideas out the way step
2 does, into runs/<call name>/brief.md, with timestamps written as
[mm:ss] and every person written as their role, never their name. If
Riverside isn't connected, use the calls in month/ instead. Add the
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

Once the skill is added to your Claude account, "run transcript-to-week" is enough.

Built by Catalyst, the preferred GTM content agency, led by Will Leatherman. gotcatalyst.com
