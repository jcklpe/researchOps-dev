# Agent Instructions
This is the ResearchOps HackPack maintainer repository, an independently versioned development project. Version-control project documentation, configuration, and implementation files as appropriate to the project.

## Repository Boundaries
`researchOps-hackpack/` is a separate Git repository registered as a submodule. Consumer-facing changes belong there; maintainer reasoning, unfinished tasks, policies, and development history belong here. Check Git roots and status before editing or committing. Preserve unrelated user changes.

Keep project documentation usable after cloning, without dependencies on machine-specific paths or private external workspaces.

## Development Workflow
Use `TODO.md` as the index. Bounded development work uses a conceptual document and a `.todo.md` companion in `docs/active-spikes/`. Rough exploration belongs in `docs/scratch/`; current policies in `docs/policies/`; completed or superseded spike history in `docs/archive/`. Policies describe the current approach, including rules, defaults, procedures, and useful rationale. Revise them directly; Git holds their history. Use applicable project-workflow skills when available. Do not adopt exploratory agent suggestions as requirements.

Human researchers author inquiry. Agents can help articulate, challenge, retrieve, organize, and execute work in service of that inquiry. Agent-generated documents do not by themselves demonstrate research progress. The exact product approach remains open.

## Repo-Local Skills
Prefer `skills/<skill-name>/SKILL.md` over a similarly named global skill. These local copies govern the maintainer workflow and may evolve with the project; global skills are fallback material. Load the relevant skill from its explicit path when needed.

- `run-project-spike`: scoped development work, conceptual/to-do pairs, continuation, and archival.
- `commit-work`: authorized local checkpoints and their scope.
- `triage-project-misc`: route loose development observations.
- `pin-issue`: preserve unresolved questions with a revisit condition.
- `log-future-idea`: record future infrastructure, tooling, or development-workflow ideas; research questions and other domain content belong in their relevant project context.

Honor requested review periods: when the maintainer asks to review before committing, leave changes uncommitted until that review ends or a checkpoint is explicitly requested. Do not push without authorization.

## Validation and Commits
Validate documentation links and Git boundaries after structural changes. Run checks appropriate to any implementation changes. Commit authorized, completed project work locally at a verified completion boundary. Use the commit-work skill when available, explicit paths, and no co-author trailers. Never push or create a remote without authorization.

Commit consumer changes in the submodule first, then update the outer repository's pinned commit when the change is ready. Do not silently advance the submodule to the latest remote revision.

## Privacy
Keep credentials, secrets, and local agent state out of Git. Check that any research materials included in the repository are suitable for its public audience.

## Markdown And Prose Style
Do not hard-wrap prose. Preserve paragraph boundaries and avoid reflow-only diffs. Prefer compact heading spacing in hand-authored files unless project tooling requires otherwise.

`CLAUDE.md` links to this file so the same instructions apply to both agents.
