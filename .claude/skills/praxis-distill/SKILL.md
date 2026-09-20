---
name: praxis-distill
description: Turn raw log or inbox material into atomic, own-words knowledge notes staged for review. Use when the user runs /praxis-distill or asks to distill, write up, or turn findings into notes.
allowed-tools: Read, Write, Grep, Glob
---

Convert raw material into atomic knowledge notes. Read `../../spine/artifacts.md`
first.

Steps:
1. Read the source (an inbox dump or a log entry).
2. For each distinct idea, write one atomic note from
   `spine/templates/note.md` into `staging/`:
   - one idea per note, stated as a claim
   - in the human's own words, not quotes (the understanding gate)
   - a one-line summary and tags in frontmatter
   - link related notes with [[note-id]]
   - use a timestamp id (YYYYMMDDHHMM)
3. Tag any captured failure #dead-end.
4. Leave notes in staging. Promotion to truth is via praxis-commit.
