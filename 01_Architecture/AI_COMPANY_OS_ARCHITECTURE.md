# AI Company OS Architecture

## Core Thesis

A solo AI company is not a small version of a big company. It is a context-controlled execution system.

The unit of work is not "department" or "employee". The unit of work is:

```text
one window = one role = one bounded task = one receipt
```

## Layers

### 1. CEO Layer

Owns direction, judgment, narrative, final decisions, capital allocation, and public commitments.

### 2. Clarification Layer

Turns raw CEO intent into concrete requirements.

Required outputs:

- clarified intent
- assumptions
- non-goals
- acceptance criteria
- open questions
- decision required from CEO

### 3. Architecture Layer

Determines technical path before execution.

Required outputs:

- frontend/backend/data/design/testing split
- build vs buy
- tools and MCP needs
- affected files or repos
- risks
- verification path

### 4. Role Routing Layer

Chooses the next worker window.

Rules:

- do not route full-stack work into one window
- split implementation and review
- split design and frontend implementation when quality matters
- split evidence collection and claim writing
- split raw thought curation and platform distribution

### 5. Execution Layer

Codex and Claude Code are worker runtimes.

Default division:

- Codex: implementation, file edits, tests, local verification, artifact generation
- Claude Code: review, architecture critique, code review, prompt/role critique, second-pass reasoning

### 6. Review Layer

No worker reviews its own work as final authority.

Review types:

- code review
- UI/design review
- test/QA review
- security review
- claim-boundary review
- memory consistency review

### 7. Receipt and Memory Layer

Every meaningful work window ends with a SACP-style receipt.

Receipts feed:

- project sync board
- Obsidian memory
- role improvements
- prompt improvements
- next task packet

## 60% Context Rule

```text
0-15%: read role, task, and minimal memory
15-45%: execute
45-55%: verify
55-60%: write receipt and next handoff
60-75%: only compress and hand off
75%+: stop execution
```

## Source of Truth Order

1. Latest explicit CEO decision.
2. CEO decision log.
3. Project sync board.
4. Role library.
5. Prompt library.
6. Latest receipt.
7. Historical worklogs.
8. Raw thoughts and brainstorms.

Raw thoughts are valuable, but they are not execution instructions until curated.
