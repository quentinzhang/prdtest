You are a coding agent working on ONE PRD card.

Required skill:
- You MUST use the prd-worker skill for this run.
- If you cannot access prd-worker, finish with outcome="blocked" and include a blocker: "prd-worker skill unavailable".

Card ID: IMP-0003
Project: test
Repo: /var/www/prdtest
Worktree: /var/www/prdtest/.worktrees/test/IMP-0003
Codex invoke: exec
Result schema: /private/var/www/prd/skills/prd-worker/assets/result.schema.json
Result JSON path: /var/www/prdtest/.worktrees/test/IMP-0003/.prd-autopilot/results/test-IMP-0003.json
Worker log path: /var/www/prdtest/.worktrees/test/IMP-0003/.prd-autopilot/results/test-IMP-0003.log
Date: 2026-02-10
Started at: 2026-02-10T04:27:09.701Z

Hard constraints:
- Do NOT edit the PRD hub at /private/var/www/prd. Treat it as read-only.
- Work ONLY inside the repo worktree at: /var/www/prdtest/.worktrees/test/IMP-0003
- Immediately before the FINAL JSON, output a short natural-language summary message (not JSON).
- You MUST finish by emitting a FINAL JSON response matching the required output schema.
- Your FINAL message must be ONLY the JSON object (no prose before/after).
- Include the same human-readable summary inside the FINAL JSON "notes" field so it is captured in logs/artifacts.
  - outcome: "in-review" if you implemented + validated the change.
  - outcome: "blocked" if you cannot proceed (missing info, cannot run validation, unclear AC, etc.).

PRD card content:
---
---
id: "IMP-0003"
title: "将咖啡馆名称改为拾壹咖啡，且today的咖啡改为：哥伦比亚 · 慧兰"
type: "improvement" # bug | feature | improvement
status: "pending" # source of truth (drafts | pending | in-progress | blocked | in-review | done | archived)
priority: "P0" # P0 | P1 | P2 | P3
severity: null # (bug only) S0 | S1 | S2 | S3
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