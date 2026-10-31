# ML research methods

This is the reading club's evolving method library for the general [Paprika ML Research skill](../../skills/paprika-ml-research/SKILL.md). Other agents can use a specific method with its evidence and limits, without adopting the club's personal research preferences.

Reading categories organize sources. Methods answer decisions and can draw from several categories. These initial records are **proposed, independently unreviewed, and not adopted for any target project**. They turn existing research directions into testable decision procedures; they are not completed cross-paper scientific syntheses.

| Method ID / version | Decision it helps make | Relevant focus | Applicability / important exclusion | Record |
| --- | --- | --- | --- | --- |
| `learning-and-search` / 0.1.0 | Whether to invest in learning or search beyond a current supervised or specialist baseline | The Bitter Lesson; learning beyond imitation | Requires meaningful feedback and a feasible resource envelope; no reliable reward means no automatic RL recommendation | [Learning and search](learning-and-search.md) |
| `learned-representations` / 0.1.0 | Whether to replace a fixed representation or segmentation | Learned representations; The Bitter Lesson | A specific representation bottleneck and comparable evaluation; not evidence for changing the training objective to RL | [Learned representations](learned-representations.md) |
| `world-models` / 0.1.0 | Whether modeling action consequences would improve decisions | World modeling | Sequential decisions and testable action-conditioned predictions; next-item prediction alone does not establish a useful causal world model | [World models](world-models.md) |

## Provenance and maintenance

Seeded on 2026-10-31 from the club's [core directions](../core-ideology.md), existing source notes at `c97395153d441ba62c157010cf2d259d9d35bbea`, and [PR #3](https://github.com/newbiesitl/paprika-reading-club/pull/3) at `de531a48454c88a9fc383d47e4ad3e19b95e3592`. The PR supplies the Bitter Lesson reading category, not scientific validation. Primary-source access performed for these records is stated in each card.

Resolve source IDs through [the source registry](../../library/sources.json). PR #3 introduces category-specific `note_path` fields; older snapshots may require the [library index](../../library/INDEX.md). Do not infer scientific validity or human adoption from metadata verification, category membership, or a moved note.

To add a focus, identify the decisions it could improve, curate relevant and contrary evidence, and write conditional methods using the skill's [library contract](../../skills/paprika-ml-research/references/method-library.md). Record scientific review and local adoption separately. Follow the [research skill workflow](../../docs/RESEARCH_SKILL.md) for decision records and outcomes.
