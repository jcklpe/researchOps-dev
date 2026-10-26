# Development Index
## Current State
The maintainer repository contains the HackPack as a pinned submodule and has the public origin https://github.com/jcklpe/researchOps-dev. As of 2026-10-13, the first product slice is implemented and locally verified. Aslan subsequently reported testing the entry path: it worked “kind of okay,” with much more work remaining. Test details and specific friction have not yet been captured. The spike stays active; closure and full acceptance are not established.

## Active Spikes
- **Project Workflows adoption** — [reconciliation](docs/active-spikes/project-workflows-adoption.md) · [local validation and publication hold](docs/active-spikes/project-workflows-adoption.todo.md).
- **Portable runbooks and mechanical setup** — [concept and scope](docs/active-spikes/portable-runbooks-and-setup.md) · [work list and human QA](docs/active-spikes/portable-runbooks-and-setup.todo.md). Implemented project → trial → artifacts, flat templates, three fictional method examples, portable runbooks with GitHub adapters, four mechanical skills, and the revised README. An initial user test is reported, with qualified feedback; detailed follow-up and the remaining QA criteria stay open.

## Context for Resuming
Aslan requested a detailed end-of-evening capture on 2026-10-13. Start with [the resume context](docs/scratch/researchops-resume-context.md), which links the authorship, methods/evidence, agent/tooling, and competitive-analysis scratch notes. They preserve discussion and later possibilities without starting new implementation work. Fuller private sources remain ignored.

## Later Work
These clusters are retained in the [active spike's scope discussion](docs/active-spikes/portable-runbooks-and-setup.md#later-work-clusters), not started as separate spikes:
- Research framework and template content: UX Epistemology, methods rigor, terminology, and possible structural changes.
- Further agent assistance: human authorship, boundaries of delegation, and competitive analysis of actual workflows and toolkit architecture.
- Optional integrations and tools: tracker/document destinations and possible MCP dependencies.
- Evidence and provenance: original materials, traceability, and the [pinned artifact-storage question](docs/scratch/research-artifact-naming-and-ignore-rules.md).

## Completed Setup
- Established the outer maintainer repository and registered the existing consumer template as a pinned submodule.
- Separated maintainer documentation from consumer-facing template files; durable guidance lives in `docs/policies/`.
- Included the five maintainer workflow skills under `skills/`.
- Added AGPLv3 licensing for the maintainer repository.
