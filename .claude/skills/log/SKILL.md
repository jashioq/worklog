---
name: log
description: End-of-day work log. Turns my rough notes into daily/, open.md and glossary.md updates, then commits.
disable-model-invocation: true
---
Log my day. Notes: $ARGUMENTS (if empty, ask for them).

1. Read FORMAT.md, glossary.md, open.md. Get date/time with `date '+%F %a %H'` (before 05:00 → yesterday).
2. Map what I mention to existing links in glossary.md and open.md; always reuse an existing link over a new variant. Grep daily/ only for things you can't place otherwise. Ask only when you can't identify something or can't choose between candidates; batch all questions in one message.
3. Show one review, writing nothing yet (omit empty sections, mark guesses "(guess)"):
   - **Date**
   - **Today** — bullets for today's file
   - **Appendices** — per past day
   - **open.md** — added / changed / removed
   - **glossary.md** — added / changed (list new links)
4. Apply my feedback and show only what changed; repeat until I approve.
5. Write the files per FORMAT.md, then re-read each changed file against FORMAT.md and fix any deviation.
6. `git add -A && git commit -m "log: YYYY-MM-DD"` with a short body of what changed. Reply with the commit hash. Never push.
