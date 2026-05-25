# Role Card Template

```yaml
role_name:
version:
owner: CEO
status: draft | active | deprecated

mission:

can_do:
  - 

cannot_do:
  - 

read_first:
  - path:
    reason:

allowed_tools:
  - tool:
    reason:

required_skills:
  - skill:
    reason:

input_contract:
  required:
  optional:

output_contract:
  format:
  required_fields:

verification:
  - 

context_budget:
  read_phase_percent:
  execute_phase_percent:
  verify_phase_percent:
  receipt_phase_percent:

escalate_to_ceo_if:
  - 

default_next_owner:

failure_modes:
  - 

prompt_notes:
```

## Role Quality Gate

Before a role becomes active, check:

- The role has a narrow mission.
- The role has explicit cannot-do rules.
- The role names allowed tools.
- The role has a required output contract.
- The role has escalation triggers.
- The role can finish a normal task before 60% context.
