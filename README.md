# ResearchOps Development
Maintainer workspace for developing the ResearchOps HackPack. The consumer-facing template lives in the `researchOps-hackpack/` Git submodule; development reasoning, policies, and history belong in this outer repository.

## Start Here
Read `AGENTS.md` and `TODO.md`. The submodule is pinned to a specific HackPack commit. On a future clone, initialize it with `git submodule update --init --recursive`.

Work inside `researchOps-hackpack/` when changing the consumer template. Commit its changes there first, then record the new submodule commit in this repository. Maintainer documentation should stay outside the submodule.

## Project Direction
The intended users are individuals and teams organizing product, UX, and service-design research, including people with constrained tools or no terminal access. Assistance should augment human-authored inquiry, beginning with tedious setup and coordination. Markdown follows the principle of least power; integrations and stronger tools should be optional. Research provenance matters.

The maintainer wants to develop an authored toolkit and learn through building it. Competitive analysis should inform substantive choices rather than establish uniqueness by assertion. Researcher purpose and judgment remain central. The first slice now supplies project/trial/artifact organization, interview/survey/user-testing examples, portable runbooks, and mechanical agent setup. Its [active spike](docs/active-spikes/portable-runbooks-and-setup.md) retains the reasoning and pending human QA. Broader methodological content, further agent assistance, and integrations remain open.

## Development Documentation
The maintainer workflows are adopted under `project-workflows/`; see `AGENTS.md` for local authority. Use conceptual and to-do document pairs under `docs/active-spikes/` for bounded development work; `TODO.md` is the short index. Keep rough ideas in `docs/scratch/`, current agent obligations in `docs/agent-policies/`, and completed development history in `docs/archive/`.

The public GitHub repository is [jcklpe/researchOps-dev](https://github.com/jcklpe/researchOps-dev), configured as `origin`.

## License
This maintainer repository is licensed under the GNU Affero General Public License, version 3 (`AGPL-3.0-only`). See [LICENSE](LICENSE). The HackPack submodule is a separate repository; this license notice applies to the maintainer repository.

## Optional External Context
Read [External Reference Locations](AGENTS.md#external-reference-locations) for local paths-only configuration and missing-context behavior. Project work and its spike records stay in this repository; external context and reference sources retain their own purpose and authority.

## Project Workflows adoption
The unchanged shared collection lives in `project-workflows/` at an exact detached pin, with project settings in [docs/workflow.toml](docs/workflow.toml). Use its [update procedure](project-workflows/update-project-workflows/SKILL.md) for reconciliation, with project rules in [AGENTS.md](AGENTS.md). Initialize the recorded workflow revision with `git submodule update --init -- project-workflows`; client discovery and service access are separate checks. [Reconciliation and validation](docs/active-spikes/project-workflows-adoption.md) · [remaining steps](docs/active-spikes/project-workflows-adoption.todo.md).

For local collaborator setup, use the adopted [Get started guidance](project-workflows/README.md#get-started). Start contribution work with [Coordinate Project Contribution](project-workflows/coordinate-project-contribution/SKILL.md); each agent keeps its own spike and follows this project’s existing scope and review rules.
