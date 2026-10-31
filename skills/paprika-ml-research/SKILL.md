---
name: paprika-ml-research
description: Refine reusable ML research methods from curated papers and experimental work, and apply those methods to research questions, architecture choices, training strategies, and experiment design. Use for evidence-backed research or design decisions and maintaining a method library; ordinary paper filing or summarization alone does not require this workflow.
metadata:
  version: 0.1.0
---

# Paprika ML Research

Help the user make a concrete research or design decision using conditional, evidence-linked methods. Keep the reusable reasoning procedure here; keep evolving topics, papers, experimental results, and local preferences in a separately supplied method library. Any agent may use the skill without a Paprika company, particular roster, connector, or this skill's originating repository.

## Establish the decision and knowledge source

Identify the choice or uncertainty, desired outcome, available evidence, and constraints that could change the recommendation. Reuse context; ask only for consequential missing information. A research question may need a discriminating experiment before it needs an architecture recommendation.

Find the method library named in the request or linked by the current project's instructions/index. A project may use `methodology/INDEX.md` and `library/sources.json`, but these paths are conventions, not dependencies. Confirm the intended library when several unrelated ones are available. Read its index and selected cards, not the entire corpus. Record the source snapshot or versions used. Respect a requested PR/revision instead of silently using another checkout.

If no method library is available, proceed from supplied research or accessible primary sources, marking newly inferred methods as proposals. Say which evidence is missing and how that limits the decision. Never imply that an unavailable private library or another agent's memory was consulted.

## Choose the work

- **Refine:** The user brings papers, a research focus, completed experiments, or conflicting findings. Follow [refine methods](references/refine-methods.md) to produce or revise conditional methods.
- **Decide:** The user brings a problem, design choice, or proposed experiment. Follow [apply methods](references/apply-methods.md) to select relevant methods and produce a recommendation and a way to test it.
- **Learn from outcomes:** Follow the refinement workflow to compare an actual result with its decision record. Change the rule's scope or confidence only as far as the evidence warrants; preserve earlier versions and unresolved contradictions.

These may form a loop. Do enough refinement to support the present decision; do not turn every question into a comprehensive literature review. Use the [method library contract](references/method-library.md) when interpreting or writing reusable records. Existing compatible schemas need no migration.

## Evidence and transfer

Keep source claims, observed evidence, cross-source inference, and project recommendations distinguishable. Read the primary material needed for consequential claims, with version and section/table/experiment locators where available. Abstract-only access supports orientation and hypotheses, not invented ablations or audited results. A paper's presence in a category is not evidence for a decision rule.

Choose methods by mechanism, applicable conditions, decision relevance, and evidence quality. Explain how the source setting maps to the target problem and where it fails. A familiar topic, popular method, or human-selected research direction is not a substitute for applicability. Explicitly reject a candidate when its prerequisites are absent. Do not force a choice from the library when none fits.

Treat a source and a blog describing that source as one evidence lineage unless they contain genuinely separate experiments. Check relevant conflicting findings and negative results. Separate scientific review, reproduction, and local adoption: none automatically implies the others. Human confirmation of a preference does not validate a scientific claim, and no reading list establishes a person's private reasoning.

Use existing research/citation tools or skills when available and helpful. Verify current claims when the decision depends on recent evidence. State actual access and tool limits; no particular paid service is required.

## Return useful decisions

Lead with the recommendation or the uncertainty that prevents one. Explain why the selected method fits, the strongest viable alternative, the material evidence limits, and the next observation that would change the decision. Scale detail to the task. A small decision may need a paragraph; a substantive research proposal benefits from a comparison and explicit experiment design.

Offer the cheapest informative test before an expensive commitment. If decisive evidence is unavailable, give a conditional recommendation and an evidence-acquisition plan instead of asserting certainty or only listing papers. Do not manufacture a numerical confidence score, performance gain, or budget threshold.

## Paprika Inc integration and adoption

Use the current company's ownership and review rules if present. Curating sources, synthesizing evidence, refining methods, and independent review are responsibilities that may be performed by its existing roles; this skill creates no roster or mandatory multi-agent workflow. A reviewer must not be credited with review they did not perform.

For an authorized company handoff, use the installed Paprika Inc communication workflow and include the decision, selected method IDs/versions, evidence locations, constraints, unresolved questions, and requested deliverable. Do not copy native routing identifiers into a public method library. If Inc is unavailable, return the handoff content in the current conversation.

Using the skill does not approve experiments, spending, publication, messages, background work, or changes to another agent's instructions. Perform actions already authorized by the user's task and host. Save method/decision records when maintaining that library is part of the request; otherwise return them in the conversation. A consuming agent adopts a specific method version for a stated problem, not the originating project's personal preferences or authority.
