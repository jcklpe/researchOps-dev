# Agent Instructions
This is the ResearchOps HackPack maintainer repository, an independently versioned development project. Version-control project documentation, configuration, and implementation files as appropriate to the project.

## Repository Boundaries
`researchOps-hackpack/` is a separate Git repository registered as a submodule. Consumer-facing changes belong there; maintainer reasoning, unfinished tasks, policies, and development history belong here. Check Git roots and status before editing or committing. Preserve unrelated user changes.

Keep project documentation usable after cloning, without dependencies on machine-specific paths or private external workspaces.

## Development Workflow
Use `TODO.md` as the index. Bounded development work uses a conceptual document and a `.todo.md` companion in `docs/active-spikes/`. Rough exploration belongs in `docs/scratch/`; current policies in `docs/policies/`; completed or superseded spike history in `docs/archive/`. Policies describe the current approach, including rules, defaults, procedures, and useful rationale. Revise them directly; Git holds their history. Use applicable project-workflow skills when available. Do not adopt exploratory agent suggestions as requirements.

Human researchers author inquiry. Agents can help articulate, challenge, retrieve, organize, and execute work in service of that inquiry. Agent-generated documents do not by themselves demonstrate research progress. The exact product approach remains open.

## Repo-Local Skills
This repository adopts [Project Workflows](project-workflows/README.md) as a pinned Git submodule. Read [workflow.toml](project-workflows/workflow.toml), then load `project-workflows/<skill-name>/SKILL.md` before global workflow seeds. The child branch is `project/researchops-dev`; the parent branch is separate. Project instructions and existing document conventions remain authoritative. Actual project documents stay here, outside the collection.

The complete collection provides run-project-spike, commit-work, triage-project-misc, capture-for-later, draft-approval-slate, setup-project-workflows, and update-project-workflows.

Use `capture-for-later` for saved possibilities or parked subjects as small individual notes in `docs/scratch/`. Update an existing subject note rather than duplicating it. Capturing a subject does not create tasks or authorize external writes.

Honor requested review periods: when the maintainer asks to review before committing, leave changes uncommitted until that review ends or a checkpoint is explicitly requested. Do not push without authorization.

## Validation and Commits
Validate documentation links and Git boundaries after structural changes. Run checks appropriate to any implementation changes. Commit authorized, completed project work locally at a verified completion boundary. Use the commit-work skill when available, explicit paths, and no co-author trailers. Never push or create a remote without authorization.

Commit consumer changes in the submodule first, then update the outer repository's pinned commit when the change is ready. Do not silently advance the submodule to the latest remote revision.

## Privacy
Keep credentials, secrets, and local agent state out of Git. Check that any research materials included in the repository are suitable for its public audience.

## Markdown And Prose Style
Do not hard-wrap prose. Preserve paragraph boundaries and avoid reflow-only diffs. Prefer compact heading spacing in hand-authored files unless project tooling requires otherwise.

`CLAUDE.md` links to this file so the same instructions apply to both agents.

## External Reference Locations
Optional private context and reference assets live outside this public repository. Discover them through `.reference-paths.local.json` at the repository root, a gitignored JSON object mapping descriptive keys to file/directory paths. `context` identifies the external context/index; `references` identifies the reference-source root. Additional descriptive keys may identify other external locations. Use `.reference-paths.example.json` only as a generic example; actual paths belong in the local file.

Parse the file strictly as JSON data, resolve relative values from the configuration's directory, and read only locations needed for the current task. Never source/execute it or load unrelated credential-bearing `.env` files. If it is missing or a required path is inaccessible, report that specific gap and continue work that does not depend on the missing context. Pointers do not grant access or permission.

Keep private sources outside the tracked tree rather than creating nested ignored reference-material copies. Gitignore is not access control and does not untrack files or erase history. Select public-safe reasoning deliberately; private source availability does not authorize copying it into public docs or shared artifacts.

Historical `reference-material/` path mentions refer to the external `references` root. Current project work and spike docs remain in this repository; external context supports them without creating a parallel implementation spike.
