# Founder idea library, in Claude Cowork

Turn every call your team records into a library of what your founder says, then into a month of content in their voice. Every claim traces to a timestamp in the call, so sign-off takes minutes. You build it in Claude Cowork with no code, then save it as a skill you run on every new call.

> Your build-along project for the Maven session "Automate Your Content Creation in Claude Cowork, No Code", Tue 2026-11-24.

## The idea underneath it

Your company's best thinking is already recorded, on podcasts, demos, webinars and customer calls. Those calls hold the specifics, the numbers, the stories and the line said off the cuff that beats anything typed cold. So Claude's job is to pull those out and reshape them, with the source of every line. It never makes them up.

## What you leave with

- `ideas.md`, a library of everything your founder says on calls, sorted by theme, each idea with the call and minute behind it
- `brief.md`, the claims, quotes and story pulled out of one real call, each with its timestamp
- `voice.md`, written from posts the person actually wrote, so the drafts sound like them
- A week of drafts, three LinkedIn posts, an X thread and a newsletter section
- `review.md`, every claim with its source, for a sign-off that takes minutes
- The `transcript-to-week` skill, which runs all of it again on the next call and grows the library
- `month-plan.md`, a month of content planned from a month of calls

## Start here

1. Read [PREREQUISITES.md](PREREQUISITES.md) and stage the two inputs.
2. Open this folder in Cowork.
3. Work through [BUILD_STEPS.md](BUILD_STEPS.md) top to bottom. Every prompt is in it, ready to paste.

## What's in the folder

| Path | What it is |
|---|---|
| `PREREQUISITES.md` | What to have open and staged before step 1 |
| `BUILD_STEPS.md` | The five steps, with every prompt to paste |
| `CLAUDE.md` | The rules Cowork reads first in this folder |
| `prompts/` | The four prompts on their own, to rerun any step |
| `templates/brief.md` | The shape step 2 fills in |
| `templates/ideas.md` | The shape of the idea library. Step 2 copies it to `ideas.md` |
| `templates/voice.md` | Where the three posts go. Step 3 copies it to `voice.md` and writes the rules there |
| `transcript/` | Where your transcript goes |
| `skills/transcript-to-week/SKILL.example.md` | A finished version of the skill, to compare with yours |

Built by Catalyst, the preferred GTM content agency, led by Will Leatherman. gotcatalyst.com
