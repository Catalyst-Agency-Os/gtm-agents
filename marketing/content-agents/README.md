# Two content agents, in Claude Cowork

A research agent finds what your buyers are struggling with this week. A writer agent turns it into drafts for every channel, in your founder's voice. Both work from one library of everything your founder has said on calls, so every claim traces to the minute it was said and sign-off takes minutes. You build it in Claude Cowork with no code, then put both agents on a weekly schedule.

> Your build-along project for the Maven session "Automate Your Content Creation in Claude Cowork, No Code", Tue 2026-11-24.

## The idea underneath it

AI content sounds like everyone else's when it's asked to invent. Your company's best thinking is already recorded, on podcasts, demos, webinars and customer calls. So the research agent picks what to write about, from what buyers are saying this week, and the answer always comes from what your founder already said on a call. A topic your founder has no answer to gets dropped.

## What you leave with

- `ideas.md`, a library of everything your founder says on calls, sorted by theme, each idea with the call and minute behind it
- `topics.md`, what your buyers are struggling with this week, matched to what your founder already said about it
- `voice.md`, written from posts the person actually wrote, so the drafts sound like them
- Drafts for every channel, LinkedIn, X and a newsletter section, each in its own folder
- `review.md`, every claim with its source, for a sign-off that takes minutes
- The `content-research` and `content-writer` skills, on a weekly schedule

## Start here

1. Read [PREREQUISITES.md](PREREQUISITES.md) and stage the inputs.
2. Open this folder in Cowork.
3. Work through [BUILD_STEPS.md](BUILD_STEPS.md) top to bottom. Every prompt is in it, ready to paste.

## What's in the folder

| Path | What it is |
|---|---|
| `PREREQUISITES.md` | What to have open and staged before step 1 |
| `BUILD_STEPS.md` | The five steps, with every prompt to paste |
| `CLAUDE.md` | The rules Cowork reads first in this folder |
| `prompts/` | The five prompts on their own, to rerun any step |
| `templates/ideas.md` | The shape of the idea library. Step 1 copies it to `ideas.md` |
| `templates/market.md` | Who your buyers are and where they talk. The research agent reads it first |
| `templates/voice.md` | Where the three posts go. Step 3 copies it to `voice.md` and writes the rules there |
| `transcript/` | Where your call transcripts go |
| `examples/` | Finished versions of both skills, to compare with yours |

Built by Catalyst, the preferred GTM content agency, led by Will Leatherman. gotcatalyst.com
