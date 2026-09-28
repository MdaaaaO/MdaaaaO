I build data platforms that companies bet their numbers on, and the tooling that keeps them running. My specialty is entity and identity resolution. Now I'm focused on AI-ready infrastructure: systems that ML and agents can operate on directly.

#### ai-baton: new in 0.5

- **Sessions keep each other honest.** Every session now leaves a ready-to-use prompt for the next one, checks its own work against the kit before it closes, and signs the pull requests it opens, so a new session can pick up where the last one stopped.
- **The right model for each job.** Reading and sorting goes to a small, cheap model and routine fixes to a mid-size one. The largest model is kept for judgement calls, which cuts cost without cutting quality.
- **Safer by default.** Checks catch private names and secrets before they leave the machine, reviews are tied to the exact change they approved, and every script now runs the same on Linux, WSL and macOS.
- **Sturdier throughout.** More than fifty fixes found by reviewing the whole kit: no more silent failures, clearer errors, and tests that cannot touch your real setup.

[Release notes](https://github.com/MdaaaaO/ai-baton/releases/tag/v0.5.0)

#### Coming in ai-baton 0.6

- **Shared memory that answers.** ai-baton will keep its notes in [ctx-store](https://github.com/MdaaaaO/ctx-store). Describe the task, and the session opens with the few notes that matter instead of reading everything.
- **Every skill tested.** Each skill gets its own examples that prove it still triggers and behaves after a change.
- **Easier first steps.** Clearer setup docs, so a new user gets from install to a first working session faster.

[Follow along](https://github.com/MdaaaaO/ai-baton/milestone/3)

#### At Docker

On the Data Platform team. I work on canonical data products, event pipelines and the internal tooling around them, including agent tooling for the team's own workflow.

#### Before that

- Eight years at Atlassian. I co-architected the customer master-data platform that unified 300,000+ customers into a single source of truth, and built an identity graph ingesting 100M+ behavioural events a day.
- Wrote and open-sourced [Observe](https://github.com/atlassian-labs/observe), a Python observability decorator. [observe-kit](https://github.com/MdaaaaO/observe-kit) is its rewrite.
- Co-inventor of a collaborative data-quality framework, [U.S. Patent 10,909,109](https://patents.google.com/patent/US10909109B1/en).

#### What I'm building now

| Project | What it does |
|---|---|
| [ai-baton](https://github.com/MdaaaaO/ai-baton) | A workspace kit for Claude Code: shared skills, rules and memory for every session, handoffs between sessions, and a self-check that keeps every machine healthy. |
| [conventional-release](https://github.com/MdaaaaO/conventional-release) | CHANGELOG and release PRs from Conventional Commits, tagged by CI after merge. No Node. |
| [observe-kit](https://github.com/MdaaaaO/observe-kit) | `@observed`: one Python decorator that times a call, classifies how it ended, logs it with structlog and emits an event. On [PyPI](https://pypi.org/project/observe-kit/). |
| [ctx-store](https://github.com/MdaaaaO/ctx-store) | A markdown context store for coding agents: validated writes, budgeted reads, audit trail. Early stage. |

Questions or ideas? Open an issue on the relevant repo.
