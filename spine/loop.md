# praxis: The Loop

One workflow, incremental. Sessions vary in size; you return to a stream to
reuse and build on prior work.

## Rigor dial

Match rigor to uncertainty and size:

- Spike: fast, throwaway, one question. Output lands in inbox, never truth.
- Full exploration: defined search protocol, coverage tracking, provenance.

A spike is triage. It tells you whether a topic deserves full rigor. The timebox
also forces closure and respects limited time.

## Stages and what each produces

1. Frame. Intent, scope, goals and non-goals. Produces or updates an RFC.
2. Explore. Research at the dialed rigor; AI feedback loop; branches for
   parallel directions. Produces inbox dumps, literature notes, impact diffs
   against the current truth.
3. Synthesize. Distill to own-words atomic notes; update the truth view (MoC).
   Produces staged knowledge notes and an updated map.
4. Decide. Choices with tradeoffs; red-team the RFC at the review gate. Produces
   staged ADRs.
5. Prioritize. Rank action items by risk and value. Produces the action list.
6. Execute. Hand action items to OpenSpec (praxis-handoff calls opsx).
7. Close. Session log entry, git commit, provenance, next hook.

## Incremental and logged

Every session ends with a log entry (closure) and a next hook (momentum). The
log records what was explored, what action items were taken, and what got built,
so the "what built what" trail is never lost.

## Exploration rigor (scalable)

For a full exploration, define before diving: sources, search terms, and
inclusion and exclusion criteria (the value filter applied to sources). Track
coverage (identified, screened, kept) so nothing is missed unknowingly. Gaps
become open questions and action items. A small exploration gets a three-line
protocol; a big one gets full coverage tracking.
