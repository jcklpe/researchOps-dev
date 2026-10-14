# Agent Assistance and Tooling — Scratch Context
## Status and Immediate Boundary
Captured 2026-10-13. The implemented first slice is mechanical setup. This document preserves possible later behavior and architectural questions without authorizing them. The [active spike](../active-spikes/portable-runbooks-and-setup.md) describes what actually exists.

“Agentic refactor” means both help for HackPack users doing research and help for maintainers developing the toolkit. The two surfaces need different instructions. Maintainer spike/commit skills belong in the development repository; consumer setup skills belong in the downloadable HackPack. Do not copy the maintainer's unfinished project history into a user's research workspace.

## What the Four Skills Actually Do
- `setup-research-repo` starts with an available checkout, orients the user, establishes their selected working location, and stops. The README prompt handles cloning before it loads the skill.
- `create-research-project` copies one blank project brief into a chosen project folder.
- `create-research-trial` copies one blank trial brief, a plan for the human-selected method, and a blank report, and prepares an artifact directory.
- `create-research-session` prepares one interview/user-test session's blank notes, including distinct observer files when requested. It does not turn a survey response into a session.

Names and paths are administrative inputs. The researcher supplies the inquiry, method choice, recruitment approach, questions/tasks, interpretations, and findings. The code-free skill folders carry their own instructions and relative references; a clone does not depend on the maintainer's global skills. They are readable workflow documents, not installed software or proof that a particular agent will obey them.

The current README prompt explicitly asks for a clone destination if missing, reads local instructions, asks for the research working location, and stops before creating a project. The user had rejected treating “get started” as permission to generate a study plan. A one-click visual affordance was discussed, then deliberately simplified to a badge as a marker plus a visible fenced prompt. No agent-launch mechanism is promised.

## Neutral Runbooks, Optional Destinations
Aslan wanted the GitHub issue-template runbooks made neutral so users could adapt them to their working context. Three things must survive that move: which tasks exist and how they relate; what each task asks for and how completion is assessed; and the review/responsibility handoffs. A board column such as “In Review” is one tool's representation of a review request, not the research action itself.

Markdown remains the low-power source format for templates. It does not mean teams must manage live tasks in Markdown, or that a Google Docs/Microsoft 365 workflow is a failed adoption. The files can be read, copied, or adapted into an existing document/tracker environment. Actual owners and status should live in the chosen destination, rather than accidentally becoming two inconsistent tracking systems.

The earlier source discussion made a useful distinction: a neutral runbook is not a universal adapter engine. A human and capable agent may instantiate the instructions for a selected environment without a deterministic abstraction covering every service. The current GitHub forms remain an implementation example. No auto-transfer into other trackers was built in the first slice.

## Optional MCPs and Custom Tools
Aslan first considered bundling CLI tools or connectors, informed by his experience building agent-accessible command-line tooling. He later suggested assuming optional MCP-based access where appropriate, rather than rebuilding capabilities already available that way. This is a direction to evaluate, not a selected MCP dependency, a mandate for every user, or permission to connect external accounts.

The principle of least power orders the options: readable instructions and ordinary files should be useful on their own; stronger tools should earn their place and be opt-in. That does not ban building real tools. It requires identifying useful work a tool performs beyond what a template or skill already supplies.

A later integration discussion should distinguish:
- A skill's procedure and decision boundaries.
- The templates or schemas it reads and produces.
- A connector's actual read/write capabilities and permissions.
- The destination system's ownership of tasks, status, and artifacts.
- What still works without that connector or without CLI access.

Candidate environments mentioned include GitHub, Jira, Trello, Asana, Odoo, Google Drive/Docs, Microsoft 365, Nextcloud, and local files. Mention is not support. No provider or integration roadmap has been selected. A useful integration could reuse a research service rather than recreate recruitment databases, scheduling, incentives, or evidence hosting.

There is also an unresolved packaging boundary among HackPack-specific tools, generally reusable agent/terminal tools, and the maintainer's personal environment. Portability means a new user should not need the maintainer's private setup. The maintainer may want convenient reuse locally, but no additional submodule/package arrangement is adopted for that purpose.

## Structure: The Design Evolution Matters
The original nested folders let someone browse a hierarchy in GitHub and understand where a template would be used. Aslan wanted to preserve that benefit. Early options kept nested blank templates or offered multiple organizational layouts. The later decision separated flat blank templates from filled examples, making the distinction between copying material and learning from it more explicit.

Removing Product/Platform solved much of the earlier complexity. Projects can span products and services without requiring wrapper folders or alternate organization-chart examples. The consumer model is now project-first; a product can still be the subject of a brief. Do not restore a product-creation skill just because the source framework once had that level.

`artifacts/` avoids forcing one smallest-unit noun on every method. Session groups still make sense for interviews and user tests because several artifacts may concern the same encounter. A survey export can cover a response window. The artifact guide explains this arrangement after the blank templates lost their nested teaching structure.

Examples carry their own drift risk. The chosen mitigation is source-template links and checking affected examples, runbooks, skills, and GitHub forms together when their source changes. This is a maintenance practice, not a guarantee of consistency or permission to build a large generation/validation framework. Templates remain adaptable prompts; example files need not mechanically reproduce every heading.

## Further Assistance Is Still Open
The earlier source conversation suggested planning, methodology review, recruitment planning, session processing, synthesis, evidence-chain review, report assembly, and close-out skills. These are exploratory proposals. The rejected early demo also contained broader start/prepare-study behavior. Neither list is the next implementation backlog.

Potentially useful future assistance might retrieve approved context, flag contradictions, preserve disagreement, check references, show missing information, or help carry decisions into operational tasks. Each proposal needs a concrete user situation, a clear boundary on judgment, necessary tools, and an observable benefit. “The agent can generate it” is insufficient justification.

## What to Learn From the Test
The latest user report is only that it worked “kind of okay.” On resumption, inspect actual friction before adding capability. Distinguish missing information, too many setup turns, unclear workspace location, repeated prompts, blank-template quality, and agent overreach if the evidence points to any of them. These are categories for asking about the experience, not bugs observed in the test.

A successful mechanical operation and a useful research workflow are different outcomes. The first implementation is a place to learn what help the researcher needs next; it does not settle the long-term architecture.
