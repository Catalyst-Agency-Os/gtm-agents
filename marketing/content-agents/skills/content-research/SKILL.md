---
name: content-research
description: Reads any call in transcript/ that isn't in ideas.md yet into the idea library, then finds what the buyers in market.md are struggling with in the last 14 days and rewrites topics.md, keeping only topics the calls already answer. Research only.
---

# Content research

Run this when someone says "run content-research", or from the weekly scheduled task before content-writer.

## 1. Read new calls into the library

1. List the files in `transcript/`, skipping any README. A call is new when its file name appears nowhere in `ideas.md`.
2. Read each new call in full, oldest first. Add its main argument as one entry.
3. Add every idea worth publishing, in the speaker's own words wherever possible. That means each belief, each story, each number and each line quotable as said, filed under its theme with the call's file name and the timestamp, like [12:40].
4. A timestamp marks the start of a speaker's turn. Cite the turn the words sit in, and both turns when a quote runs across two.
5. An idea already in the library gets this call as another source, and moves to "Said on more than one call" at the top.
6. Read the last ten minutes of each call again, where the speaker sums up, and add every action and number from it.
7. Swap the name of any customer, prospect, competitor, agency, vendor, company used as an example, or person other than the speaker for their role or type of company. Keep the names of the platforms a call is about, such as Google, LinkedIn or Claude. Keep a research firm's or university's name only as the source of a number, and call a vendor's or agency's study just that.
8. Mark anything unclear [CONFIRM] instead of guessing.

If someone names a recorder connector and a tag, read last week's calls with that tag from it, and only those.

## 2. Research what buyers are talking about

Read `market.md`. Search the web for what the buyers it names are struggling with and talking about in the last 14 days, in the places it names and anywhere else they post, read or argue. Read at least 15 pieces. Leave out the topics `market.md` says to stay away from.

## 3. Rewrite topics.md

Put the date range at the top, then four sections.

1. **Pain points.** The 8 to 10 problems these buyers raise most, grouped into themes, each with how many pieces raised it. Each one quotes, with the link, someone who holds the job `market.md` names. If nobody in that job raised it in the last 14 days, quote the closest job found and say how they differ. Pieces by vendors, agencies or news sites count toward how often a pain comes up, and never supply its quote.
2. **Formats.** The post formats the pieces use most, each with how many pieces used it and one linked example. Where the page shows reactions, comments or shares, write the count it shows.
3. **This week's topics.** For each pain point, the idea in `ideas.md` that answers it directly, and one line on why it was kept or dropped. Skip any idea marked used in the last four weeks. A pain the library names without an answer goes under "Asked and not yet answered", for the next call. Rank what's kept by how many pieces raised the pain, and break ties with ideas said on more than one call. The top 5 cover at least three themes. For each of the top 5, write the pain point, the idea with its call and timestamp, the format that suits it, and one line on why now that names a dated piece from section 4.
4. **What I read.** Every piece, with its title, date, link and format, and which pain each piece raised, so every count can be checked.

## 4. Report

End with three lines.

- How many new calls you read
- How many topics made the list
- The top topic

## Never

- Never publish, post, schedule or send anything.
- Never invent a link, a quote or a count. If you can't search the web, say so and stop.
- Never take an answer from the web. The web picks the question, and the calls supply the answer.
