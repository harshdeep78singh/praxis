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
