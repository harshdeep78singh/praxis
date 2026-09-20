---
name: praxis-decide
description: Author an architecture/decision record (ADR) capturing a choice, its context, and consequences. Use when the user runs /praxis-decide or a significant decision needs recording.
allowed-tools: Read, Write, Grep, Glob
---

Record one decision as an ADR. Read `../../spine/artifacts.md` first.

Steps:
1. Create an ADR from `spine/templates/adr.md` in `staging/` (promotion via
   praxis-commit).
2. Fill Context (forces at play), Decision (what was chosen), and Consequences
   (positive and negative, tradeoffs explicit).
3. Set value_rationale (which value-filter axis it passed and why).
4. One decision per record. Number it (zero-padded, next in the stream).
5. To change a prior decision, do not edit it. Write a new ADR and set
   supersedes and superseded_by.
