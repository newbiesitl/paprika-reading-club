# Reading workflow

1. **Capture:** preserve the supplied title or URL and classify provenance as `user-shared`, `user-mentioned`, `user-requested`, `assistant-discovered`, or `unverified-recollection`.
2. **Identify:** resolve canonical metadata and versions; distinguish a verified bibliographic match from verified scientific claims. Deduplicate by DOI/arXiv ID or canonical URL.
3. **Triage:** connect the source to an agenda question; record selection or rejection rationale, priority, and prerequisites. The user makes final priority choices.
4. **Read:** use the paper-note template. Mark access as metadata-only, abstract-only, full-text, or reproduced. Separate claims, evidence, interpretation, and proposed extensions.
5. **Review:** a different role checks substantive claims against primary sources and records the reviewed file/revision. An agent cannot certify its own work.
6. **Synthesize:** compare assumptions, mechanisms, results, failure modes, and the experiment that would distinguish competing explanations.
7. **Reflect:** invite the human to record what mattered, what they rejected, and what changed. Do not fill missing reactions with inferred beliefs.
8. **Distill:** the Methodologist proposes a scoped pattern with evidence, alternatives, and counterexamples. Status is `proposed`, `human-confirmed`, `rejected`, or `superseded`.
9. **Revisit:** record changed beliefs and reasons without erasing earlier uncertainty.

For reusable scientific decision support, continue through the [research skill workflow](RESEARCH_SKILL.md): distill conditional methods, apply them to a concrete problem, and revise them from measured outcomes. Use separate scientific-review and project-adoption states; the personal-principle confirmation in step 8 does not validate a scientific claim.

Queue states: `inbox`, `selected`, `reading`, `notes-ready`, `reviewed`, `synthesized`, `deferred`. A source’s queue state does not imply that the human personally read it. Keep human reading status separately as `unknown`, `skimmed`, or `read`.

For a public repository, keep raw conversation excerpts and private reflections in `private/` (ignored), and runtime routing under Git’s common directory. Public notes may contain research metadata and deliberately prepared summaries, not native chat IDs or service bindings.
