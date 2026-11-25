# The Quiet Climb

Automate continuous improvement on work that's already in
progress.

The Quiet Climb turns an existing project into an
automatic, compounding improvement loop. A scheduled task
runs a six-step cycle — assess, study, improve, test,
record, repeat — scoring the work against a rubric out of
100 on every run, keeping only verified improvements, and
delivering the strongest verified version on time. It runs
quietly, under authority granted in advance, and surfaces
only at points named beforehand.

## Quick start

1. Point to the project — a folder, a repo, a workspace.
2. Add or confirm a rubric (quality criteria, scored out
   of 100).
3. Create the scheduled task from the YAML template in
   `SKILL.md`.
4. Enable the loop.
5. Set the delivery: when the best verified result
   surfaces.

## Worked example

A draft report starts complete at 87. Three recorded
iterations — clarify the key section (88), add evidence
(89), tighten the conclusion (91) — and it is delivered as
V1.3: verified, stronger, on time.

## What it outputs

The work itself, improved run over run, plus a short
record for every iteration: the change, the score before
and after, the result, the lesson, and the next best move.
The best verified versions collect in the project's
`output/` folder.

## Prerequisites

An agent runtime that supports SKILL.md-format skills and
scheduled tasks (cron or equivalent). The method itself is
runtime-agnostic.

## Known limitations

- The discipline assumes a human who grants standing
  authority in advance and means it; without that, every
  run becomes a permission request and the quiet is lost.
- Scores are only as honest as the rubric they are measured
  against; a vague rubric gives a vague score, and the
  record says so.

## License

MIT — see [LICENSE](LICENSE).
