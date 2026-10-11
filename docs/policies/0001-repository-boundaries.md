# Repository Boundaries
## Current Approach
The outer `researchOps-dev` repository owns maintainer guidance, conceptual and to-do documents, current policies, scratch exploration, and archived development history. The `researchOps-hackpack/` Git submodule owns the consumer-facing template and retains its separate history and origin at https://github.com/jcklpe/researchOps-hackpack.git.

The outer repository pins a specific template commit. Commit template changes in the submodule first, then update the outer repository's gitlink when those changes are ready. Maintainer tasks and development history belong outside the consumer template.

The public maintainer repository is https://github.com/jcklpe/researchOps-dev. Creating or changing a remote, pushing, and changing visibility require user authorization.

## Rationale
People starting their research should receive a clean template. Maintainers need a separate home for reasoning and unfinished work. Separate histories and a pinned submodule preserve both purposes without including maintainer material in the consumer template.

## Documentation
Current guidance belongs in `docs/policies/` and is edited in place; Git records its evolution. Preserve only rationale that helps apply the current approach. Development exploration and historical context belong in spike, scratch, or archive documents rather than appended policy timelines.
