---
name: praxis-commit
description: The commit gate. Use automatically whenever anything is about to enter the source of truth (promotion from staging to truth, explorations, or decisions), and when the user runs /praxis-commit. Always run this before writing to truth.
allowed-tools: Bash, Read, Write, Grep, Glob
---

Enforce the commit gate. The human is the sole commit authority. Read
`../../spine/trust-pipeline.md` first.

Steps:
1. Gather every unresolved item for the topic and present ONE consolidated list:
   - open questions
   - unaddressed gaps
   - untested assumptions
   - pending decisions
2. Wait for the human to clear or accept each item. Do not proceed until done.
   This is the only sanctioned place to resurface open questions.
3. On clearance, move the files from `staging/` to their home (`truth/`,
   `explorations/`, or `decisions/`).
4. Record provenance (session, RFC, decision) so the truth is traceable.
5. `git add` and `git commit` with a message stating what and why.

Never commit to truth on your own judgement.
