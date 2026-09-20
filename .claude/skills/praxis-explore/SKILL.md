---
name: praxis-explore
description: Run the praxis core loop (frame, explore, synthesize) for one question in a stream, producing an RFC, inbox dumps, and staged notes. Use when the user runs /praxis-explore or asks to explore, research, or get clear on something.
allowed-tools: Bash, Write, Read, Grep, Glob, WebSearch, WebFetch
---

Run stages 1 to 3 of the loop. Read `../../CLAUDE.md`, `../../spine/loop.md`,
and the stream's `truth/INDEX.md` first.

Steps:
1. Frame. Clarify intent and scope with sharp questions (one at a time). Set the
   rigor dial (spike or full). Create an RFC from `spine/templates/rfc.md` in
   `explorations/`, filling Goals/Non-Goals, intended_value, success_criterion.
2. Protocol. For full rigor, define sources, terms, and inclusion/exclusion
   criteria before searching. Scale to session size.
3. Explore. Research at the dialed rigor. Dump raw findings to `inbox/`. Use
   branches for parallel directions if needed. Note impact on current truth.
4. Synthesize. Draft own-words atomic notes into `staging/` (or call
   praxis-distill). Record open questions and gaps on the RFC.
5. Produce prioritized action items on the RFC. Stop. Nothing enters truth here;
   promotion is via praxis-commit.

Honor the charter: data-based, no conclusions forced, small waves when
explaining.
