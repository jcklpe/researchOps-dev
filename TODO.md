# Development Index
## Current State
The maintainer repository contains the HackPack as a pinned submodule and has the public origin https://github.com/jcklpe/researchOps-dev. As of 2026-10-13, the first product slice is implemented and locally verified. Aslan authorized local commits and will push, then test the exact published README setup prompt. Push the consumer commit before the outer repository's updated pin. Human QA and spike closure remain pending.

## Active Spikes
- **Portable runbooks and mechanical setup** — [concept and scope](docs/active-spikes/portable-runbooks-and-setup.md) · [work list and human QA](docs/active-spikes/portable-runbooks-and-setup.todo.md). Implemented project → trial → artifacts, flat templates, three fictional method examples, portable runbooks with GitHub adapters, four mechanical skills, and the revised README. Awaiting the published fresh-agent walkthrough; the spike is still active.

## Later Work
These clusters are retained in the [active spike's scope discussion](docs/active-spikes/portable-runbooks-and-setup.md#later-work-clusters), not started as separate spikes:
- Research framework and template content: UX Epistemology, methods rigor, terminology, and possible structural changes.
- Further agent assistance: human authorship, boundaries of delegation, and competitive analysis of actual workflows and toolkit architecture.
- Optional integrations and tools: tracker/document destinations and possible MCP dependencies.
- Evidence and provenance: original materials, traceability, and the [pinned artifact-storage question](docs/pinned-issues.md).

## Completed Setup
- Established the outer maintainer repository and registered the existing consumer template as a pinned submodule.
- Separated maintainer documentation from consumer-facing template files; durable guidance lives in `docs/policies/`.
- Included the five maintainer workflow skills under `skills/`.
- Added AGPLv3 licensing for the maintainer repository.
