# Research Methods, Epistemology, and Evidence — Scratch Context
## Status
Captured 2026-10-13 as candidate material for later work. The first slice adds practical method-specific plans and examples, but the broader research framework is not settled. The earlier methods note contains extensive agent-generated architecture. Its existence and level of detail do not make that architecture an adopted requirement.

## How These Inputs Relate
Aslan's UX Epistemology writing grew out of the original ResearchOps work. While trying to develop more templates and describe methods, he found the qualitative/quantitative and synthesis/analysis distinctions insufficient as the fundamental way to organize everything. That led him to develop a personal account of how research and interpretation work. The HackPack is an opportunity to make that viewpoint useful in practice.

The Quant Methods course supplies further vocabulary, distinctions, rigor, and references. It should help refine both the writing and the toolkit. It is reference material across the course, not a specification or a transformation pipeline in which class concepts must become fields in every template. An earlier agent presented a strong sequence from Quant Methods through UX Epistemology into HackPack; Aslan's later clarification limits that reading. Practice, theory, and formal methods can inform one another without one fully determining the other.

Aslan does not want a jargon-heavy academic framework or an epistemological manifesto. He also does not want merely personal terminology disconnected from existing research practice. The practical challenge is to make precision useful in ordinary work: explain what a choice means, what it supports, and why it matters, using formal terms and citations where they help.

His unfinished UX Epistemology article may be used publicly with his permission; unfinished does not mean private. It has not been copied into this repo as part of the current slice. If a future spike needs it, bring in the intended text or a suitable public reference deliberately, preserving the distinction between an unfinished author draft and a settled specification.

Peng Jiang's SurveyMonkey presentation was mentioned as possible comparison or inspiration. No structural influence from it has been established. Do not let its proximity to the course discussion make its architecture a requirement.

## Earlier Candidate Distinctions to Revisit
The earlier exploration proposed the following distinctions. This table preserves them as questions to evaluate, not a required ten-part schema or a queue of fields to add.

| Candidate distinction | Practical question it might clarify | Risk if imposed mechanically |
| --- | --- | --- |
| Research problem / inquiry aim | What is the person trying to understand, and why? | An agent manufactures a purpose to fill a brief |
| Unit and scope of inference | Who or what does an observation concern, and to what can a claim apply? | Formal terminology becomes a compulsory field without affecting interpretation |
| Research design / method | What arrangement could address the question? | A fixed menu chooses a method before the inquiry is understood |
| Sampling and recruitment | Why these participants or cases, and what does their selection leave out? | Scheduling a target number is mistaken for an adequate sampling argument |
| Constructs / measurement / operationalization | What exactly does a recorded quantity or category stand for? | A convenient measurement is treated as the whole thing of interest |
| Procedure / instrument / technique | What produced the material, using which version and conditions? | Distinct levels are collapsed into an ambiguous “method” label |
| Data / phenomena / evidence | What was recorded, what pattern is being described, and how is it used to support a claim? | A generated summary silently becomes the primary evidence |
| Analysis / synthesis / sensemaking | What transformations and interpretive work connect materials to conclusions? | A taxonomy dictates every inquiry's sequence |
| Inference / claim type | What kind of conclusion is being drawn and what supports that move? | Source links or confidence scores substitute for reasoning |
| Quality / uncertainty / error | What could lead the team to the wrong conclusion? | A checklist creates an appearance of rigor without changing decisions |

Qualitative/quantitative distinctions may still describe aspects of a study. The concern is with treating them as exhaustive mutually exclusive buckets for the whole process. Likewise, “analysis” and “synthesis” should not become catch-all labels that hide different methods or inference steps. The precise replacement vocabulary remains for Aslan to work through.

## Plain-Language Guidance and Formal References
An earlier candidate was a practitioner layer with questions such as “Why these participants?” and a reference layer connecting them to formal concepts and citations. This remains a useful possible design to evaluate rather than a decided requirement for two new directories, metadata schemas, or parallel documentation systems.

The course exploration mentioned Balnaves and Caputi, Kuehl, Haig, statistical inference, reproducibility, validity, reliability, operational definitions, and sampling. Those are leads for selective integration. Detailed interpretation, citation accuracy, and suitability for a specific template still need source work. This context-capture pass has not re-read the course materials or verified new academic claims.

Haig's data → phenomena → theory distinction and the phrase “evidence provides friction rather than foundations” appeared in the earlier agent's interpretation of the epistemology connection. Preserve them as interpretive leads with that provenance, not as quotations from Aslan's article or an already accepted reporting schema.

## Evidence and Preservation
Aslan's preference was **“As much as possible should survive. We want provenance. We want original recordings, transcripts etc etc, all this should be recoverable.”** He noted that this overlaps with separate work on an agentic wiki. The overlap is an intellectual connection, not a dependency this toolkit must import.

The current artifact guide addresses a small part of that preference: source materials, observer authorship, session groups, datasets, external references, and relationships to reports. It does not implement a provenance graph, retention system, large-file store, access-control system, or recovery service. A link to an external original is a route to the material, not preservation of the material itself.

An earlier institutional recording-deletion practice was raised during discussion; Aslan rejected treating that institution's procedure as binding here. Do not silently install a universal retention policy from a comparator. Storage and handling still need to fit the actual project's audience and arrangements; that is different from claiming every user inherits one institution's rules.

Potential questions for later evidence work include how to retain originals alongside transformations, preserve questionnaire/protocol versions, represent researcher disagreements, make omitted or contrary evidence visible, and keep claims traceable when materials live in several tools. “Keep everything” should not be flattened into “commit every file to a public repository.”

## Human Evidence and Agent Contributions
The source discussion distinguished human observations/materials, agent-derived summaries or candidate interpretations, and human judgments/decisions. These are candidate provenance distinctions worth considering. They are not yet a database model or mandatory frontmatter vocabulary.

Aslan strongly agreed that if researchers interpret the same session differently, an assistant should not automatically blend them into one authoritative summary. Later synthesis assistance would need to stay grounded in human artifacts, observations, and decisions. That concern reaches beyond showing a source citation at the bottom of generated prose: who made an interpretation and which alternatives were retained also matter.

This does not settle every future delegation question. For example, skepticism of agent-generated inquiry alone does not establish a universal prohibition on all automated moderation. Those would be substantive discussions if they become relevant; the current skills do no interviewing or synthesis.

## Current Files and Candidate Work
The project/trial briefs, three plan templates, report, field notes, and artifact guide are the concrete places later work could affect. `synthesis-methods.md` was deliberately left unchanged in the first slice; the original conversation identified its mixing of methods and synthesis techniques as a question to revisit, not a change already completed.

A data-visualization reference section was also parked in the earlier exploration. Its scope and connection to the initial setup remain open. Do not add visualization tooling or a new reference taxonomy just because the note exists.

A methods spike should select a bounded question with Aslan, inspect the relevant source and current template, and identify what behavior would improve. It should not rewrite the whole toolkit from the older exploratory architecture. The [artifact-storage pin](research-artifact-naming-and-ignore-rules.md) remains available for the broader storage/provenance questions.
