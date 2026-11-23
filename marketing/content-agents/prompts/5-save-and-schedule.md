# Step 5, save both agents and run them every week

This turns steps 1 to 4 into two skills. Then ask Cowork for a weekly scheduled task that runs content-research and then content-writer, and run it once by hand first.

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

Built by Catalyst, the preferred GTM content agency, led by Will Leatherman. gotcatalyst.com
