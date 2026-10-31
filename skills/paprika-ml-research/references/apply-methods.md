# Apply methods to an ML decision

## Frame what changes the choice

Establish the target behavior, current baseline, available data/feedback, evaluation setting, relevant resource limits, and the actual alternatives. Separate the immediate deployment decision from a longer research agenda when they have different constraints. State useful assumptions and proceed conditionally when information is missing; ask when guessing would determine the recommendation.

## Select and test applicability

Use the library index to choose a small relevant set, then read their records and the evidence needed for this decision. Match the mechanism and prerequisites before topic labels. Check lifecycle, review status, contradictory findings, and whether newer results change the rule's scope. Do not recommend a rejected or superseded version as current guidance.

For each consequential method, explain:

- Why it applies here and which assumptions remain unverified.
- Which source observation supports the recommendation and which step is a transfer hypothesis.
- What credible alternative remains, including retaining the baseline.
- What condition would make this method unsuitable.

When methods conflict, compare the assumptions and evidence that drive their different recommendations. Keep multiple hypotheses if evidence cannot resolve them. When none applies, say so and propose targeted investigation or a new provisional method; do not manufacture a match.

## Recommend and discriminate

Give the current best action with a reason tied to the decision. Depending on the evidence, this may be adopting a design, keeping the baseline, running a pilot, or obtaining a missing measurement. A paper's benchmark win or a preferred research direction alone cannot decide the target system's design.

For a proposed experiment, specify the causal contrast and strongest feasible baseline, the variable changed, relevant controls, data split and leakage/contamination checks, primary outcome, resource accounting, and the result that would change the choice. Use repeated runs and uncertainty estimates where stochastic variance could change the conclusion. Keep train-time, search/inference-time, data/interaction, external-tool, tuning, and evaluation costs distinguishable where they matter. State which budgets can be matched and which tradeoffs remain.

Choose a practical success threshold from user constraints or label it as a proposal. If its value is unknown, name what must be measured rather than inventing one. Predefine stop/pivot criteria for costly trials. If a cheap experiment cannot distinguish the hypotheses, explain what evidence would and why the additional cost may be worthwhile.

## Deliver the decision

Use only the detail the problem needs:

1. Recommendation and its scope.
2. Selected methods and versions, evidence, and transfer assumptions.
3. Viable alternatives and why they are currently weaker or unresolved.
4. Next informative test, expected distinguishing observations, and decision criteria.
5. Material uncertainties, evidence access limits, and what would reverse the recommendation.

A substantive decision record also identifies the library snapshot and whether the user has adopted the proposal. A recommendation, approval, and completed experiment are separate states. If asked to execute an experiment, follow the project's actual tooling, authorization, and reproducibility requirements; this guidance is not an execution report.
