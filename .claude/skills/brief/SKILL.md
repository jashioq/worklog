---
name: brief
description: Morning brief from open.md and glossary.md. Read-only.
disable-model-invocation: true
---
Brief me for today. Read-only: never edit files, commit or push.

Read open.md and glossary.md (for context on links). Get the date with `date '+%F %a'`, and each open.md line's last-change date with `git blame --date=short open.md`. Reply in one screen, omitting empty sections:

- **Overdue / due today**
- **Due in next 7 days** — with date
- **Waiting on others** — who to chase
- **Todo**
- **Discussions**
- **Stale** — open.md lines unchanged for 7+ days: still open?

One short line per item, keeping its links. Changes go through /log, not here.
