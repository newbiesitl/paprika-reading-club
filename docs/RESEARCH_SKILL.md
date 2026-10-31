# Research that produces reusable methods

The reading club maintains a method library that other agents can use for ML research and design decisions. The reusable procedure lives in [Paprika ML Research](../skills/paprika-ml-research/SKILL.md); the club's evolving evidence and conditional rules live in the [method index](../methodology/methods/INDEX.md). The skill also works with other projects' libraries and does not require this company's roles or services.

The working cycle is:

**Research focus → curated evidence → conditional method → problem-specific decision → experiment/outcome → revised method.**

## From categories to methods

Keep adding papers to meaningful categories, as in [PR #3](https://github.com/newbiesitl/paprika-reading-club/pull/3). For a useful subset, identify the decisions it could improve: whether to replace a fixed representation, invest in feedback-driven training, use a world model, or keep a simpler baseline. Read and compare mechanisms, assumptions, counterexamples, and costs before distilling a rule.

Each rule states when it applies, when it fails, which evidence supports it, what remains a transfer hypothesis, and what test would change the decision. Category membership is many-to-many with methods; adding a paper does not automatically endorse or strengthen a method. The three starter methods are proposals awaiting deeper synthesis and independent scientific review.

## Using the skill

The canonical portable source is `skills/paprika-ml-research/`, owned by Methodologist in the company's public ownership map. An optional, Git-ignored discovery copy at `.agents/skills/paprika-ml-research/` supports project-local discovery; Paprika Inc treats `.agents/` as internal and does not accept it in that ownership map. Refresh the discovery copy deliberately from the canonical source after skill edits, preserving unrelated installed skills and checking for local modifications before replacement.

Once discovered by the host, an agent can invoke `$paprika-ml-research`; a task can also give the canonical SKILL.md path and method index. Example requests:

> Use $paprika-ml-research with methodology/methods/INDEX.md. We have a supervised recommender, logged feedback, and a strict serving budget. Compare retaining it, feedback-driven improvement, and a learned world model. Recommend the next informative experiment and state the assumptions we still need to check.

> Use $paprika-ml-research to refine the Bitter Lesson reading category into conditional methods. Trace claims to the sources actually inspected, include counterevidence, and keep proposed rules separate from reviewed ones.

An adopting agent selects method IDs and versions relevant to its problem, checks the source evidence and conditions, and records its own recommendation or adoption decision. It does not inherit the Research Director's preferences as universal facts.

For another environment, the skill folder is a self-contained reusable unit. Supply a method library separately through that environment's permitted file or knowledge access. Use the target host's supported skill/plugin installation route; copying source is not proof of discovery or live activation. This project source does not update the installed Paprika Inc account plugin. A later plugin release can package the same skill without embedding private data or freezing the entire reading library into its instructions.

## Invocations and current support

Version 0.1.0 has **one skill invocation**, `$paprika-ml-research`, and **three named workflows**: Refine, Decide, and Learn from outcomes. It has no CLI parser, flags, or registered `scope`, `refine`, `apply`, or `deep-dive` subcommands. The phrases below are natural-language task requests after invoking the skill.

| Use case | Suggested invocation | Support in v0.1.0 |
| --- | --- | --- |
| Identify problem scope | `Use $paprika-ml-research to scope this problem: [description]. Identify the decision, constraints, competing explanations, relevant research areas, and evidence gaps. Stop before choosing a method.` | Supported within decision framing; no dedicated scoping mode or standardized problem-map artifact |
| Refine methods | `Use $paprika-ml-research to refine methods from [papers, research focus, or experiment records]. Produce conditional rules with evidence, limits, counterexamples, and tests.` | Explicit Refine workflow |
| Apply methods | `Use $paprika-ml-research to apply our method library to [problem]. Compare feasible alternatives and recommend an action and a discriminating experiment.` | Explicit Decide workflow, backed by the apply-methods reference |
| Methodology deep dive | `Use $paprika-ml-research to investigate methods for [scoped problem]. Identify gaps in our library, search accessible primary literature, compare promising mechanisms and contrary evidence, and propose candidate methods.` | Supported through refinement and evidence gathering when search access exists; no dedicated deep-dive protocol or bundled systematic-review workflow |
| Learn from outcomes | `Use $paprika-ml-research to compare [experiment outcome] with [decision record] and revise the affected method's scope, confidence, and version.` | Explicit Learn from outcomes workflow |

For a reproducible literature review, use an available literature-review skill alongside this skill, with recorded search scope, queries, screening, access limits, and evidence tables. The general skill does not install or guarantee such tools, comprehensive coverage, or access to every paper. A missing research method in the library is an evidence gap to investigate, not permission to invent supporting results.

### Example: long recommendation histories

> Use $paprika-ml-research to scope this problem: our Qwen-based recommendation pipeline cannot handle the length of users' interaction histories. Distinguish the observed failure from its proposed cause. Identify relevant research areas and what measurements would distinguish them. Stop before recommending an architecture.

The useful output is a problem map: observed symptoms, the target quality metric, exact model/version and input representation, history-length distribution, configured limits, truncation behavior, and serving constraints. It should distinguish a hard input limit, loss of relevant events during preprocessing, poor use of distant evidence, and a computational bottleneck as hypotheses to check.

Possible investigation areas include memory/recurrent state, retrieval or event selection, history/context compression, efficient long-sequence architectures, and distillation for a deployment constraint. These are candidate search directions, not findings that a particular method solves this pipeline. In particular, ask whether “distillation” means compressing the input evidence or transferring a teacher's behavior into another model; those are different proposed interventions. Select and refine methods only after checking the task and available evidence.

## Work and review

The existing roster can support this cycle within authorized tasks: Curator preserves source identity and selection rationale; Researcher develops evidence syntheses and inspects mechanisms and experiment implications; Methodologist proposes decision rules; Scientific Reviewer checks the exact candidate against its evidence; Coordinator tracks the problem and its outcome. Canonical ownership remains in [ownership.json](../company/ownership.json). This workflow does not create assignments or change live role bindings.

Keep scientific methods separate from [personal research-profile proposals](../methodology/research-profile-proposals.md). A method may be useful without claiming it describes the human's thought process. Human-selected research directions guide what the club investigates; scientific review and target-project adoption remain distinct.

Use the skill's [record contract](../skills/paprika-ml-research/references/method-library.md). For a substantive authorized task, save its decision record with the task's existing evidence (for example under `work/`), then append measured outcomes and proposed method revisions. Preserve links to older method versions. Track decisions clarified, experiments made more informative, and revisions prompted by evidence rather than treating paper counts as research progress.
