I build data platforms that companies bet their numbers on, and the tooling that keeps them running. My specialty is entity and identity resolution. Now I'm focused on AI-ready infrastructure: systems that ML and agents can operate on directly.

#### ai-baton, at 0.11

A workspace kit for Claude Code, built for the moment one session is not enough.

- **Context that accumulates.** Sessions write what they learn into a markdown database beside the repos, optionally its own git repo that every machine pulls. The next session does not start cold.
- **Sessions choose their context.** An index names every doc and a brief per initiative; a session reads what it works on, not everything, so the loaded context and the cost stay small.
- **Initiatives outlive sessions.** One doc per initiative. A session ends with a handoff prompt; its successor reads it back, checks each claim against the tracker and the open pull requests, and only then edits. A stale prompt is caught before it is acted on.
- **A live registry.** Who works on what right now, with heartbeats, the pull requests each session watches and what each session cost, so a second session coordinates instead of colliding.
- **Tooling, not prose.** Index, registry, session stats, health check and sync are scripts and hooks that run with zero model turns; the skills are the thin layer on top. One install command, one setup run, no names or ids in the kit.

[Releases](https://github.com/MdaaaaO/ai-baton/releases) · [Discussions](https://github.com/MdaaaaO/ai-baton/discussions)

#### At Docker

On the Data Platform team. I work on canonical data products, event pipelines and the internal tooling around them, including agent tooling for the team's own workflow.

#### Before that

- Eight years at Atlassian. I co-architected the customer master-data platform that unified 300,000+ customers into a single source of truth, and built an identity graph ingesting 100M+ behavioural events a day.
- Wrote and open-sourced [Observe](https://github.com/atlassian-labs/observe), a Python observability decorator. [observe-kit](https://github.com/MdaaaaO/observe-kit) is its rewrite.
- Co-inventor of a collaborative data-quality framework, [U.S. Patent 10,909,109](https://patents.google.com/patent/US10909109B1/en).

#### What I'm building now

| Project | What it does |
|---|---|
| [ai-baton](https://github.com/MdaaaaO/ai-baton) | A workspace kit for Claude Code: a context database that grows with every session, a live registry of who works on what, and handoffs that let an initiative outlive any one session. |
| [conventional-release](https://github.com/MdaaaaO/conventional-release) | CHANGELOG and release PRs from Conventional Commits, tagged by CI after merge. No Node. |
| [observe-kit](https://github.com/MdaaaaO/observe-kit) | `@observed`: one Python decorator that times a call, classifies how it ended, logs it with structlog and emits an event. On [PyPI](https://pypi.org/project/observe-kit/). |
| [ctx-store](https://github.com/MdaaaaO/ctx-store) | A markdown context store for coding agents: validated writes, budgeted reads, audit trail. ai-baton's storage engine. |

Questions or ideas? Open an issue on the relevant repo.
