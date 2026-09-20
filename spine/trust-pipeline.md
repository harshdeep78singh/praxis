# praxis: Trust Pipeline and Commit Gate

Research is the source of truth, so truth must stay clean. Nothing enters the
source of truth until confirmed.

## States (git for knowledge)

- inbox: unsure, zero-friction capture. Never treated as truth. Where AI's
  output and half-baked findings land safely.
- staging: candidate for truth, under review. This is the confirmation gate.
- committed (truth): confirmed source of truth, append-only after commit.

Files move inbox -> staging -> truth (or explorations, decisions) as they mature.
The move plus a git commit is the promotion. Logs are committed by nature
(append-only facts of what happened).

## Commit authority

The human is the sole commit authority. AI dumps, drafts, and stages freely, but
never writes to truth on its own and never overstates confidence.

## The commit gate (required)

Before anything enters the source of truth, the responsible skill (praxis-commit)
presents one consolidated list of all unresolved items for that topic:

- open questions
- unaddressed gaps
- untested assumptions
- pending decisions

Nothing commits until the human clears or accepts each item. This is the only
sanctioned place to resurface open questions (no nagging elsewhere). It enforces
"capture all value, no silent gaps" at the moment of commit.

## Provenance

On commit, record the origin trail (session, RFC, decision) so any piece of
truth is traceable to what produced it. This is the "what built what" guarantee.
