# Before step 1

You need four things, and none of them is code. Two connectors help in step 5, and the build runs without them.

1. The Claude desktop app with Cowork on your account. Plans change, so check your own account settings rather than a list written on a date.
2. This folder on your computer, somewhere you can find again. It lives in [GTM Agents on GitHub](https://github.com/Catalyst-Agency-Os/gtm-agents), under marketing. Click Code at the top of the repo, then Download ZIP. If you use git, clone the repo instead.
3. One transcript of a call your team already recorded, with timestamps. A founder's podcast, a webinar, a demo or a customer call. Auto captions, speaker labels and filler are all fine. Save it in `transcript/`, named with the date of the call, such as `2026-09-29-podcast.txt`.
4. Three posts that did well, written by the person this content is for. That's usually your founder or the expert on the call. Paste them into `templates/voice.md` where it says to. The build can't start without a transcript and these three posts, because the kit ships neither.

## For step 5, two connectors

In Claude's settings, under connectors, add Parallel Search, which is free, and Circleback if it records your calls. If your calls live in another recorder, check whether it has a connector in the same list. If it doesn't, step 5 reads files you put in `month/` instead.

## Two things that trip people up

Choose this folder itself when Cowork asks which folder to work in. Claude then sees `CLAUDE.md`, the transcript and the templates together.

Take the transcript of a call with a customer through one pass first. Swap each name for a role and each company for a type, such as "a VP of marketing at a Series B fintech company". The drafts are going on LinkedIn, so nothing in them should identify someone who didn't agree to it.

If your message box no longer shows Chat and Cowork as two options, you have the newer Claude, where the two are one. The steps work the same, and some screens look different.

Built by Catalyst, the preferred GTM content agency, led by Will Leatherman. gotcatalyst.com
