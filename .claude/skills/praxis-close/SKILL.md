---
name: praxis-close
description: Close a praxis session with a log entry, provenance, a next hook, and a commit. Use when the user runs /praxis-close or ends a working session.
allowed-tools: Bash, Read, Write
---

End the session with closure and momentum. Read `../../spine/loop.md` first.

Steps:
1. Create a log entry from `spine/templates/log-entry.md` in the stream's
   `log/` as `YYYY-MM-DD-NN-slug.md` (append-only).
2. Fill Objective, Explored, Findings, Action items, Realized value (which
   value-filter axis; worth repeating?), and a Next hook (the continuation
   point).
3. Link refs (RFC, branch, relevant commits).
4. `git add` and `git commit`. Record the commit hash in the log entry.
5. Report the next hook so the next session starts with momentum.
