# Agentic ResearchOps Comparison — Questions to Resume
## Status and Source Limits
Captured 2026-10-13 from this conversation. This is a guide for resuming comparative work, not a new competitive-research pass. Existing source inspections were recorded on October 8 and October 11. Products and repositories may have changed; re-check the relevant primary files or documentation before relying on their capabilities in a new decision.

A verbatim [private snapshot of the previous companion analysis](../../reference-material/competitive-analysis-snapshot-2026-10-13.md) is available locally. It will not be present in a public clone. The earlier conversation itself includes strong chatbot claims later qualified by Aslan; preserve those qualifications rather than extracting only persuasive-looking differentiators.

## What Aslan Wants the Comparison to Answer
The question is not just “Why not use an existing tool?” Aslan wants to build, customize, learn, and receive credit, while avoiding thoughtless duplication and making his version worth using. Maintenance burden was not the central concern. He also wants to see where the comparison could help him build something better, without treating that aspiration as an achieved result.

Two kinds of authorship matter. First, who supplies the research purpose, questions, method choices, interpretations, and accepted claims? Second, where can a toolkit author express a viewpoint through the actual workflow, rather than branding generic outputs? Human review at the end is not equivalent to preserving human authorship throughout the process.

A useful comparison needs actual folder hierarchies, skill dependencies, state and artifact locations, and the choices each workflow makes. The earlier summaries sounded agreeable but did not make the hard distinctions legible. Do not replace detailed mechanism comparison with another matrix of vague checkmarks.

## Comparison Set Already Introduced
The set expanded during discussion. Aslan specifically questioned why each response introduced apparently brand-new comparators. Keep track of what has already been discussed and why a new candidate is added; do not quietly replace the set each time.

| Comparator or group | Why it belongs in the existing discussion | Concrete thing to inspect next if relevant |
| --- | --- | --- |
| Cookiy | Planning/synthesis skills and a separate service route were discussed | Actual skill dependencies, prescribed outputs/defaults, and the boundary between instructions and service execution |
| Rampstack UX research skill | Example of research instructions for an existing agent | What context it requires, what it writes, and what operational tools it does not itself supply |
| Rally Agent/MCP | Administrative research operations were a major comparison | Actual participant/search, study, outreach, scheduling, and approval capabilities; required service state |
| Istara | Broader application/evidence architecture was introduced | Finding/data models, the links between evidence and interpretation, and which review behaviors are actually implemented |
| ux-research-pipeline | A connected skill sequence with dependent artifacts | Intake, question audit, guide building, assistive/autonomous choices, and pressure to complete prescribed outputs |
| Research OS | Researcher questions, durable context, and human-approved direction | Original-note preservation, curated state, source/interpretation distinctions, change proposals, and discovery of prior reasoning |
| Design Skill Pack | A personal practitioner viewpoint expressed in skills and generators | Differences between instruction contracts and deterministic demonstration generators; whether viewpoint changes actual choices |
| Condens | Analysis/repository assistance and MCP retrieval | Which evidence surfaces the assistant can access, who interprets, and the distinction between internal assistance and external retrieval |
| Maze AI moderator | Participant-facing interviewing as a different form of delegation | Human goal/question configuration, what happens during an encounter, and what the researcher can review afterward |
| User Interviews MCP | Lead surfaced during the later comparison | Verify current documentation and tool inventory before relying on expanded launch/participant-management claims |
| Dovetail, Looppanel, Marvin | Adjacent research repositories and analysis products | Relevant labor-saving or provenance mechanisms without assuming HackPack should become another hosted repository |
| ResearchOps Community, VA, GOV.UK | Discipline, practitioner-workflow, and lineage references | Specific useful procedures and their contexts, without importing an institution's rules wholesale |

These rows preserve the comparison questions and source leads. They are not fresh attestations that every listed feature is currently shipped or available.

## Hard Differences to Make Visible
1. **Procedure versus execution:** Does the repository supply instructions an agent reads, runnable code, or a hosted service with participant and study state? A skill mentioning scheduling does not establish a scheduling capability.
2. **Authorship versus approval:** Does the human supply and revise inquiry, or merely accept/reject the agent's completed plan? What happens when the human has an unformed concern rather than a specification?
3. **Template defaults versus methodological prescriptions:** Are hypotheses, sample sizes, analysis stages, or question counts compulsory? Does the agent have a legitimate way to leave something unsettled?
4. **Source navigation versus justified inference:** Can the user inspect underlying evidence, transformations, uncertainty, disagreement, and contrary cases? A citation or confidence field alone does not answer those questions.
5. **Repository architecture:** Show a small real tree, name each skill's inputs/outputs, explain ordering and dependencies, and identify which file or service owns current state. Avoid inferred generic folder diagrams.
6. **Adoption into existing work:** Does the approach adapt existing researcher-authored materials, or create competing copies and another source of status?
7. **Portability and authority:** What remains useful without CLI access, a subscription, write permissions, or a particular connector? Who can authorize external actions, and where is that recorded?
8. **Authored viewpoint:** Which actual decisions or omissions differ when the toolkit's instructions are present? More documents and headings are not sufficient evidence.

## Candidate Behavioral Comparisons
The previous analysis suggested prompts involving an unformed concern, a thin brief, existing approved materials, a changing inquiry, conflicting interpretations, contradictory raw evidence, and constrained tool access. Those could reveal mechanisms that reading a README misses. They remain proposed probes; this conversation does not establish that competitors were installed or tested.

For a future pass, pick a small common scenario and compare the same step across a few relevant tools. Separate documented instructions, inspected code, observed behavior, vendor claims, and our inference. Retain which claims were corrected. Record a source's date or revision when practical. Do not claim HackPack uniquely preserves human inquiry, provenance, plain files, or readable skills merely because those values matter to Aslan; earlier comparisons already found precedents.

## Open Outcome
The comparison should support choices: reuse a component, adopt an external service, borrow a useful mechanism, reject an unsuitable assumption, or design an improvement to test. It does not have to produce a uniqueness claim. It also should not defer every practical improvement until an exhaustive market survey is complete.
