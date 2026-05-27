# Signal AI Company OS

中文入口: [README.zh-CN.md](README.zh-CN.md)

Signal AI Company OS is a local-first operating system for a solo AI company.

It turns one founder's judgment into bounded AI work:

```text
raw thought -> clarified intent -> task packet -> bounded worker -> review -> receipt -> memory -> next decision
```

## Core Rule

```text
One window = one role = one bounded task = one receipt.
```

The CEO owns direction, role tuning, final commitments, public narrative, and resource allocation. AI workers own execution inside explicit boundaries.

## Repository Map

## 5-Minute Quick Start

Use this repo to understand how a solo founder can split AI work safely. Fastest path: open the architecture map, read the CEO entry, then compare one role card in the role library. In 5 minutes, you should have a whole-system map.

| Path | Purpose |
|---|---|
| `00_CEO/` | CEO entry, daily loop, decision authority |
| `01_Architecture/` | Operating architecture and context rules |
| `02_Role_Library/` | Role library and role card templates |
| `03_Prompt_Library/` | Prompt stack and worker prompt templates |
| `04_Task_Packets/` | Task packet templates and a filled example |
| `05_Receipts/` | SACP-style receipt templates |
| `06_Project_Sync/` | Project sync board |
| `07_Learning/` | CEO full-stack learning loop |
| `08_Info_Flow/` | CEO information filtering system |
| `09_Visuals/` | Local HTML architecture diagrams |

## Start Here

Use this 10-minute path to understand whether the system fits your work:

1. Read the 5-minute quick start above to understand what this repo is for.
2. Open [09_Visuals/solo_company_architecture.html](09_Visuals/solo_company_architecture.html) to see the full operating map.
3. Read [00_CEO/CEO_START_HERE.md](00_CEO/CEO_START_HERE.md) to understand the CEO loop and core principles.
4. Read [04_Task_Packets/EXAMPLE_TASK_PACKET.md](04_Task_Packets/EXAMPLE_TASK_PACKET.md), then compare it with the empty task packet template.
5. Open [02_Role_Library/ROLE_LIBRARY_INDEX.md](02_Role_Library/ROLE_LIBRARY_INDEX.md), choose one role closest to your current need, and decide whether this method fits your scenario.

After that, tune the first three active roles:
   - CEO Clarification Partner
   - Technical Path Architect
   - Claude Code Reviewer

## Design Principles

- Do not put full-stack execution into one AI window.
- Split implementation and review.
- Keep raw thoughts out of execution prompts until curated.
- Treat HTML as a visual working surface, not the source of truth.
- Treat Markdown as the durable operating memory.
- Every meaningful worker window must end with a receipt.

## Status

This is an initial architecture repo. Role cards and prompt templates are intentionally designed to be tuned by the CEO over time.

Current stage: public reference. Feedback via issues is welcome, PRs are not being accepted yet. You are welcome to fork and adapt the system for your own use.
