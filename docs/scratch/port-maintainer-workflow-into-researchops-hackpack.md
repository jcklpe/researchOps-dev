---
status: parked
---
# Port maintainer process and docs into ResearchOps HackPack
Captured 2026-11-01 from the maintainer’s discussion of package versus template repositories. This is a potential future spike; ResearchOps remains parked and no migration is authorized by this note.

## Question and reasoning
Should ResearchOps HackPack be treated primarily as a reusable skills-and-tools package, with its own development records, rather than as a template repository that someone clones and turns into their working research project?

The existing split keeps maintainer process and documentation in `researchOps-dev`, with consumer material in the `researchOps-hackpack` submodule. Its rationale is a clean consumer template. Project Workflows and Wireframe Workflows instead distribute reusable capabilities while retaining documentation for their own development in the same repositories. As ResearchOps becomes more agentic and skills-centric, that package model may fit it better too.

A package can contain templates. The useful distinction is whether users transform the checkout into their own workspace or consume capabilities and copy selected templates into a separate workspace. Keeping actual research and participant data separate remains necessary in either arrangement; moving maintainer docs into the toolkit would not make the public package a research-data destination.

The current setup already offers skills that prepare a separate research workspace. That makes the package approach plausible, but does not settle distribution, maintenance, installation or migration choices. DesignOps is trying the package approach independently; its choice is not automatic authority for ResearchOps.

## Scope of a future spike
If this direction is resumed and chosen, investigate porting the maintainer process and suitable documentation from `researchOps-dev` into `researchOps-hackpack`: agent instructions, development entrypoints, spike/task records, relevant policies, scratch and archive material, and the development index. Preserve provenance and useful history, repair links, and make the distinction between toolkit use and toolkit maintenance explicit. Do not copy private references or local configuration into public toolkit content.

Decide separately how Project Workflows is supplied. A pinned development dependency, global-only maintenance procedures, and the package’s consumer skills solve different needs. A package approach does not automatically require removing the existing workflow dependency or adding one to every consumer project.

## Questions to resolve on pickup
- Is the checkout a reusable dependency, a template for a new research repository, or a package supporting both entrypoints? What should setup create, and where should actual research live?
- Which maintainer records belong in the package, which are private or external, and which should stay as historical records with navigable source references?
- How will instructions keep consumer agents focused on the requested operation without treating development proposals as adopted research procedures?
- Should the Project Workflows adoption move with the development process, and how would its project root, branch and references change?
- How should Git provenance, remote links and existing clones be preserved if the outer repository is eventually retired? Do not assume that copying files preserves their full history.
- Can installation or selected-folder distribution keep consumer use light without requiring a separate maintainer repository?

## Existing context
- [Repository boundaries](../policies/0001-repository-boundaries.md): current policy remains authoritative until a migration is approved.
- [Agent assistance and tooling](agent-assistance-and-tooling.md): existing consumer/maintainer and portability questions.
- [Current HackPack entrypoint](../../researchOps-hackpack/README.md): inspect its actual setup behavior when resuming.
- [Project Workflows adoption](../active-spikes/project-workflows-adoption.md): current maintenance workflow arrangement.
