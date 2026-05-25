# Role Library Index

Each role is a bounded worker identity. A role is not a personality. It is an execution contract.

## Role Card Template

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

## Core Control Roles

| Role | Mission | Default Runtime |
|---|---|---|
| CEO Clarification Partner | Interview CEO until intent is concrete | Claude or Codex |
| PMO Router | Convert approved intent into task packets and dependency order | Codex |
| Context Budget Manager | Keep each worker under the context budget | Codex |
| SACP Auditor | Check receipts, evidence, and next-owner handoff | Codex |
| Memory Curator | Sync durable memory without polluting execution context | Codex |

## Engineering Roles

| Role | Mission | Default Runtime |
|---|---|---|
| Technical Path Architect | Choose implementation path and tradeoffs before coding | Claude |
| Frontend Worker | Implement UI slices with visual verification | Codex |
| Backend Worker | Implement API/data/business logic slices | Codex |
| Data/Evidence Worker | Capture, preserve, hash, and index evidence | Codex |
| QA/Test Worker | Reproduce, test, screenshot, and verify | Codex |
| Claude Code Reviewer | Review implementation for bugs, regressions, missing tests, overcomplexity | Claude Code |
| Security/Claim Reviewer | Review safety, privacy, legal/claim boundaries | Claude or Codex |
| Handoff Worker | Compress state into next-task receipt | Codex |

## Content and Growth Roles

| Role | Mission | Default Runtime |
|---|---|---|
| Raw Thought Curator | Extract decisions, questions, tasks, and content seeds from CEO writing | Claude |
| Core Essay Writer | Turn curated thought into durable longform | Claude |
| Platform Adapter - X | Convert core thought into X posts/threads | Claude |
| Platform Adapter - Reddit | Convert core thought into discussion-native posts | Claude |
| Platform Adapter - YouTube | Convert core thought into script/storyline | Claude |
| Platform Adapter - Short Video | Convert core thought into Douyin/Bilibili/Xiaohongshu variants | Claude |
| Content Analytics Reviewer | Read feedback and turn it into next decisions | Codex or Claude |

## Commercial Roles

| Role | Mission | Default Runtime |
|---|---|---|
| Lead Research Worker | Build target lists and contact paths | Codex |
| Outbound Copy Worker | Draft first-touch and follow-up messages | Claude |
| Proposal/SOW Worker | Draft scope, price, and delivery terms | Claude |
| Claim Boundary Reviewer | Ensure sales copy does not outrun evidence | Claude |

## Learning Roles

| Role | Mission | Default Runtime |
|---|---|---|
| CEO Engineer Apprentice Coach | Turn real engineering pain into daily learning tasks | Claude |
| Code Reading Tutor | Explain project code paths to CEO | Claude |
| Small Patch Coach | Help CEO make tiny verified code changes | Codex |

## Role Tuning Rule

AI may propose role diffs, but CEO approves role changes.

Every role update should record:

- why it changed
- what failure it prevents
- what new behavior is expected
- whether it affects prompts or task packets
