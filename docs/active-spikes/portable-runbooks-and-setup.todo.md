---
attention: live
reviewed: 2026-10-13
---
# Portable Runbooks and Mechanical Setup — Work List
## Background
See the [conceptual document](portable-runbooks-and-setup.md) for the agreed scope, design reasoning, and later clusters. Consumer implementation lives in `researchOps-hackpack/`.

## Current State
Aslan explicitly authorized implementation and local commits on 2026-10-13. The agreed slice is implemented and locally checked: project-first structure, flat templates, portable runbooks with GitHub adapters, three fictional method examples, four mechanical skills, and README entry paths. He will push the consumer repository first, then the maintainer repository that pins it, and test the published README prompt. The spike remains active until that QA and any resulting corrections are addressed; this is not a close-out.

Private source notes remain in the ignored `reference-material/` folder. No private source package, generated study, or separate demo distribution is included in this implementation.

## To Do
- Respond to the fresh-agent test results within this scope. Discuss any broader feature request separately.

## Ready for Human QA
- [ ] Walk through the fresh-clone human and agent paths, verify file outputs and links, and check that task relationships and review handoffs survived the port. Local file-copy checks passed; the independent agent run against the published repository remains pending.
- [ ] After pushing, copy the exact README setup prompt into a fresh agent and choose a new temporary destination. Verify that it clones the consumer repository, reads the local instructions, asks for a working location, and stops without creating a project/trial or inventing research content.
- [ ] Request a project, each chosen trial method, and an interview/user-test session separately. Check the files remain blank, links work, and existing-target/repeated requests prompt for a choice rather than overwriting work.
- [ ] Browse README, the three worked trials, and GitHub issue forms after publication. Confirm the copy, GitHub rendering, and practical sequence are useful for the walkthrough. Creating public issues is not required for this check.

## Local Verification — 2026-10-13
- Resolved 101 relative or upstream-toolkit Markdown links against the working tree. Checked paths used by the skills and absence of stale product-brief links, placeholder assignees, old issue-creation repository URLs, and personal filesystem paths in new consumer content.
- Parsed all eight issue forms and all four skill frontmatters with the available YAML parser; checked required form fields and distinct input IDs, skill names/descriptions, and absence of default assignees or labels.
- The skill-creator quick validator could not run because its Python environment lacks PyYAML. The direct YAML/frontmatter and reference checks above ran instead; no claim of a successful quick-validator run is made.
- Exercised the documented copies in an isolated temporary workspace: workspace setup alone, one project, all three method plans, and two session-note groups. Verified blank research prompts and the copied documents' relative links. This was a direct file-operation smoke check, not an independent agent behavior test.
- Checked all 12 example Markdown documents for fictional labeling and source-template links. Independently counted the six fictional survey rows: first routes 3 website / 2 telephone / 1 walk-in; clarity 3 yes / 2 no / 1 not sure, matching the report.
- Reviewed the portable workflow and adapters for task grouping, owners, review/revision handoffs, and session versus survey branches. Git whitespace checks passed. The final pre-commit scope check excludes ignored reference material and unrelated files.

## Done
- [x] Agree on placement and file boundaries for portable runbooks and task instructions, considering `templates/runbooks/`, and their relationship to the retained GitHub examples. Outcome, 2026-10-13: Agreed and implemented: flat documents, portable runbooks under templates, and eight GitHub adapters.
- [x] Define the mechanical setup contract: required workspace-level inputs, prepared files, naming/link substitutions, and behavior around existing work. Setup does not create a project or trial. Outcome, 2026-10-13: Implemented the workspace-only contract, chosen location, and collision handling instructions.
- [x] Refine `setup-research-repo`, including its boundary with cloning, what remains to prepare after cloning, and the instructions an agent reads first. Define the separate project/trial creation skills and agree on the walkthrough sequence. A product-creation skill is no longer part of the proposal. Outcome, 2026-10-13: Implemented four separate skills; README cloning precedes workspace setup. No product skill exists.
- [x] Map the removal of Product/Platform wrappers while preserving the project/trial templates. Identify and revise dependent product-specific brief prompts, missing product-brief links, runbook roles/labels, and README explanations; do not delete the templates inside the existing folders. Outcome, 2026-10-13: Preserved and adapted the useful source templates under templates; removed missing product-brief references and organizational wrapper assumptions.
- [x] Resolve the method-neutral treatment of the unit below Trial: whether Session remains method-specific, how survey responses/datasets fit, and the implications for artifact folders, collection tasks, and creation skills. Outcome, 2026-10-13: Resolved as artifacts with method-specific session groups, plus a trial-level survey dataset and data-collection task.
- [x] Finalize the flat document-template layout, worked-example coverage, links back to templates, and the bounded maintenance check. The old mixed-organization/problem-led pair is no longer required. Review each proposed folder README for unique content; omit `templates/README.md`. Keep creation skills pointed at blank templates. Outcome, 2026-10-13: Implemented one fictional project with three methods, source-template links, consumer maintenance guidance, and an artifact guide instead of folder READMEs.
- [x] Draft the human and agent getting-started instructions using the proposed visual badge plus adjacent fenced prompt; review the text and layout together. Outcome, 2026-10-13: Implemented the badge and adjacent prompt; exact published prompt behavior remains in human QA.
- [x] Review the proposed README framing and opening copy with Aslan; agree on treatment of authorship/origins and the changes needed to the structure and workflow explanation. The opening copy is now approved verbatim; the remaining README discussion is still open. Outcome, 2026-10-13: Applied the opening verbatim, revised the workflow diagram and rest of README; copy and usability remain in human QA.
- [x] Agree on the concrete walkthrough and expected outputs, then turn the approved requirements into file-level implementation tasks. Outcome, 2026-10-13: Implemented the agreed vertical slice. Setup stops before project creation; separate requests select each creation operation. Expected outputs are documented and checked locally.
- [x] Port the existing runbook and task instructions into the agreed Markdown structure, preserving workflow meaning and retaining the GitHub implementation examples. Outcome, 2026-10-13: Implemented eight portable definitions and matching GitHub forms, with explicit owners, review cycles, and handoffs.
- [x] Remove the Product/Platform structural layer through the agreed relocation and dependent text updates, preserving reusable project/trial content and adding no product-brief template or product-creation skill. Outcome, 2026-10-13: Implemented the project-first layout, seven flat document templates, and artifact guidance. No product brief or creation skill added.
- [x] Implement the agreed workspace-setup and separate creation skills once their individual contracts are resolved; workspace setup must not invoke creation skills automatically. Outcome, 2026-10-13: Implemented workspace, project, trial, and session skills with blank-template sources and separate operation boundaries.
- [x] Rewrite the consumer README and getting-started instructions to match the agreed framing and actual setup behavior; update the affected workflow explanation. Outcome, 2026-10-13: Implemented manual and agent entry paths, approved opening, example links, and a portable workflow diagram.

### Earlier Planning Record
These entries preserve the state of discussion when recorded. Later agreements and implementation above supersede earlier open questions.
- [x] Record the approved narrow scope in a conceptual/to-do pair and link it from `TODO.md`. Created on 2026-10-13; no consumer implementation or commits accompanied this planning pass.
- [x] Preserve the other thematic clusters as later work. They remain in the conceptual document and the development index rather than becoming additional active spikes.
- [x] Record Aslan's clarification that setup prepares the workspace only and product/project/trial creation belongs in separate skills. Recorded on 2026-10-13; no skills implemented.
- [x] Record approval of the README opening verbatim. Approved on 2026-10-13; retained in the conceptual document for later application to the consumer README.
- [x] Record that the additional mechanical creation skills belong in this spike and preserve Aslan's preference for a browsable nested template structure. Recorded on 2026-10-13; flexible placement and the actual work remaining after clone are still design questions.
- [x] Record agreement on separate templates and worked examples, with multiple examples demonstrating structural flexibility. Recorded on 2026-10-13. Browsable hierarchy remains in the examples; Aslan raised flat template storage as an alternative to the earlier nested-template proposal, and that choice is still open.
- [x] Record the later 2026-10-13 decision to remove Product/Platform as organizational units. This supersedes the product-creation and organizational-example portions of earlier entries above; they record the discussion's development, not current requirements. Source inspection confirmed that no usable product-brief template exists and the workflow diagram already starts at Project. Consumer files remain unchanged while concrete placement and terminology are discussed.

## Later Work
The [later-work clusters](portable-runbooks-and-setup.md#later-work-clusters) retain broader research content, agent assistance, integration, and provenance questions. Promote a cluster when a bounded piece of work is ready to start; link successor spikes from this pair.
