# praxis: Artifacts

Four artifact types per stream, all Markdown plus YAML frontmatter, git-diffable
and Obsidian-friendly. Templates live in `spine/templates/`.

## The spine (do, understand, decide, plus clarity)

- Exploration (RFC): how I got clear and what to do. Central, upstream of
  OpenSpec.
- Log: what I did. Raw, chronological, append-only.
- Knowledge: what I understand. Atomic, linked, distilled.
- Decision (ADR): what I chose and why. Immutable, tradeoffs explicit.

Action items flow out of the RFC to OpenSpec for execution.

## Storage and naming

- RFC: `streams/<s>/explorations/RFC-NNNN-slug.md`
  frontmatter: id, title, stream, status (draft, review, accepted, superseded),
  created, updated, rigor (spike, full), intended_value, success_criterion,
  links, open_questions.
  body: Context, Goals and Non-Goals, Alternatives, Risks (systematic), Action
  items, Review.

- Log: `streams/<s>/log/YYYY-MM-DD-NN-slug.md` (append-only, one per session)
  frontmatter: date, stream, session_id, rigor, refs (rfc, branch, commit).
  body: Objective, Explored, Findings, Action items, Realized value, Next hook,
  commit.

- Knowledge note: `streams/<s>/truth/notes/<zid>-slug.md` (atomic; zid is
  YYYYMMDDHHMM)
  frontmatter: id, title, tags, source, created, links, review_by (optional).
  body: the idea in own words, plus [[wikilinks]].
  MoC and entry point: `streams/<s>/truth/INDEX.md` and
  `streams/<s>/truth/maps/<topic>.md`.

- Decision (ADR): `streams/<s>/decisions/ADR-NNNN-slug.md`
  frontmatter: number, title, status (proposed, accepted, superseded), date,
  supersedes, superseded_by, value_rationale.
  body: Context, Decision, Consequences (positive and negative).

## Special note conventions

- Dead-ends are first-class: capture "tried X, failed, why" as a note tagged
  #dead-end so it is never re-researched.
- Truth freshness: a note may carry review_by; stale truth is flagged for
  re-validation.

## Links and retrieval

- Use [[wikilinks]] between notes: navigable graph for humans, navigation edges
  for the agent.
- Retrieval is on-demand (grep, glob). Read `truth/INDEX.md` first, then follow
  links to only the needed notes. Frontmatter carries a one-line summary and
  tags for cheap triage before opening bodies.

## Trust states

Every artifact is inbox, staging, or committed. See `spine/trust-pipeline.md`.
