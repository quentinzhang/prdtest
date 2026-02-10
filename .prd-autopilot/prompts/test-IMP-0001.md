You are a coding agent working on ONE PRD card.

Required skill:
- You MUST use the prd-worker skill for this run.
- If you cannot access prd-worker, finish with outcome="blocked" and include a blocker: "prd-worker skill unavailable".

Card ID: IMP-0001
Project: test
Repo: /var/www/prdtest
Worktree: /var/www/prdtest/.worktrees/test/IMP-0001
Codex invoke: exec
Result schema: /private/var/www/prd/skills/prd-worker/assets/result.schema.json
Result JSON path: /var/www/prdtest/.worktrees/test/IMP-0001/.prd-autopilot/results/test-IMP-0001.json
Worker log path: /var/www/prdtest/.worktrees/test/IMP-0001/.prd-autopilot/results/test-IMP-0001.log
Date: 2026-02-09
Started at: 2026-02-09T12:52:47.316Z

Hard constraints:
- Do NOT edit the PRD hub at /private/var/www/prd. Treat it as read-only.
- Work ONLY inside the repo worktree at: /var/www/prdtest/.worktrees/test/IMP-0001
- You MUST finish by emitting a FINAL JSON response matching the required output schema.
  - outcome: "in-review" if you implemented + validated the change.
  - outcome: "blocked" if you cannot proceed (missing info, cannot run validation, unclear AC, etc.).

PRD card content:
---
---
id: "IMP-0001"
title: "把版权声明的2026改成2025～2026"
type: "improvement" # bug | feature | improvement
status: "pending" # # # source of truth (drafts | pending | in-progress | blocked | in-review | done | archived)
priority: "P2" # P0 | P1 | P2 | P3
severity: null # (bug only) S0 | S1 | S2 | S3
component: "ui"
owner: "codex"
reporter: ""
created_at: "2026-02-09"
updated_at: "2026-02-09"
due_at: null
spec: "self" # self | <path> | <url>
related_files: []
related_cards: []
labels: []
estimate: "" # XS | S | M | L
---

## Background / Problem Statement

## Impact

- User impact:
- Environment / browser / device:
- Components affected:

## Current Behavior

## Expected Behavior

## Reproduction Steps (Bug Only)

1.
2.
3.

## Solution / Design (Optional)

## Acceptance Criteria

- [ ] (Verifiable, testable, and avoids subjective wording)

## Test Plan

- Build/test commands:
- Manual validation:
- Regression areas:

## Risks & Rollback

- Risks:
- Rollback plan:

## Deliverables / Results (Fill When Done)

- Code changes:
- Validation evidence (command output / screenshot / recording / logs):
- Impact & compatibility notes:

## Clarifications / Open Questions

- Open questions / points needing clarification.

## Progress Log

### YYYY-MM-DD

- Status:
- Completed:
- Next:
- Blockers:
- Notes:

## Autopilot

### 2026-02-09

- Project: `test`
- Card: `IMP-0001`
- tmux: `prd-test-IMP-0001`
- Repo: `/var/www/prdtest`
- Worktree: `/var/www/prdtest/.worktrees/test/IMP-0001`
- Outcome: `blocked`
- Summary: Unable to locate a copyright statement containing "2026" in the provided worktree to update to "2025～2026".
- Blockers:
  - Worktree contains no copyright statement/year to update (no occurrences of "2026"; repository only tracks test.txt).

### Human update
- Added "2026" copywriting text
---

Now begin.

Reminder: Your FINAL message must be a single JSON object matching the schema.