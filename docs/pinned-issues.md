# Pinned Issues
Unresolved development questions intentionally preserved for later, not an implementation backlog.

## Current Pins
### Research Artifact Naming and Ignore Rules
Pinned: 2026-10-11

Issue pinned: Decide how research evidence, provenance records, and any tool execution records should be named and stored, and which generated files should be ignored. A generic `logs/` folder should not be assumed to be an appropriate research structure.

Current context: The setup starter ignores `logs/`. Aslan questioned treating research material as logs and deferred this choice. No logs folder or new research-storage structure has been introduced.

Revisit when: The refactor defines its evidence/provenance structure or introduces a tool that produces persistent execution records. At that point, check ignore rules against the actual artifacts rather than prescribing a folder now.
