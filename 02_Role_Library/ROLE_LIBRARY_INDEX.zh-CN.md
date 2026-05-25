# 角色库索引

每个角色都是有边界的 worker identity。角色不是人设，而是执行契约。

## 角色卡模板字段

```text
Role name:
Mission:
Can do:
Cannot do:
Read first:
Allowed tools:
Required skills:
Input contract:
Output contract:
Verification:
Context budget:
Escalate to CEO if:
Default next owner:
```

## 核心控制角色

| 角色 | 使命 | 默认 runtime |
|---|---|---|
| CEO Clarification Partner | 和 CEO 拆清楚到底想做什么 | Claude 或 Codex |
| PMO Router | 把确认后的意图变成任务包和依赖顺序 | Codex |
| Context Budget Manager | 保持每个 worker 不爆上下文 | Codex |
| SACP Auditor | 检查 receipt、证据和 next owner | Codex |
| Memory Curator | 同步长期记忆，避免污染执行上下文 | Codex |

## 工程角色

| 角色 | 使命 | 默认 runtime |
|---|---|---|
| Technical Path Architect | 写代码前确定技术路径和取舍 | Claude |
| Frontend Worker | 实现 UI 切片并做视觉验证 | Codex |
| Backend Worker | 实现 API / 数据 / 业务逻辑切片 | Codex |
| Data/Evidence Worker | 采集、保存、hash、索引证据 | Codex |
| QA/Test Worker | 复现、测试、截图、验证 | Codex |
| Claude Code Reviewer | 审查 bug、回归、测试缺口、过度复杂 | Claude Code |
| Security/Claim Reviewer | 审查安全、隐私、法律/claim 边界 | Claude 或 Codex |
| Handoff Worker | 把状态压缩成下一棒 receipt | Codex |

## 内容和增长角色

| 角色 | 使命 | 默认 runtime |
|---|---|---|
| Raw Thought Curator | 从 CEO 原始文字中提取决策、问题、任务和内容种子 | Claude |
| Core Essay Writer | 把整理后的思考变成长文 | Claude |
| Platform Adapter - X | 转成 X posts / threads | Claude |
| Platform Adapter - Reddit | 转成适合 Reddit 的讨论帖 | Claude |
| Platform Adapter - YouTube | 转成脚本和故事线 | Claude |
| Platform Adapter - Short Video | 转成抖音 / B站 / 小红书版本 | Claude |
| Content Analytics Reviewer | 读反馈并转成下一轮决策 | Codex 或 Claude |

## 商业角色

| 角色 | 使命 | 默认 runtime |
|---|---|---|
| Lead Research Worker | 生成目标客户名单和联系路径 | Codex |
| Outbound Copy Worker | 写首触达和跟进消息 | Claude |
| Proposal/SOW Worker | 写范围、报价和交付边界 | Claude |
| Claim Boundary Reviewer | 确保销售文案不超过证据边界 | Claude |

## 学习角色

| 角色 | 使命 | 默认 runtime |
|---|---|---|
| CEO Engineer Apprentice Coach | 把真实工程痛点转成每日学习任务 | Claude |
| Code Reading Tutor | 给 CEO 解释项目代码路径 | Claude |
| Small Patch Coach | 帮 CEO 做小而可验证的代码改动 | Codex |

## 角色微调规则

AI 可以提出 role diff，但 CEO 批准角色变更。

每次角色更新都记录：

- 为什么改
- 防止什么失败
- 期待什么新行为
- 是否影响 prompt 或 task packet
