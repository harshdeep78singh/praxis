# praxis: TODO

Parked work, crisp. Each item passes the value filter before it is built.

## Define the state-of-the-art "trend-scout" agent

Goal: keep streams current on state-of-the-art tools and techniques.

To define before building:
- Survey existing tools first (Superpowers, github.com/mattpocock/skills, others).
  Decide what to reuse vs. build.
- Mechanism: a standing, re-runnable protocol (living review) over the top people
  and feeds named in each stream's `sources`.
- Output: candidates plus alternatives into `inbox/` and this backlog, never
  straight to truth. Passes the value filter.
- Invocation: on-demand first; consider scheduled later.
- Open: agent vs. skill; how sources are stored per stream; dedup against truth.

Status: to design.

## Framework follow-ups

- Custom OpenSpec schema for the praxis loop (fork spec-driven). Currently on
  spec-driven default.
- `streams/_template/`: a ready stream scaffold for `praxis-new-stream`.
- Generic tools in `tools/` (for example a scope-filter), built as needed.

## First stream: bug-bounty

- Scaffold the `bug-bounty` stream.
- Migrate the existing Fivetran work (`fivetran-pro-testing-playbook`) into it.
- Data-driven re-optimization: rank vuln classes by last-6-months payouts;
  extract recent top reporters' tooling; propose alternatives to backlog; rewrite
  tasks around highest ROI and the "AI explains past vulns, human hunts live"
  split.

## Parked decision: prior-art scan (2026-09-20)

Decision: keep praxis as a thin integrating clarity layer. Do not rebuild the
commodity layers; reuse existing conventions. Revisit this before extending the
notes, decisions, or charter mechanics.

Landscape found:
- Spec-driven build: GitHub Spec Kit (its "constitution" is an always-on rules
  file, like our charter), Kiro, BMAD-METHOD (multi-domain), Agent OS, OpenSpec
  (our substrate). All are build/code-gen-first.
- Agentic skills: obra/superpowers (mandatory skill-check, opt-in via
  workflow.json, cross-tool), mattpocock/skills. Dev-focused.
- PKM/notes: Obsidian, Logseq, joshylchen/zettelkasten (AI, atomic, CEQRC
  workflow). This is our knowledge layer, already solved.
- Decisions: me2resh/agent-decision-record (AgDR, ADR for AI agents),
  zircote/git-adr (ADRs in git notes), MADR.
- Provenance: "Lore" (git commit messages as a knowledge protocol for agents).

Defensible core (keep sharp): integration across the full arc (curiosity to
clarity to action to knowledge); clarity/research-first and generic across
streams; the trust/commit gate (human as sole commit authority); the
psychology-grounded anti-slop charter. No direct equivalent found for the last
two.

Actions when unparked:
- Reuse Zettelkasten + CODE conventions for notes; do not author from scratch.
- Reuse AgDR / MADR / git-adr conventions for decisions.
- Study Spec Kit's "constitution" and obra/superpowers before extending the
  charter or skills; borrow their mechanics (opt-in switch, mandatory
  skill-check).
- Be able to answer: "why not just wire Spec Kit + Obsidian + superpowers?"

References:
- https://medium.com/@tim_wang/spec-kit-bmad-and-agent-os-e8536f6bf8a4
- https://reenbit.com/bmad-vs-spec-kit-vs-openspec-choosing-your-spec-driven-ai-framework/
- https://github.com/github/spec-kit
- https://github.com/obra/superpowers
- https://github.com/joshylchen/zettelkasten
- https://github.com/me2resh/agent-decision-record
- https://github.com/zircote/git-adr
- https://arxiv.org/pdf/2603.15566  (Lore)
