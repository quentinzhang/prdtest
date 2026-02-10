You are a coding agent working on ONE PRD card.

Required skill:
- You MUST use the prd-worker skill for this run.
- If you cannot access prd-worker, finish with outcome="blocked" and include a blocker: "prd-worker skill unavailable".

Card ID: BUG-0002
Project: test
Repo: /var/www/prdtest
Worktree: /var/www/prdtest/.worktrees/test/BUG-0002
Codex invoke: prompt
Result schema: /private/var/www/prd/skills/prd-worker/assets/result.schema.json
Result JSON path: /var/www/prdtest/.worktrees/test/BUG-0002/.prd-autopilot/results/test-BUG-0002.json
Worker log path: /var/www/prdtest/.worktrees/test/BUG-0002/.prd-autopilot/results/test-BUG-0002.log
Date: 2026-02-10
Started at: 2026-02-10T07:43:14.675Z

Hard constraints:
- Do NOT edit the PRD hub at /private/var/www/prd. Treat it as read-only.
- Work ONLY inside the repo worktree at: /var/www/prdtest/.worktrees/test/BUG-0002
- Immediately before the FINAL JSON, output a short natural-language summary message (not JSON).
- You MUST finish by emitting a FINAL JSON response matching the required output schema.
- Your FINAL message must be ONLY the JSON object (no prose before/after).
- Include the same human-readable summary inside the FINAL JSON "notes" field so it is captured in logs/artifacts.
  - outcome: "in-review" if you implemented + validated the change.
  - outcome: "blocked" if you cannot proceed (missing info, cannot run validation, unclear AC, etc.).

IMPORTANT (prompt/TUI mode): Codex cannot auto-save your last message.
- You MUST ALSO write the same FINAL JSON object to the file path in "Result JSON path".
- Write ONLY the JSON object to that file (do not include the human-readable summary).
- You may use PRD_AUTOPILOT_RESULT_PATH / PRD_AUTOPILOT_SCHEMA_PATH env vars if available.

PRD card content:
---
---
id: "BUG-0002"
title: "把页脚的上海地址改为北京朝阳区的一个随机地址"
type: "bug" # bug | feature | improvement
status: "pending" # source of truth (drafts | pending | in-progress | blocked | in-review | done | archived)
priority: "P0" # P0 | P1 | P2 | P3
severity: "S2" # (bug only) S0 | S1 | S2 | S3
component: "ui"
owner: "codex"
reporter: ""
created_at: "2026-02-10"
updated_at: "2026-02-10"
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
---

Now begin.

Reminder: Immediately before the FINAL JSON, output a short natural-language summary message.
Reminder: Your FINAL message must be a single JSON object matching the schema.