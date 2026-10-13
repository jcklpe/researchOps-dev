---
attention: live
reviewed: 2026-10-13
---
# Portable Runbooks and Mechanical Setup
## Purpose and Current Agreement
Make the existing HackPack easy to obtain and begin using, with a small, demonstrable path from cloning the consumer repository to having research templates ready for a person to fill in. Build additively on its existing folders, templates, and workflow.

Aslan approved the scope, then the concrete structure and implementation on 2026-10-13, explicitly authorizing implementation and local commits. He will push and test the published README prompt himself. The agreed slice is implemented and locally checked; the spike remains active for that human QA. See the [work list](portable-runbooks-and-setup.todo.md).

The immediate use case is an Open Austin walkthrough of getting started. The walkthrough should demonstrate obtaining the actual HackPack repository and preparing a workspace. A generated study plan, new distribution package, or comprehensive redesign is not needed to demonstrate that result.

## Implemented Contracts — 2026-10-13
The shared model is Project → Trial → artifacts. `session-01/` groups an interview or user test's materials; a survey keeps its dataset at trial level. Project is the largest prescribed unit. Blank document templates are flat under `templates/`; portable runbooks and their tasks live under `templates/runbooks/`. One fictional community-support project demonstrates interview, survey, and user-testing trials under `examples/`, with each example document linked to its template.

| Operation | Inputs from the researcher | Mechanical output |
| --- | --- | --- |
| `setup-research-repo` | Available checkout and chosen working location | Orientation and an empty working directory if needed; no project |
| `create-research-project` | Workspace and project name | Project folder and blank project brief; no trial |
| `create-research-trial` | Existing project, trial name, selected method | Trial brief, selected method plan, report, and empty `artifacts/`; no session |
| `create-research-session` | Interview/user-test trial and session identifier; optional observer identifiers | Session folder and blank notes, with separate files when multiple observers are supplied |

The README prompt clones the consumer repository before loading the workspace skill. It asks for a destination when missing and stops after setup. All four skills ask about collisions instead of overwriting existing work. They leave research questions, method selection, plans, and findings to the researcher. The suggested `research/` working folder is ignored in the toolkit; another chosen location retains its own version-control arrangements. No integrations or runtime packages are required for file copying.

The root README contains the approved opening, manual setup, a visual badge with an adjacent copyable prompt, skill examples, the folder explanation, and the workflow. `guides/research-artifacts.md` carries the useful guidance previously embedded in the session-artifacts README and explains the now method-neutral placement. No additional folder READMEs were created. The GitHub forms adapt the same portable workflow without fixed assignees, required labels, board columns, or issue-creation URLs into someone else's repository.

Earlier questions and alternatives below explain how these contracts developed. Where a question is marked resolved, the implemented contracts and linked consumer files supply the current behavior. The proposed broader agentic demo, generated study content, and separate distribution package are not part of this implementation.

## Agreed Scope
### 1. Portable Runbooks
Express the existing GitHub runbook and task-template instructions in ordinary Markdown so someone can adapt the workflow to their chosen context. Keep the GitHub issue templates as an implementation example.

Preserve what the workflow means: which tasks to create, how they relate, each task's instructions and completion criteria, and the review and responsibility handoffs. Describe actions independently of a particular board or issue system. For example, requesting team review should survive even when moving a GitHub card to a named column does not apply.

The existing [issue templates](../../researchOps-hackpack/.github/ISSUE_TEMPLATE/) are the starting material: project runbook, epic, project brief, trial runbook, trial brief and plan, recruitment and scheduling, research sessions, and synthesis and report. Preserve their useful workflow while removing product-organization assumptions where they occur. The agreed change to a project-first structure requires bounded changes to the project/trial prompts as well as folder placement; broader methodological revisions remain separate.

Markdown supplies a readable, adaptable definition. It does not require a team to keep its live assignments or project status in Markdown. This slice also does not promise automatic transfer into every tracker.

Aslan approved placing portable runbooks under `templates/runbooks/`, with task definitions beneath that and the document templates flat at `templates/`. This distinguishes instructions for writing/reviewing a brief from the blank brief itself without imposing an organizational hierarchy. The portable definitions own the workflow; the GitHub forms adapt it. Consumer agent instructions require checking affected forms, skills, and examples when templates or workflows change.

### 2. Mechanical Setup
Initially, agent assistance prepares the files and folders that the researcher will fill in manually. It can ask practical setup questions such as names and destinations. The researcher supplies the inquiry and substantive research content.

Aslan suggested a skill named `setup-research-repo` and clarified its boundary: it prepares the overall research workspace only. Creating a project, trial, or method-specific collection unit belongs in separate operations. Setup must not create the first instance automatically. The creation skills belong in this spike too; their implemented contracts are listed above. The proposed product-creation skill is withdrawn following the decision to remove Product and Platform as structural units. Session creation is method-specific, not a survey-response operation. The existing maintainer skills in the outer repository serve a different audience.

The source checkout contained the old product/project/trial/session-artifacts tree with templates in place. Aslan values being able to explore actual examples in GitHub and see how the research fits together. The agreed direction removes the Product/Platform wrapper while retaining useful project/trial material. Identify an actual initialization or orientation need before inventing setup work merely to justify a skill.

Questions considered before writing the skills, now resolved by the contracts above:
- Is cloning part of this skill, or does the getting-started instruction clone the kit and then invoke it?
- What does workspace setup need to do after cloning, given that the example folders and templates already exist?
- Which workspace-level files need preparation, which example material stays as reference, and which names or links need substitution?
- How does setup behave when the destination already contains research work or setup is run again?
- What does the agent show the researcher at the end so they can choose the appropriate next operation?
- What does each separate project/trial creation skill copy, and what method-specific operation belongs below a trial? Keep their initial behavior mechanical, with research content left for the researcher. Copying an entire nested example branch must not silently create real child trials or sessions that the researcher has not requested.

The portable runbooks may describe an entire research workflow. The setup skill's ability to read them does not give it responsibility for performing that workflow. Drafting research questions, selecting methods, generating plans, conducting research, and producing findings are outside this initial agent role.

#### Projects as the Top-Level Research Unit — Agreed 2026-10-13
Aslan decided to remove the Product/Platform hierarchy from the HackPack's model. Project is the largest prescribed research unit. Product teams, Platform teams, cross-service work, and academic HCI research can all organize projects without the toolkit encoding their organization chart or requiring a product. Products and services can still be subjects or context described in a project brief; they no longer need dedicated wrapper folders, templates, or creation skills.

This supersedes the earlier proposals to preserve a product-first template tree, make its levels optional, or illustrate separate product-organized and project-organized layouts. Those alternatives tried to preserve browsability and accommodate heterogeneous teams. Aslan's correction identified a simpler route: retain browsable worked examples of research, and remove the organizational wrapper itself. The earlier private adaptation had already demonstrated project → trial → sessions without a required product.

Inspection of the pre-change source on 2026-10-13 confirmed that its README's workflow diagram started at Project and had no Product step. Its product folder contained only a README headed "Product Brief" followed by a one-sentence definition; there was no usable product-brief template or issue template. The agent's proposed `product-brief.md` and product-creation skill filled an unverified gap instead of questioning whether Product belonged in the model. Those additions are withdrawn.

The source project and trial briefs also assumed products: their background asked about a product, both linked to a missing product brief, and outcome/hypothesis prompts presupposed product development. The implementation revises those passages around the research problem, context, and intended use of learning, and generalizes product-specific roles and labels while retaining review handoffs. This required more than moving folders, without expanding into a wholesale research-method rewrite.

The useful project/trial templates have been adapted and relocated. Removing the organizational wrapper preserved their purpose rather than deleting the research templates inside it. The remaining placement and method distinctions were subsequently agreed and implemented as described above.

#### The Unit Below a Trial — Resolved 2026-10-13
Aslan questioned "Session" as a universal term because it fits interviews more naturally than surveys. He subsequently approved `artifacts/` as the neutral container and `session-01/` for grouping materials from an interview or user-test encounter. The workflow task is now data collection.

An interview can have sessions and field notes; a survey can retain responses as a dataset without requiring one folder per response. Data collection names a workflow responsibility rather than treating a session and a survey response as equivalent units. Aslan's later approval of the three-method vertical slice includes a blank survey plan and a fictional filled example. Its questions are teaching examples, never the source for a real trial's inquiry.

#### Blank Templates and Worked Examples — Layout Agreed 2026-10-13
Aslan agreed to separate blank `templates/` from fictional worked `examples/`, with examples linking back to their source templates. Flat document templates are the adopted layout. Following removal of the Product/Platform hierarchy, separate mixed-organization and problem-led demonstration workspaces are no longer needed. Worked examples still matter because they show completed documents and their relationships. The agreed coverage is an interview, survey, and user-testing trial. A fictional community-support scenario implements that coverage; the earlier plural-workspace requirement is superseded.

The agent initially recommended preserving the nested template tree to retain a visual explanation. With multiple worked examples providing that explanation, the current agent recommendation is a flat set of clearly named reusable documents, plus nested examples showing different valid arrangements. This avoids presenting one product-first ancestry as the apparent rule for copying. The tradeoff is that the blank files alone no longer show the full arrangement; links to examples and the runbooks must supply that context. Aslan resolved the tradeoff in favor of flat templates, nested worked examples, and a short artifact guide.

Most of the existing tree supplies template material, but its repeated `README.md` filenames and mixed explanatory/example content need deliberate mapping when flattened. Aslan challenged adding folder-root READMEs by default, particularly `templates/README.md`. The agent withdraws that proposed file: the folder name and root introduction can supply its basic orientation. Retain or create another README only for concrete, nonduplicative content that belongs there; existing useful explanatory material should be deliberately integrated rather than lost during moves. Product-specific prompts do require the bounded revision described above.

The creation skills copy from templates. Examples explain how the resulting documents and folders work together and are labeled fictional, including when an individual file is encountered separately. Real research lives in the researcher's chosen destination. The researcher chooses the destination inside or outside the clone; neither templates nor fictional examples become active research by default.

Maintenance practice implemented in consumer agent instructions:
- Link each example document to the template it illustrates; an example's overview can link to the relevant workflow.
- When a template or workflow changes, inspect the examples that depend on it and update affected guidance, structure, and links as part of that change. Conversely, notice when improving an example reveals a needed template correction; propose that correction rather than silently expanding the template.
- Keep blank templates as the copying source so sample answers do not enter new research documents.
- Review examples for useful, intentional adaptation rather than requiring every heading or field to be identical. Templates remain prompts that people can adapt.

Skills and maintainer instructions can make this dependency check part of the workflow; they cannot guarantee that drift will never occur. Link checks can catch broken references, while whether an example still teaches the intended practice needs content review. No new generation system, schema, or validation tool is proposed as a prerequisite.

Earlier example proposals expanded from one worked project to several organizational arrangements to demonstrate flexibility. That rationale is superseded by removing the organizational hierarchy from the model. Select examples for the research process and document relationships they teach, with enough coherent fictional content to be useful. Product, platform, service, or academic context can appear in a brief without demanding a separate structural pattern. The three-method coverage is now agreed and implemented in the fictional community-support project.

### 3. Getting Started and README
Provide human-facing instructions for obtaining and using the consumer HackPack, plus instructions someone can give their local coding agent to obtain it and perform the agreed setup. A person should be able to start by cloning the consumer repository directly; they do not need the maintainer repository or its submodule arrangement.

Aslan approved a Shields.io badge used as a visual marker, followed directly by a fenced prompt that someone can copy to their agent. The prompt is visible in the README without requiring navigation to another instruction page. [Shields.io documents static badges](https://shields.io/docs/static-badges). This layout needs no agent-launch mechanism; the person supplies the prompt to their chosen agent. The text is implemented in the consumer README and awaits Aslan's test of the published prompt.

The README rewrite belongs to this same entry path. Its opening should explain the toolkit's usefulness and Aslan's authorship clearly. Aslan describes the structure as a combination of practices encountered and adapted during years of federal government contracting and his own ways of organizing research. He does not want the introduction to read like a lightly modified copy of another organization's system, and no longer wants to foreground an individual thank-you there. He approved the opening below verbatim on 2026-10-13. Any separate treatment of origins remains to be discussed.

The existing purpose paragraphs contain useful intentions: helping teams coordinate, making responsibilities and review understandable, and giving stakeholders visibility. Their emphasis on GitHub project management needs to change. They also blur the reusable toolkit's README with a particular team's operational handbook. Proposed framing: explain what the kit supplies and how a team can adapt it, while leaving that team's actual roles, policies, and tools for the team to establish.

#### Approved Opening Copy — 2026-10-13
> ResearchOps HackPack is a practical toolkit for organizing product, UX, and service-design research. It provides reusable templates and runbooks for setting up projects, coordinating the work, and keeping research materials organized.
>
> I developed it through years of work in federal government contracting, bringing together practices I used and adapted there with my own approaches to organizing research. The toolkit gives individuals and teams a starting structure they can adapt to their tools and ways of working.

The approved opening is now applied verbatim. The rest of the README connects it to the folder structure, human and agent setup paths, and portable workflow. The revised diagram describes research actions and review handoffs without requiring GitHub issues or a specific document store.

## Why This Boundary Matters
The broader audience includes individuals and teams establishing research operations from scratch or joining existing practices, with widely different control over their computers and tools. Markdown and folders provide a modest starting point that people can inspect and adapt. Agent assistance should lower the setup burden without making research authorship depend on an agent generating documents.

This first slice builds on the existing project/trial documents and workflow, with the agreed removal of organizational wrappers. Broader conceptual work can improve it later, but settling an ontology, rewriting every research template, or building integrations would delay learning whether this basic entry path is useful. The larger goal remains a practical tool for doing research; academic material and Aslan's epistemological work inform that purpose without becoming specifications for the whole product.

## Acceptance Check — Local Checks Complete, Human Test Pending
Starting from a fresh copy of the consumer repository, walk through both the human instructions and the agent-assisted path. The researcher should be able to locate the templates, prepare the overall workspace, and identify the appropriate next operation. Verify that workspace setup does not create a user-specific project or trial. Any demonstration of those operations should invoke their separate skills explicitly. Verify the concrete outputs against the implemented contracts above.

Check that the portable runbooks preserve the existing task relationships, review steps, and handoffs, that the GitHub examples are still available, and that the basic path does not depend on configuring a tracker integration. Check that the setup agent leaves research content for the researcher. The work list records the checks actually run. Direct copying checks verify file arrangement, source templates, and links; they are not evidence that an independent agent follows the published prompt or handles every collision correctly. Aslan will push and run that test.

## Later Work Clusters
These are deferred discussion areas, not active spikes or implementation commitments. Give a cluster its own spike when its question and outcome are clear enough to work on independently.

| Cluster | Material to retain for later | Relationship to this slice |
| --- | --- | --- |
| Research framework and template content | UX Epistemology, plain-language integration of research-methods terminology and rigor, interview/questionnaire differences, and broader changes to the hierarchy or templates. | Can build on the existing content after the entry path is usable. Removal of the Product/Platform layer, affected prompts, and the session/artifact terminology decision are in this spike because they affect the mechanical skills and portable workflow. |
| Further agent assistance | Which additional work an agent should support, where human authorship and judgment sit, and competitive analysis of actual mechanisms and structures. | Starts from experience with mechanical setup; it must not inherit permission to generate inquiry from this spike. |
| Optional integrations and operational tools | Adapting to chosen trackers and document systems, potentially using optional MCP connections before building custom tools. | Portable workflow descriptions make later adapters possible; no MCP dependency or integration is selected here. |
| Research evidence and provenance | Preservation of originals, recordings, transcripts, and relationships to later interpretations; artifact naming and storage. | Keep the existing [pinned storage question](../pinned-issues.md) visible without redesigning storage during setup work. |

## Reference Material
The [earlier methods exploration](../../reference-material/researchops-hackpack-methods-spike.md) is optional local context in the Git-ignored `reference-material/` folder and will be absent from a public clone. It contains mixed human discussion and agent proposals, not an adopted specification. The reasoning needed for this spike is recorded above; following that reference is not required to implement an agreed requirement.

Aslan permits use of his unfinished UX Epistemology writing in this project. If later work needs a copy, select and place it deliberately rather than exposing unrelated workspace links. This spike has not copied that article or promoted the older exploration wholesale.
