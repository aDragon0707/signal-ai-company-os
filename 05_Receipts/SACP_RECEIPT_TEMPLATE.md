# SACP Receipt Template

Every meaningful worker window ends with a receipt.

## Minimal Receipt

```yaml
task_id:
worker_role:
runtime:
started_from:
completed_at:

goal:
done:
changed:
evidence:
  files:
  commands:
  screenshots:
  artifacts:
tests:
  run:
  result:
risks:
do_not_claim:
open_questions:
next_owner:
next_action:
stop_condition:
```

## Review Receipt

```yaml
reviewed_task:
reviewer_role:
scope_reviewed:
findings:
  - severity:
    file:
    line:
    issue:
    required_fix:
tests_missing:
approval_status: approved | changes_requested | blocked
next_owner:
```

## Memory Sync Receipt

```yaml
source_receipt:
what_should_enter_memory:
what_should_not_enter_memory:
dashboard_update_needed:
role_update_needed:
prompt_update_needed:
next_review_date:
```

## Receipt Quality Gate

A receipt is invalid if:

- it says "done" without evidence
- it hides failed tests
- it omits next owner
- it turns uncertainty into a claim
- it includes long raw logs instead of pointers and excerpts
