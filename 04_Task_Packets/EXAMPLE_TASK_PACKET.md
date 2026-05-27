# Example Task Packet

This filled example shows how to turn a vague founder thought into a bounded AI worker task.

```yaml
task_id: example-readme-quick-start-001
created_at: 2026-05-27
created_by: CEO
target_role: Technical Path Architect
runtime: Codex

goal: Propose a minimal README quick-start path so a first-time reader can understand the repo in 10 minutes.
why_now: The repo is understandable as an architecture manual, but a new reader may not know what to open first.
business_or_project_context: Signal AI Company OS is a public reference for a solo founder using multiple AI windows with role boundaries, task packets, receipts, and memory.

scope:
  in: README quick-start copy, links to existing files, one suggested example path.
  out: New product claims, growth promises, external validation claims, large restructuring.

read_first:
  - path: README.md
    reason: Understand the current first-reader experience.
  - path: 00_CEO/CEO_START_HERE.md
    reason: Understand the CEO operating loop.
  - path: 09_Visuals/solo_company_architecture.html
    reason: Understand the visual architecture map.
  - path: 02_Role_Library/ROLE_LIBRARY_INDEX.md
    reason: Understand the role library entry point.

allowed_tools:
  - tool: text editor
    reason: Draft a small README change.

required_skills:
  - skill: evidence audit
    reason: Separate what the repo publicly shows from what the author intends.

actions:
  - step: Identify the fastest path from repo landing page to whole-system understanding.
    expected_result: A 3-5 step reader path using existing files.
  - step: Draft quick-start copy.
    expected_result: A short, concrete section that does not overclaim.
  - step: Check every link.
    expected_result: All linked files exist in the repo.

acceptance_criteria:
  - A new reader can tell what the repo helps them understand.
  - The path can be completed in about 10 minutes.
  - The copy does not claim external user validation.
  - The copy does not promise stars, users, PRs, revenue, or growth.

verification:
  commands:
    - command: git status --short
      expected: Only README and task-packet files changed for this task.
  artifacts:
    - path_or_description: README quick-start section
    - path_or_description: this filled task packet

do_not:
  - rule: Do not create a full contribution process.
  - rule: Do not claim the 10-minute path has been externally tested.
  - rule: Do not choose a license on behalf of the author.

stop_if:
  - condition: The requested change requires a legal license decision.

context_budget:
  max_percent: 60
  handoff_required_at_percent: 55

output_format:
  required_receipt: true
  summary_style: concise change summary with remaining boundaries
```
