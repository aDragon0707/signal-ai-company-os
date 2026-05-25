# AI Company OS 总架构

## 核心命题

一人 AI 公司不是大公司的缩小版，而是一个上下文受控的执行系统。

工作单位不是“部门”，也不是“员工”，而是：

```text
一个窗口 = 一个角色 = 一个 bounded task = 一个 receipt
```

## 分层

### 1. CEO 层

负责方向、判断、叙事、最终决策、资源配置和公开承诺。

### 2. 需求澄清层

把 CEO 的原始想法变成具体需求。

必须输出：

- 澄清后的意图
- 假设
- 非目标
- 验收标准
- open questions
- 需要 CEO 决策的点

### 3. 架构层

执行前先确定技术路径。

必须输出：

- 前端 / 后端 / 数据 / 设计 / 测试拆分
- build vs buy
- 工具和 MCP 需求
- 影响的文件或 repo
- 风险
- 验证路径

### 4. 角色路由层

选择下一个 worker 窗口。

规则：

- 不把全栈工作塞进一个窗口
- 实现和 review 分开
- 高质量 UI 需要拆设计和前端实现
- 证据采集和 claim 写作分开
- 原始思考整理和平台分发分开

### 5. 执行层

Codex 和 Claude Code 是 worker runtime。

默认分工：

- Codex：实现、文件编辑、测试、本地验证、artifact 生成
- Claude Code：review、架构质疑、代码审查、prompt/role 质疑、第二轮推理

### 6. 审查层

任何 worker 都不能把自己的工作当成最终审查。

审查类型：

- 代码审查
- UI / 设计审查
- 测试 / QA 审查
- 安全审查
- claim 边界审查
- 记忆一致性审查

### 7. Receipt 和记忆层

每个重要工作窗口都以 SACP 风格 receipt 收口。

Receipt 回流到：

- project sync board
- Obsidian 记忆
- 角色改进
- prompt 改进
- 下一个 task packet

## 60% 上下文规则

```text
0-15%: 读取角色、任务和最小记忆
15-45%: 执行
45-55%: 验证
55-60%: 写 receipt 和下一棒 handoff
60-75%: 只允许压缩和交接
75%+: 停止执行
```

## 真源顺序

1. CEO 最新明确决策。
2. CEO decision log。
3. Project sync board。
4. Role library。
5. Prompt library。
6. 最新 receipt。
7. 历史 worklog。
8. 原始思考和 brainstorm。

原始思考很有价值，但在整理前不是执行指令。
