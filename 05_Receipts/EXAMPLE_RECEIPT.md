# Example Receipt

This filled example shows what a worker handoff can look like after completing a bounded task.

It is intentionally sanitized: it uses this public repository as the example project, avoids private paths, avoids customer data, and does not claim external validation.

```yaml
task_id: example-readme-quick-start-001
worker_role: Technical Path Architect
runtime: Codex
started_from: 04_Task_Packets/EXAMPLE_TASK_PACKET.md
completed_at: 2026-05-27

goal: Propose a minimal README quick-start path so a first-time reader can understand the repo in about 10 minutes.

done:
  - Added a concrete first-reader path to README.md.
  - Pointed readers to the architecture map, CEO entry, filled task packet example, empty task packet template, and role library.
  - Kept the path framed as public reference material, not a validated product workflow.

changed:
  files:
    - README.md
    - 04_Task_Packets/EXAMPLE_TASK_PACKET.md

evidence:
  files:
    - path: README.md
      note: Contains the quick-start and start-here path.
    - path: 04_Task_Packets/EXAMPLE_TASK_PACKET.md
      note: Shows a filled task packet for the README quick-start task.
  commands:
    - command: git status --short
      result: Used to confirm the changed files before handoff.
  artifacts:
    - README quick-start section
    - filled task packet example

tests:
  run:
    - Link check by reading the referenced paths in the repository.
  result: All referenced local files existed at handoff time.

risks:
  - The 10-minute path has not been tested with an external reader.
  - The repository license is still undecided.
  - This example covers one README task only; it does not prove every role or workflow.

do_not_claim:
  - Do not claim this path has been externally validated.
  - Do not claim the repo is production-ready software.
  - Do not claim this example proves user demand, adoption, stars, PRs, revenue, or growth.

open_questions:
  - Which license should the author choose?
  - Should future examples include a completed review receipt?
  - Where do new readers get stuck when filling their first task packet?

next_owner: CEO
next_action: Ask one new reader to copy the task packet template, fill one real task, and report where they got stuck.
stop_condition: Stop if the next change requires a legal license decision or private project material.
```
