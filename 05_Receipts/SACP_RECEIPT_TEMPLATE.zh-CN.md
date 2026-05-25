# SACP Receipt 模板

每个重要 worker 窗口结束时必须留下 receipt。

## 最小 Receipt

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

## 记忆同步 Receipt

```yaml
source_receipt:
what_should_enter_memory:
what_should_not_enter_memory:
dashboard_update_needed:
role_update_needed:
prompt_update_needed:
next_review_date:
```

## Receipt 质量闸门

receipt 无效，如果：

- 说 done 但没有证据
- 隐藏失败测试
- 不写 next owner
- 把不确定性写成结论
- 用长 raw log 代替路径和摘录
