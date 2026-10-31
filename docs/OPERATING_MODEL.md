# Operating model

## Company style

Use a small personal research institute with a question-led agenda and independent scientific review. The useful inspiration from a large research lab is sustained inquiry, criticism, and transfer between ideas and experiments. At this stage, the outputs are a curated library, evidence-linked syntheses, and an evolving methodology.

The human is Research Director: sets priorities, supplies reactions, confirms personal principles, and decides publication. The Coordinator is the intake contact. The other four roles report progress to the Coordinator; review relationships are defined separately in the role contracts and ownership map.

| Role | Main outcome |
| --- | --- |
| Coordinator | A coherent agenda, clear assignments, and tracked decisions |
| Curator | A deduplicated, attributed library and prioritized queue |
| Researcher | Mechanism-level notes and cross-paper syntheses |
| Scientific Reviewer | Independent checks of evidence and conclusions |
| Methodologist | Revisable research principles and belief-change records |

Release preparation is a bounded Coordinator duty for this small roster, with independent review and human publication authority. Add a separate Release Engineer when reproducible code, datasets, multiple parallel PRs, or recurring releases justify the workload. Add topic specialists after recurring demand becomes clear.

## A useful reading cycle

Choose a question, select a small set of papers, read for mechanisms, test claims against evidence, connect the papers, and record what changed. Include a counterexample or competing view when possible. At a synthesis milestone, ask which research decision changed and what would change it again. The cycle is on demand; no schedule or background monitoring is enabled by these documents.

Track useful outcomes: decisions clarified, claims checked, experiments sharpened, and principles revised. Counts of papers or summaries are activity measures only.

## Models and optional skills

The general [Paprika ML Research skill](../skills/paprika-ml-research/SKILL.md) provides the method-refinement and decision-support procedure. The club maintains its [first method library](../methodology/methods/INDEX.md); the skill can also consume other libraries without this roster. See [adoption and research workflow](RESEARCH_SKILL.md). Source availability, host discovery, and scientific readiness are separate states.

Keep the user’s native model defaults unless they select explicit overrides. Paprika’s optional recommendation for Coordinator and Researcher is `gpt-6-astra` with `xhigh` effort where supported; this is a preference to discuss, not a tested accuracy guarantee or an applied setting.

The optional `research-core` pack offers paper lookup, literature review, citation management, and scientific critical thinking. Researcher and Scientific Reviewer are suitable users, with the latter reviewing the former’s scientific claims. The initial manifest does not install or activate that pack. Select and install it separately if desired; API access and full-text availability still need evidence.
