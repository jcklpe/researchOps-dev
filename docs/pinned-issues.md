# Pinned Issues
Unresolved development questions intentionally preserved for later, not an implementation backlog.

## Current Pins
### Research Artifact Naming and Ignore Rules
Pinned: 2026-10-11

Issue pinned: Decide how research evidence, provenance records, and any tool execution records should be named and stored, and which generated files should be ignored. A generic `logs/` folder should not be assumed to be an appropriate research structure.

Current context, updated 2026-10-13: The maintainer setup starter ignores `logs/`. Aslan questioned treating research material as logs. The [portable runbooks and setup spike](active-spikes/portable-runbooks-and-setup.md) now establishes `artifacts/` beneath trials, with session groups for interviews/user tests and trial-level survey datasets. The consumer toolkit ignores its suggested local `research/` workspace. No generic research logs folder was introduced. Broader provenance storage, tool execution records, and their ignore rules remain deferred.

Revisit when: A later spike develops evidence/provenance storage beyond the initial artifact folders or introduces a tool that produces persistent execution records. At that point, check ignore rules against the actual artifacts rather than prescribing a folder now.
