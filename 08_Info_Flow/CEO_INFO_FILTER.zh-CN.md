# CEO 信息流过滤器

CEO 信息系统的目标是把噪音变成决策、资产、技能或任务。

## 信息层

| 层 | 来源 | 用途 |
|---|---|---|
| Signal Radar | X、Reddit、YouTube、抖音、B站、小红书 | 发现弱信号 |
| Deep Sources | 官方文档、论文、repo、长文、案例 | 建立判断 |
| Books | 实体书和经典书 | 建立长期模型 |
| People Map | 创始人、工程师、客户、教授、操盘手 | 找真实实践者 |

## 筛选标准

每个信息源按这些维度打分：

- Cash：是否能帮助 7-30 天内产生收入？
- Skill：是否提升工程、销售、写作或判断？
- Asset：是否能变成文章、产品、工作流或代码？
- Trust：作者是否有一手证明？
- Fit：是否服务当前活跃项目？
- Cost：消耗多少注意力？

## Info Scout 输出

```yaml
source:
type:
why_it_matters:
score:
recommended_action: ignore | skim | deep_read | turn_into_task | turn_into_content | contact_person
evidence:
next_step:
```

## 规则

- 社交媒体是雷达，不是记忆库。
- 长文和书是深水区，不是无限摄入。
- 每个有用输入必须变成以下之一：
  - decision
  - task packet
  - essay seed
  - role/prompt improvement
  - contact/person map
  - project risk
