# Task Packet Template

Use this before opening a worker window.

```yaml
task_id:
created_at:
created_by:
target_role:
runtime: Codex | Claude Code | Claude | other

goal:
why_now:
business_or_project_context:

scope:
  in:
  out:

read_first:
  - path:
    reason:

allowed_tools:
  - tool:
    reason:

required_skills:
  - skill:
    reason:

actions:
  - step:
    expected_result:

acceptance_criteria:
  - criterion:

verification:
  commands:
    - command:
      expected:
  artifacts:
    - path_or_description:

do_not:
  - rule:

stop_if:
  - condition:

context_budget:
  max_percent: 60
  handoff_required_at_percent: 55

output_format:
  required_receipt: true
  summary_style:
```

## Tiny Task Packet

Use for small tasks:

```text
Goal:
Role:
Read:
Do:
Verify:
Do not:
Stop if:
Output:
```
