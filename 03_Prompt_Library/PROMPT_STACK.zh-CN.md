# Prompt Stack

好的 prompt 不是一个巨大的咒语，而是分层约束。

## 1. Company Constitution

公司级稳定规则。

包含：

- CEO 权威
- 证据规则
- 上下文预算
- 角色边界
- receipt 要求

不包含：

- 临时任务细节
- 完整项目历史
- 原始 brainstorm

## 2. Project Rules

项目级说明，例如 `AGENTS.md`、`CLAUDE.md`、命令、架构说明、真源顺序。

包含：

- repo path
- build/test 命令
- 目录地图
- 编码边界
- claim 边界

## 3. Role Card

worker 身份和允许行为。

包含：

- mission
- can/cannot do
- allowed tools
- required skills
- output format
- escalation triggers

## 4. Task Packet

当前可执行任务。

包含：

- goal
- scope
- files/paths
- actions
- acceptance criteria
- verification command
- stop rule

## 5. Evidence Tail

最新相关事实。

包含：

- failing test
- screenshot
- review finding
- artifact path
- user feedback

不包含：

- 可用小片段替代的长日志
- 过期假设
- 无关聊天历史

## 6. Receipt

窗口结束状态。

包含：

- done
- changed
- evidence
- tests
- risks
- do not claim
- next owner
- next action

## Prompt 质量闸门

一个 prompt 没准备好，如果：

- 让同一个 worker 同时实现和最终审查
- 没有验收标准
- 没有 stop rule
- 用原始历史代替整理后的上下文
- 不命名文件、artifact 或证据
- 不说明 worker 不能做什么
