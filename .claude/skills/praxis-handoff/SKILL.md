---
name: praxis-handoff
description: Convert an RFC's prioritized action items into OpenSpec changes and tasks for execution. Use when the user runs /praxis-handoff or is ready to execute action items from an accepted exploration.
allowed-tools: Bash, Read, Write, Grep, Glob
---

Hand accepted action items to OpenSpec. praxis produces; OpenSpec executes.

Steps:
1. Read the accepted RFC and its action items.
2. Create an OpenSpec change (this repo is the shared store):
   `openspec new change "<stream>-<slug>"`. Name it by stream.
3. Drive the opsx propose workflow to turn the action items into tasks. Ground
   the tasks in the RFC; do not invent scope.
4. Link the change back to the RFC (record the change name on the RFC).
5. Stop at planning. Execution (apply) is a separate, explicit step.
