# ResearchOps — Context for Resuming After 2026-10-13
## Read This First
This is a scratch handoff, saved at Aslan's request when stopping for the night. It preserves context rather than starting another implementation phase. The [active spike](../active-spikes/portable-runbooks-and-setup.md) and [work list](../active-spikes/portable-runbooks-and-setup.todo.md) remain the owners of the current slice. The thematic scratch documents linked below contain discussion, taste, and possible later work; they are not approved specifications or active task lists.

Aslan's latest assessment was: **“okay I tested it. Seems to work kind of okay.”** He also said there is much more to do and he cannot continue tonight. A test happened. Its agent, exact prompt, environment, steps, outputs, intervention, and friction have not been supplied in this conversation. Do not convert this qualified result into full acceptance, a clean bill of health, or a specific bug report. Do not ask for a reconstruction while he is trying to stop; begin there when he returns.

## Where the Work Actually Stands
The first implementation uses Project → Trial → artifacts. Project is the largest prescribed research unit; Product and Platform wrapper folders have been removed. Interviews and user tests group material by session, while survey material can be a dataset at trial level. Seven blank document templates sit flat under `templates/`. Eight portable workflow/task definitions sit under `templates/runbooks/`. Eight GitHub issue forms remain as one implementation of those definitions.

One fictional community-support project demonstrates three trials: interview, survey, and user testing. The examples have filled documents and underlying notes or data, with source-template links. They are illustrations of arrangements and document relationships, not actual research results or a compulsory three-stage study.

Four consumer skills exist: workspace setup, project creation, trial creation, and session creation. They copy blank materials and substitute administrative names/paths. The researcher authors the questions, selects the method, and supplies substantive plans and findings. Setup stops before project creation. Separate requests create projects, trials, and interview/user-test session notes. The README has manual instructions and an adjacent badge/copyable agent prompt that clones the consumer repository before reading its instructions.

The artifact guide explains arrangements that were previously visible inside the nested template tree. No redundant folder READMEs were added. The suggested local `research/` workspace is ignored by Git; users may choose an external location with its own storage arrangements. This default is an implementation choice visible in the README, not proof that every user's version-control needs have been solved.

## Repository and Verification Snapshot
As of this capture, both repositories are on `main` and their working trees were clean before these context edits. The consumer implementation is `a15ea0a`; the maintainer implementation record is `d6b8bf3`, whose submodule pin matches that consumer commit. Each local `origin/main` tracking reference matches its respective implementation commit. This is a local observation, not a new network verification or a claim about how Aslan performed his test.

The earlier local checks covered links, YAML/frontmatter, fictional survey counts, template-source links, and direct copying into a temporary workspace. They did not execute an independent agent against the prompt. The skill-creator Python validator lacked PyYAML, so the agent used direct YAML/frontmatter/reference checks and recorded that limitation. GitHub rendering, real collision handling by an agent, and the complete user journey were not established by those checks. Aslan's later test adds qualified user feedback but does not disclose which of these surfaces it exercised.

Use the stable history handle `Spike: portable-runbooks-and-setup` when following development across later commits. Commit hashes above identify this snapshot, not a permanent substitute for the active documents.

## The Context That Must Not Be Lost
- [Direction and authorship](researchops-direction-and-authorship.md): who the toolkit serves; why Aslan wants to author it; why vague differentiation claims and artifact production do not establish its value; the origins and README framing.
- [Methods, epistemology, and evidence](research-methods-and-evidence.md): how the course and article should inform practice; the limits of earlier agent architectures; provenance and methodological questions for later work.
- [Agent assistance and tools](agent-assistance-and-tooling.md): mechanical first-slice boundaries, neutral runbooks, optional MCPs, skill/tool/platform distinctions, and the evolution of the folder decision.
- [Competitive-analysis questions](agentic-researchops-comparison.md): the comparison set already introduced, source limitations, what needs comparing, and why a feature checklist was not enough.
- [Misc intake](misc.md): the unelaborated first-test reaction, to unpack with Aslan rather than translate into invented defects.

Optional private source context is indexed under [reference-material; `references/README.md`](../../AGENTS.md#external-reference-locations). That external source set is absent from public clones. It contains a fuller conversation reconstruction, verbatim original attachments, the earlier methods exploration, a snapshot of the competitive-analysis companion, and the saved Perplexity link. Public reasoning here is intended to stand on its own. Old source links may refer to pre-refactor filenames; source snapshots are historical evidence, not current navigation instructions.

## How the Current Scope Was Reached
The work began as a larger agentic ResearchOps discussion. An earlier implementation outran the discussion, created more agent behavior than requested, prepared a demo archive, and made commits while the user still expected to settle direction. Aslan rejected that sequence and explicitly asked to undo those commits. They were undone before this approved slice. Do not treat the abandoned implementation as a source of accepted requirements.

The correction was a narrow three-part scope: portable runbooks; agents initially doing little more than copying files; and a clone/setup entry path. Further discussion deliberately changed the structural proposal. Nested blank templates initially seemed useful for GitHub browsing, but separate filled examples could supply that visual explanation. The Product wrapper turned out to encode an organizational structure rather than a necessary research relationship. An agent had proposed a product brief that did not actually exist as a usable template. Aslan identified the confabulation and used that gap to question the wrapper itself. He then explicitly removed Product and Platform from the model.

“Session” was also questioned as a universal smallest unit. The adopted solution is an artifact container plus method-specific session groups, not a new universal noun imposed on survey responses. The artifact guide earned its place because flattening the templates removed the old visual explanation of where collected materials fit.

The user approved implementation and local commits only after these discussions. The subsequent authorized implementation should not be conflated with the rejected earlier work. The current consumer commit contains the agreed narrow skills, not an autonomous start-study flow.

## When Aslan Returns
Start from his experience, not a new roadmap. Ask which parts of the test worked, where he intervened, what felt wrong, and what he wanted to happen next. If he supplies a transcript or output folder, inspect that evidence before rewriting the skills. Keep small corrections to the existing journey in the active spike when they fit its scope. Bring substantive new behavior back for discussion.

The larger brain dump is unfinished. Thematic clusters can become separate spikes once their question and intended outcome are concrete. Saving a cluster here does not authorize it, impose a sequence, or mean its work should start automatically. The current spike has not been closed or archived. The user requested context preservation for tonight, not more product implementation, another demonstration artifact, or another round of research.
