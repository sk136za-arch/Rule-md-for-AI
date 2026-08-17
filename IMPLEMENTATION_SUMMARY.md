# Implementation Summary

## Task

Update `AGENTS.md` orchestration rules for Git-scoped summaries, independent test-case design and test execution, and role-based model routing.

## Result

The guidance now summarizes only the current uncommitted task, separates Test-Case Designer from Tester, and routes reasoning work to sol and implementation/testing actions to luna.

## Changes Made

* `AGENTS.md`: Added Git-status/history checks and uncommitted-only rules for `IMPLEMENTATION_SUMMARY.md`.
* `AGENTS.md`: Added the Test-Case Designer role, workflow step, independence requirements, and Definition of Done checks.
* `AGENTS.md`: Added model routing for sol and luna across the main and corrective workflows.

## Validation Performed

| Check | Command | Result |
| --- | --- | --- |
| Diff validation | `git diff --check` | Passed |
| Policy coverage | `rg -n -i "gpt-5\\.6-(sol|luna)|Test-Case Designer|uncommitted|committed|git status" AGENTS.md` | Passed |

## Remaining Concerns

* None for this documentation-only change.

## Files Changed

* `AGENTS.md`
* `IMPLEMENTATION_SUMMARY.md`

## Final Status

Completed
