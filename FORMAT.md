# Worklog format

## Links
`[[anything]]` links a note to a person, project, ticket, PR, date, and so on. Lowercase kebab-case; reuse existing links, never invent variants.
Examples: `[[tanaka]]` `[[project-games]]` `[[ticket-432141]]` `[[pr-new-interfaces]]` `[[2026-10-20]]`

## glossary.md
One line per link: the link, then a description that may contain more links. Edit in place; git keeps history.
```
[[project-games]] Project adding games to the app. Requested by [[tanaka]].
[[tanaka]] PM on [[project-games]] and [[project-ads]].
```

## open.md
Only open things, as free-form bullets under these headings. Remove a bullet when it's done. A deadline lives only under Deadlines.
```
## Discussions
- Waiting on [[tanaka]]'s feedback on [[ticket-432141]] ([[project-games]]), needed to merge [[pr-new-interfaces]].
## Todo
- Align with [[taro]] on [[ticket-2381823]] analytics spec.
## Deadlines
- Merge [[pr-new-interfaces]] by [[2026-10-20]].
```

## daily/YYYY/YYYY-MM-DD.md
Free-form bullets: what I did and the outcome, with links.
```
# 2026-10-12 (Mon)
- Implemented consent screen for [[project-ads]], opened [[pr-consent-screen]].
- [[pr-new-interfaces]] merged. Closed.
- Deadline for [[pr-new-interfaces]] moved [[2026-10-20]] → [[2026-10-27]]: [[tanaka]] on leave.
- Feedback from [[taro]]: design doc clear but too long.
```
Every addition to or removal from open.md gets a bullet here; this is the only place history survives.

## Corrections
Today's file may be edited freely. Past days: never change existing lines; append to that day's file:
```
## Appendix 1 — 2026-10-15
- Correction: "opened [[pr-consent-screen]]" — it was [[pr-consent-v2]].
- Addition: crash reports on checkout halved since this change.
```
Latest appendix wins. Missed a whole day: create that day's file.

## Git
Local only. Commit, never push.
