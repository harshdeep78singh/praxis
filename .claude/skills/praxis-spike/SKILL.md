---
name: praxis-spike
description: Run a timeboxed throwaway probe to answer one narrow question and reduce uncertainty. Use when the user runs /praxis-spike or asks for a quick check, spike, or "can this even work" probe.
allowed-tools: Bash, Write, Read, Grep, Glob, WebSearch, WebFetch
---

A spike is fast, low-rigor, and throwaway. Its deliverable is the learning, not
the output.

Steps:
1. State the one question and the timebox (for example 30 minutes).
2. Probe directly. Skip polish, tests, and coverage.
3. Write the finding (answer plus any evidence) to `inbox/` as a short note.
4. If it de-risks a decision, link it into the relevant RFC.
5. Stop at the timebox regardless of state. Report what was learned.

Never promote spike output to truth directly; it stays in inbox until it earns
promotion through the normal gate.
