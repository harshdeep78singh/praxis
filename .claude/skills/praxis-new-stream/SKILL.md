---
name: praxis-new-stream
description: Scaffold a new praxis stream (a domain) with its charter and folder structure. Use when the user runs /praxis-new-stream or asks to start a new stream, domain, or area in praxis.
allowed-tools: Bash, Write, Read
---

Scaffold a new stream under `streams/<name>/`.

Read `../../CLAUDE.md` and `../../spine/artifacts.md` first.

Steps:
1. Get the stream name (kebab-case).
2. Author `stream.md` (the charter). Ask for the seven definitions one at a time
   (Charter principle 14), in this order: intent; scope and non-goals;
   current-truth baseline; success/impact criteria; methods; sources; default
   rigor. Build on each answer before the next.
3. Create folders: `inbox/ staging/ truth/notes/ truth/maps/ log/
   explorations/ decisions/ methods/ tools/`.
4. Copy `spine/templates/index.md` to `streams/<name>/truth/INDEX.md` and fill
   the stream field.
5. Confirm the layout with `ls`, then stop. Do not start exploring.
