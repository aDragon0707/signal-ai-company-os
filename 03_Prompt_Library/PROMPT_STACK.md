# Prompt Stack

Prompt quality comes from layered constraints, not one giant prompt.

## Layers

### 1. Company Constitution

Stable company-wide rules.

Includes:

- CEO authority
- evidence rules
- context budget
- role boundaries
- receipt requirement

Excludes:

- temporary task details
- full project history
- raw brainstorming

### 2. Project Rules

Project-level instructions such as `AGENTS.md`, `CLAUDE.md`, commands, architecture notes, and source-of-truth order.

Includes:

- repo path
- build/test commands
- directory map
- coding boundaries
- claim boundaries

### 3. Role Card

Worker identity and allowed behavior.

Includes:

- mission
- can/cannot do
- allowed tools
- required skills
- output format
- escalation triggers

### 4. Task Packet

Current executable task.

Includes:

- goal
- scope
- files/paths
- actions
- acceptance criteria
- verification command
- stop rule

### 5. Evidence Tail

Latest relevant facts.

Includes:

- failing test
- screenshot
- review finding
- artifact path
- user feedback

Excludes:

- full logs when a small excerpt is enough
- stale assumptions
- unrelated chat history

### 6. Receipt

End-of-window state.

Includes:

- done
- changed
- evidence
- tests
- risks
- do not claim
- next owner
- next action

## Worker Prompt Template

```text
You are: [role name]

Mission:
[one sentence]

Current task:
[bounded task]

Read first:
- [path or receipt]
- [path or spec section]

Allowed tools:
- [tools]

Required skill behavior:
- [skill or method]

Acceptance criteria:
- [criterion]

Verification:
- [command, screenshot, review, artifact]

Do not:
- [forbidden action]

Stop if:
- [stop condition]

Output:
- [required receipt format]
```

## Prompt Quality Gate

A prompt is not ready if:

- it asks one worker to do implementation and final review
- it lacks acceptance criteria
- it lacks a stop rule
- it includes raw history instead of curated context
- it does not name files, artifacts, or evidence
- it does not say what the worker must not do
