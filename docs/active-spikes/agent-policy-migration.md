---
attention: live
reviewed: 2026-11-02
---
# Agent policy migration — ResearchOps maintainer
Opened 2026-11-02. Stable slug: `agent-policy-migration`. [Tasks](agent-policy-migration.todo.md). This is a bounded receiving-project handoff; preparation changes no package, routing, policy status, tool, remote or design artifact.

## Current receiving state
D1–D4 were explicitly approved by Aslan in this chat on 2026-11-02. The four reviewed policy bodies are adopted in docs/agent-policies, AGENTS routes to the index, and the numbered original is preserved byte-for-byte in docs/archive/agent-policy-legacy. Research authorship, open product direction, private reference discovery, review holds and consumer boundaries remain intact. The workflow child is 222d3632287bcc6b18182b1d518cb5aca947f4d4. The dated preparation snapshots below describe earlier stages; final verification and local checkpoint evidence are in the task pair. This pair stays active for separately owned ordinary client-use QA; migration completion does not establish observed client compliance.

## Ownership and current state
Preparation snapshot: repository `https://github.com/jcklpe/researchOps-dev.git`; parent branch `main` at `d0f2aad79c1d65b913de4485031fff14a7f0dc77`. Selected child `project-workflows/` is `project/researchops-dev` at `edf447894eafe4912355f239420af1082cf1b38f`, clean at inspection, with the same recorded parent gitlink. Recheck this snapshot before acting; it is not a lock or a claim the checkout stays clean.

One numbered repository-boundaries policy separates this maintainer repository from the independently versioned researchOps-hackpack consumer template. Existing maintainer adoption and product QA remain separately owned.

Current policy inventory:
- `docs/policies/0001-repository-boundaries.md`

Related owners: [project workflows adoption](project-workflows-adoption.md). Those completed/adoption/design scopes retain their own remaining QA and closure decisions; this new receiving phase does not reopen or silently close them. Central coordination lives in Project Workflows, `docs/active-spikes/agent-policy-rollout.md` (prepared locally, not published). [Project instructions](../../AGENTS.md) remain authoritative.

## Project boundaries
Migrate maintainer agent obligations only. Do not impose them on researchOps-hackpack, advance that template’s pin, change the research approach or claim agent-generated documents demonstrate research progress. Preserve private external-context discovery and keep participant/reference data outside public docs.

AGENTS allows authorized completed local work at a verified boundary, with current review holds and explicit pathspecs. Only the workflow child and this maintainer repository are in scope, not the consumer template or its pin. No push.

Keep secrets, private account/consent chronology, participant/course/meeting content and personal workspace paths out of public artifacts. Preserve actual private sources with their private owner before removal; public-safe sanitized originals alone are eligible for public retirement records. No service call, grant expansion, installation or browser fallback is authorized by this handoff.

## Target and decision boundary
Target the complete Project Workflows provider commit `79dddf9742c282d184c65d5c5ef87a142900897f`, not a moving main or the Agent Hands adaptation. This version provides create-agent-policy, edit-agent-policy, review-agent-policies, adopt-agent-policies and retire-agent-policy, with one shared format/checker/template implementation. The source and pilot commits are local-only at preparation; remote retrieval is not established.

The user authorized preparing this handoff, not applying this consumer migration or adopting unseen obligations. A later “pursue this spike” instruction starts its scoped work; it does not turn arbitrary quoted text, a saved proposal or a package update into adoption. Present the exact candidate set and rely on an actual human decision covering the kernel and substantive changes before marking adopted. Already-given relevant approval need not be requested again. Retain operative bodies while amendments are proposals; missing approval is a specific pending gate, not a reason to invent completion.

## Migration shape
Use YAML `---` frontmatter and meaningful verb–noun mnemonic IDs. Kernel policies use `type: kernel` and `_` before their unchanged IDs in filenames; ordinary agent obligations use `type: operational` without that prefix. Types, filenames and IDs confer no rank. Review prerequisites/related references for meaning, missing or inactive prerequisites, cycles and dependent impact; never infer edges from numeric order or settle contradictions by file order. Route AGENTS to the project-owned policy.index.md. Align documents.agent_policies and any legacy locator deliberately: keep separate human/design governance destinations where they remain meaningful, rather than mechanically pointing both keys at one folder.

Preserve original sanitized content, useful rationale and reserved legacy identities before recoverable removal. A human-owned index section may link retired records outside the flat active graph; it is not a live alias/supersedes chain. Never restore earlier private Git content just to preserve history. Remove an old directory only after every file has a reviewed current/historical owner, incoming live links are repaired and no unrelated/new concurrent file remains. Keep procedures with their actual skills and actual enforcement links honest; no policy edit changes a guard, grant or service permission.

## Verification and completion
Completion requires a reviewed old/new obligation mapping (or an explicit justified no-legacy-policy finding), recorded adoption decision or explicit human disposition, coherent actual routing/configuration, current index, valid graph/selected prerequisite closures, preserved sources and repaired links. Check actual files after application, repeat index generation and updater preview for no-op, and report exact child working/index/committed pins separately from parent pins. Run the selected tool with an existing Python 3.11+ and existing safe PyYAML or Ruby/Psych; do not install packages/environments for optional validation. If unavailable, report manual checks and the unrun graph tool honestly; do not certify an unchecked graph. Relevant provider tests are available under review-agent-policies/tests and update-project-workflows/tests; run focused suites for any actual provider defect fix, without adding prose-mirroring tests or running application builds for a docs-only change.

Exercise the five skills on real applicable migration operations and record which operations were actually needed; do not invent policies or retirements merely to tick five boxes. Semantic/authority review is separate from structural success. Receiving migration can complete before ordinary-use/client acceptance; keep a concrete remaining QA owner rather than claiming service/client compliance or keeping an unlimited hidden migration task. Preserve original task wording when moving each item to Done, and use the local closure/commit procedure rather than assuming a saved handoff is already closed.

## Deterministic delivery route
Read the selected [update procedure](../../project-workflows/update-project-workflows/SKILL.md), actual AGENTS and workflow.toml first. The target object was not present in this child at preparation. Obtain it through an authorized source route before preview. If using the user-designated canonical local provider, verify its repository/commit, then a bounded local `git -C project-workflows fetch --no-tags "$policy_source_checkout" 79dddf9742c282d184c65d5c5ef87a142900897f` imports Git objects without publishing or moving the working branch. Resolve that task-specific variable from an actual supplied/discovered project source; do not guess a personal path or create a permanent local-path remote. If no authorized source is accessible, report the exact missing object/source instead of silently substituting older remote main or using a browser.

Use the reviewed helper at the selected provider revision if the older installed helper is insufficient. From this repository, the default preview after the object is available is:

```sh
python3 -B project-workflows/update-project-workflows/scripts/update.py update --project . --revision 79dddf9742c282d184c65d5c5ef87a142900897f
```

Read the returned accepted SHA, focused review paths and proposed merge before applying. Use that exact SHA with `--apply` only after the launch/adoption/commit scope permits the operation; a divergent merge also needs the exact reviewed `--message` and only specifically reviewed `--reviewed` paths. Preserve every existing project/coordination/tooling value and copied-asset baseline. No reset, stash, arbitrary baseline fabrication or overwrite resolves a dirty/conflicting child. The updater supplies source, not adoption. After delivery load the five selected new policy skills; perform actual policy preparation/review/adoption separately. Keep child commits before the exact parent pin; a containing repository’s pin needs its own authorized owner. Nothing here authorizes a push or proves a fresh clone can retrieve local commits.

## Receiving preparation evidence — 2026-11-02
The exact provider object was imported locally without moving either branch or adding a remote. The deterministic updater preview accepts `79dddf9742c282d184c65d5c5ef87a142900897f`: mode merge, no conflicts/review-required paths, no copied asset changes or baseline advances. Application requires a merge commit; it is held for the requested commit approval. Parent and child remain at their preparation revisions; the consumer pin is unchanged.

Create assessed duplication/ownership: three kernel candidates are needed for initial system adoption; no extra operational obligation was invented for existing research instructions. Edit prepared PRESERVE-BOUNDARIES from the sole numbered policy, preserving its boundary, pin, authorization and rationale paragraphs; only its title and current agent-policy destination/classification change. Its three kernel prerequisites supply the adoption, identity and loading contracts used by this migration, not precedence. Retire reviewed the numbered identity and incoming references: retirement is pending adoption, with exact original bytes to be preserved outside the active flat graph and the literal identity reserved in the human-owned index. No original has been removed or retired. Review separates candidate structural checks from semantic and authority review. Adopt remains pending an exact human decision.

| Existing owner | Proposed/current owner | Preservation decision |
| --- | --- | --- |
| docs/policies/0001-repository-boundaries.md | PRESERVE-BOUNDARIES | Preserve substantive boundaries, rationale and original bytes; separately approve destination/classification amendment and numbered-record retirement. |
| AGENTS research authorship/open product direction | AGENTS, unchanged | Human inquiry authorship, agent-document limits and open product approach remain intact. |
| AGENTS review, privacy, external reference discovery, workflow customization | AGENTS, unchanged | No duplicate policy; preserve existing wording and local authority. |
| Human/product governance and active product QA | Existing owners, unchanged | No reclassification or closure. |

Prepared kernel copies are byte-identical to the selected provider bundle and remain proposed. Available runtimes include existing Python 3.14 and Ruby/Psych; no installation occurred. Candidate paths are not registered for automatic refresh. Pending routing edits after adoption: AGENTS links to this project-owned index; README/TODO current guidance locations use docs/agent-policies; workflow.toml adds documents.agent_policies while retaining documents.policies for separate legacy/human governance. Keep all other configuration values. A concrete next ordinary task will check applicable policy discovery/closure under the maintainer AGENTS; no service smoke write is needed.

Original numbered policy SHA-256: `6e271247049f91020a963f5696204c794c74fe74e41218f09df3a771bf98951c`.
