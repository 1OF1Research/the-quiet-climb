---
name: the-quiet-climb
description: Turn work already in progress into an automatic, compounding improvement loop — a scheduled six-step cycle (assess, study, improve, test, record, repeat) scored against a rubric, run quietly, and delivered at its strongest verified version on time. Trigger: 'quiet climb', 'climb it silently', 'set up a climb', any standing improvement lane.
---

# The Quiet Climb

Automate continuous improvement on work that's already in
progress.

## Purpose

Turn an existing project into an automatic, compounding
improvement loop: study, improve, verify, record — and
climb daily.

## When to use

- A project is already started.
- You want steady, measurable improvement.
- You want it to run on a schedule without manual prompts.
- You want a stronger, verified result over time.

## Key principles

- **Iterate** — improve what works.
- **Verify** — measure the gain.
- **Preserve** — keep proven wins.
- **Compound** — build a stronger result each run.
- **Quiet** — run without noise.
- **Surface** — deliver on the deadline or milestone.

## The cycle

Every run takes the same six steps:

1. **Assess** — read the current work, its status, and its
   results.
2. **Study** — learn from new data, research, and
   comparisons.
3. **Improve** — derive and apply a small, verifiable
   change.
4. **Test** — run checks, benchmarks, or the rubric.
5. **Record** — log the change, the results, and the
   lesson.
6. **Repeat** — run again on the schedule, and keep
   climbing.

## Setup (one time)

1. Point to the project — a folder, a repo, a workspace.
2. Add or confirm a rubric: the quality criteria the work
   is scored against, out of 100.
3. Create the scheduled task, using the template below.
4. Enable the loop: assess, study, improve, test, record,
   repeat.
5. Set the delivery: when, and how, the best verified
   result surfaces.

## Task template (YAML)

    name: Quiet Climb — Project X
    schedule:
      cron: "32 * * * *"        # hourly at :32
    task:
      type: quiet-climb
      target: "/projects/project-x/"
      rubric: "/projects/project-x/RUBRIC.md"
      steps:
        - assess
        - study
        - improve
        - test
        - record
      mode: silent              # minimal notifications
      surface: on_time          # deliver for milestone

## Schedule examples

- Hourly — active development, fast iteration.
- Daily — study, improve, and record once a day.
- Daily (deep) — larger tests, evaluations, or balances.
- Weekly — a major refactor or a new variant.
- Pre-deadline, every 6 hours — an intensive climb before
  a submission.

## Run output (each iteration)

    status: in_progress
    iteration: 12
    change: stronger evidence section
    score: 87 -> 91 (+4)
    result: keep
    lesson: data source improved clarity
    next: test alternate format

## Success rules

- The work stays complete and usable at every step.
- Only verified improvements are kept.
- Every change and result is recorded.
- Quality compounds over time; it never resets.
- The loop runs quietly and keeps its schedule.
- The strongest verified version is delivered on time.

## Metrics to track (optional, recommended)

- Rubric score (e.g. 87 -> 91).
- Task success (pass / fail).
- Quality deltas (e.g. +4).
- Runtime and compute cost.
- Token usage, where applicable.
- Cumulative improvement (e.g. +12).

## Project layout (recommended)

    project-x/
      WORK.md        # current work, in progress
      RUBRIC.md      # quality criteria and scoring
      CLIMB.md       # plan, daily log, and lessons
      runs/
        2026-11-24/  # iteration results
        2026-11-25/
      lessons.md     # cumulative learnings
      output/        # best verified versions

## Worked example

A work-in-progress report, climbed:

- Baseline — draft complete, score 87.
- Iteration 1 — clarify the key section, score 88.
- Iteration 2 — add evidence, score 89.
- Iteration 3 — tighten the conclusion, score 91.
- Deliver — V1.3: verified, stronger, on time.

## Guardrails

- A climb runs under authority granted in advance; anything
  outside it (a spend, public words, an irreversible step)
  waits at the surface point, named plainly, instead of
  happening quietly.
- Surface points are named before the climb starts: a
  verified win, money at stake, a genuine deadline risk, a
  step only the owner can do, or the finished work.
- If a score cannot honestly rise, record the plateau and
  change the approach — never invent progress.
- Every test outcome is saved, failures and successes both,
  with the exact condition where the work is tender.
- Claims travel labelled — VERIFIED / DERIVED / UNKNOWN —
  and a researched claim stays a lead until it is measured
  firsthand.

## Proof standard

The strength is present when a stranger reading the climb's
records can see the score rise run over run on named proof,
nothing surfaced before its named point, and the delivered
package needed no repair after handoff.

## Falsifier

If climbs repeatedly surface noise, stall without a
recorded plateau, or hand off packages that need fixing
afterward — measured on real climbs, not preference — the
cadence or the record rules above are wrong and are
re-derived, not quietly abandoned.
