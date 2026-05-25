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

| Path | Purpose |
|---|---|
| `00_CEO/` | CEO entry, daily loop, decision authority |
| `01_Architecture/` | Operating architecture and context rules |
| `02_Role_Library/` | Role library and role card templates |
| `03_Prompt_Library/` | Prompt stack and worker prompt templates |
| `04_Task_Packets/` | Task packet templates |
| `05_Receipts/` | SACP-style receipt templates |
| `06_Project_Sync/` | Project sync board |
| `07_Learning/` | CEO full-stack learning loop |
| `08_Info_Flow/` | CEO information filtering system |
| `09_Visuals/` | Local HTML architecture diagrams |

## Start Here

1. Read [00_CEO/CEO_START_HERE.md](00_CEO/CEO_START_HERE.md).
2. Read [01_Architecture/AI_COMPANY_OS_ARCHITECTURE.md](01_Architecture/AI_COMPANY_OS_ARCHITECTURE.md).
3. Open [09_Visuals/solo_company_architecture.html](09_Visuals/solo_company_architecture.html) in a browser.
4. Tune the first three active roles:
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
