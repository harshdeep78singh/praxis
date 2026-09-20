# praxis

A personal, clarity-first research and build framework on top of OpenSpec.

praxis owns the phase OpenSpec skips: turning curiosity and AI's motion into
clarity, an impact map, and prioritized, reviewed action items, with no silent
gaps. OpenSpec then executes. It is generic; each domain is a stream.

## Layout

- `CLAUDE.md`, `AGENTS.md`: operating manual and charter (always loaded).
- `spine/`: the framework (philosophy, loop, artifacts, trust pipeline, value
  filter, charter) and `spine/templates/`.
- `streams/<name>/`: one domain each (inbox, staging, truth, log, explorations,
  decisions, methods, tools).
- `.claude/skills/`: the `praxis-*` skills and OpenSpec `opsx` skills.
- `openspec/`: execution layer.
- `tools/`: generic scripts (Python, PEP-723, run via `uv run`).

## The loop

Explore, derive action items, execute, return and build, repeat. Rigor dial:
spike (fast, throwaway) to full exploration (protocol, coverage). Every session
ends with a log entry and a next hook.

## Artifacts

Exploration (RFC), Log, Knowledge notes, Decisions (ADR). All Markdown plus
frontmatter. Notes are atomic and linked with `[[wikilinks]]`.

## Skills

`praxis-new-stream`, `praxis-explore`, `praxis-spike`, `praxis-distill`,
`praxis-commit` (the commit gate), `praxis-decide`, `praxis-handoff`,
`praxis-close`.

## Use on a new machine

1. Clone this repo.
2. Register it as an OpenSpec store: `openspec store register . --id praxis`.
3. Open it in Claude Code. `CLAUDE.md` and the skills load automatically.

Requires the `openspec` CLI and `uv` (for tools).
