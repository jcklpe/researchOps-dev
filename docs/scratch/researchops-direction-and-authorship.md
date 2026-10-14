# ResearchOps Direction and Authorship — Scratch Context
## Status and Purpose
Captured from the planning conversation on 2026-10-13. These notes preserve the product discussion for future work. The implemented slice is tracked in the [active spike](../active-spikes/portable-runbooks-and-setup.md); broader ideas here need discussion before implementation.

## Who This Is For
Aslan described an individual or team standing up product, UX, or service-design research in an organized way. They may be starting fresh or entering an existing operation that is more or less organized. Their computing environment may range from complete control of local tools to a tightly constrained institution with restrictions on CLI access, accounts, or software selection.

The toolkit must be useful to people who do not know Markdown or the terminal. An agent-assisted clone path is a useful first demonstration, not a complete solution for every constrained environment. Manual reading, copying, and adapting documents remain legitimate uses. Do not make installing a particular agent, adopting GitHub, or moving all research into Markdown the definition of successful use.

The desired onboarding feeling was **“George Jetson throwing down his suitcase that turns into his flying car.”** Aslan wants a starting structure that is easy to obtain and prepare. This analogy is about lowering setup friction. It is not permission for an agent to invent the inquiry, create an unsolicited study, sign up for services, or configure every possible integration.

The repository is a practical tool to help people doing research do their work. It should not become an academic jargon system, an epistemological manifesto, or a comprehensive personal operating system. Educational context is useful when it makes a researcher's actions more understandable and effective.

## Two Different Kinds of Authorship
### The Researcher Authors the Inquiry
Aslan's objection to indiscriminate generation was not merely a request for a human approval checkbox at the end. A person has a question, purpose, experience, or uncertainty that makes the work worth doing. An agent can support the work in service of that inquiry. Producing plausible research questions, a polished plan, or a report does not establish that useful inquiry took place.

His formulation was: **“Agents don't have questions. Humans should be seeking to answer their questions not just churn out artifacts with no viewpoint. We are seeking to augment human work.”** In context, this states the source of research purpose and judgment; it should not be turned into a ban on an assistant asking clarifying questions or challenging an argument. It does prohibit treating the agent's ability to complete a template as a substitute for the researcher's reason to investigate.

The current operational boundary is deliberately narrower than the entire long-term possibility space: agents initially copy files and set up folders. Later assistance with retrieval, critique, transformations, evidence navigation, or other labor may be considered, but no specific expansion follows automatically from the word “agentic.” The planning discussion also used “agentic” for the way agents help develop and maintain the toolkit itself.

### Aslan Authors the Toolkit
Aslan wants to build this, make it his own, receive credit for a considered contribution, and learn through the process. Those are real goals. A recommendation to adopt another tool solely to avoid maintenance did not answer his concern, because maintenance cost was not what bothered him.

He wants his version to **earn its place**. That means understanding precedents, avoiding blind duplication, and making choices that improve the work or express a useful viewpoint. Competitive analysis can inform reuse, borrowing, rejection, or a better alternative. It should not function as an argument that he must abandon authorship, nor as a marketing exercise assuring him his toolkit is already unique.

His objection to earlier summaries was that they were **“pretty Teflon”**: appealing descriptions did not grapple with the hard differences among actual workflows. A claim such as “human-centered,” “flexible,” or “evidence-grounded” does little comparison work unless it explains a different action, dependency, authority boundary, or failure mode.

## What Would Make the Viewpoint Observable?
This remains a discussion question, not a completed product argument. Candidate places to examine include what the toolkit asks a person to decide, what it refuses to invent, what source material it preserves, how it makes uncertainty and disagreement visible, and how it accommodates work already underway. An authored viewpoint should affect these behaviors, not merely appear in an introduction or as a label on generated documents.

The mechanical first slice establishes a modest boundary that is easy to inspect: copy blank templates, keep examples separate, and ask for actual names/locations/method choices. It does not demonstrate the full epistemological contribution or prove superiority over another toolkit. Likewise, having an agent instruction that says “human authorship” does not yet prove that an agent follows it in use.

## Origins and Presentation
Aslan developed the HackPack through years of federal government contracting, drawing on practices he encountered and adapted and his own ways of organizing research. The earlier source discussion specifically linked its roots to the VA's research framework. That provenance helps explain where the starting structure came from; it does not require keeping all of that structure or framing the toolkit as a minor derivative in its introduction.

Aslan did not want the opening to overemphasize an individual thank-you, sound apologetic about authorship, or imply that he had simply copied a framework with minor edits. He approved this text verbatim, now used in the consumer README:

> ResearchOps HackPack is a practical toolkit for organizing product, UX, and service-design research. It provides reusable templates and runbooks for setting up projects, coordinating the work, and keeping research materials organized.
>
> I developed it through years of work in federal government contracting, bringing together practices I used and adapted there with my own approaches to organizing research. The toolkit gives individuals and teams a starting structure they can adapt to their tools and ways of working.

That is settled opening copy, not an invitation to rewrite it again whenever other parts of the project change. Any later treatment of detailed lineage or attribution should be grounded in actual sources and usefulness to the reader. Current institutional procedures are reference material, not rules binding every HackPack user.

## Terms and Structures Should Earn Their Place
The Product → Project hierarchy initially survived by familiarity: it came from the organizational setting of the original framework. Aslan's examples of cross-service, platform, and academic work exposed its limits. The agent's invention of a missing product-brief template accidentally hid the more useful question: did Product need to be a prescribed level at all?

The adopted answer is no. A project can investigate products or services without copying an organization chart into its directory ancestry. Do not reintroduce Product/Platform wrappers under the banner of completeness or fidelity to the original source. Equally, do not solve every organizational variation by adding more example topologies when a simpler shared model is enough.

The objection to unnecessary folder READMEs has the same character: a file should add useful information beyond the folder's own name. The artifact guide has a specific explanatory job after templates were flattened. A `templates/README.md` that merely announces that templates live there does not.

## Questions Worth Returning To
- What did the first real setup test make easier, and what remained confusing or unnecessarily agent-dependent?
- Which constraints of an existing research operation should the kit recognize before creating parallel files or tasks?
- What learning should the kit provide to a new practitioner, and what would be distracting ceremony?
- Which later behavior would most clearly express Aslan's viewpoint while reducing real work?
- Where is copying or integrating a mature existing tool preferable to building its infrastructure again?

These questions preserve the conversation's direction. They are not a demand to settle all product strategy before fixing a small usability problem, and they are not instructions to start another broad refactor tonight.
