# Signal AI Company OS（一人 AI 公司操作系统）

这是一个本地优先的一人 AI 公司操作系统。

它的目标不是让一个 AI 窗口变成“全栈万能员工”，而是把创始人的判断拆成可执行、可审查、可交接、可复利的工作链。

```text
原始思考 -> 需求澄清 -> 任务包 -> 有边界的 AI 员工 -> 审查 -> receipt -> 记忆 -> 下一轮决策
```

## 核心规则

```text
一个窗口 = 一个角色 = 一个 bounded task = 一个 receipt
```

CEO 负责方向、角色微调、最终承诺、公开叙事和资源配置。AI 员工只在明确边界内执行。

## 5 分钟快速上手

用这个仓库快速理解：一人创始人如何把 AI 工作拆成安全、可审查、可交接的任务。最快路径：打开架构图看全局，读 CEO 入口理解工作循环，再选一个角色卡对照理解。5 分钟内建立整体认知。

## 目录结构

| 路径 | 用途 |
|---|---|
| `00_CEO/` | CEO 入口、每日循环、决策权边界 |
| `01_Architecture/` | 总架构、上下文规则、执行分层 |
| `02_Role_Library/` | 角色库和角色卡模板 |
| `03_Prompt_Library/` | Prompt Stack 和 worker prompt 模板 |
| `04_Task_Packets/` | 任务包模板和已填实例 |
| `05_Receipts/` | SACP 风格 receipt 模板 |
| `06_Project_Sync/` | 项目同步板 |
| `07_Learning/` | CEO 全栈学习闭环 |
| `08_Info_Flow/` | CEO 信息流筛选系统 |
| `09_Visuals/` | 本地 HTML 架构图 |

## 从这里开始

用这条 10 分钟路径判断它是否适合你的工作：

1. 先读上面的 5 分钟快速上手，理解这个仓库能帮你做什么。
2. 用浏览器打开 [09_Visuals/solo_company_architecture.html](09_Visuals/solo_company_architecture.html)，看全局架构图。
3. 读 [00_CEO/CEO_START_HERE.zh-CN.md](00_CEO/CEO_START_HERE.zh-CN.md)，理解 CEO 工作循环和核心原则。
4. 读 [04_Task_Packets/EXAMPLE_TASK_PACKET.md](04_Task_Packets/EXAMPLE_TASK_PACKET.md)，再对照空任务包模板理解每个字段。
5. 打开 [02_Role_Library/ROLE_LIBRARY_INDEX.zh-CN.md](02_Role_Library/ROLE_LIBRARY_INDEX.zh-CN.md)，选一个与你当前需求最接近的角色，判断这套方法是否适合你的场景。

之后再精修三个角色：
   - CEO Clarification Partner（CEO 需求澄清伙伴）
   - Technical Path Architect（技术路径架构师）
   - Claude Code Reviewer（Claude 代码审查员）

## 设计原则

- 不把全栈任务塞进一个 AI 窗口。
- 实现和审查必须分离。
- 原始思考不能直接进入执行 prompt，必须先结构化。
- HTML 是可视化工作台，不是唯一真源。
- Markdown 是长期可维护的制度源文件。
- 每个重要 worker 窗口必须以 receipt 收口。

## 当前状态

这是初始总架构 repo。角色卡和 prompt 模板故意保留为可演化版本，后续应由 CEO 逐步微调。

当前阶段：公开参考。欢迎通过 issue 交流反馈，暂不接受 PR。欢迎 fork 并自行修改适配。
