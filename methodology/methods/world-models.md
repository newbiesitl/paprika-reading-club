# Test whether a learned model improves action selection

- ID / version: `world-models` / `0.1.0`
- Updated: 2026-10-31
- Lifecycle: proposed
- Independent scientific review: pending
- Local adoption: unassessed; no target-project trial recorded
- Origin: source-inspired proposal; world modeling is a human-selected club direction

## Decision and applicability

Would predicting consequences of actions improve a sequential decision problem enough to justify learning and using a model? Establish the observations/history, actions, outcomes, feedback delay, planning horizon, and how predictions can be checked. If data only support passive prediction, the applicability of planning or policy improvement remains uncertain.

## Proposed rule

Model quantities needed for better decisions, then test whether using the model improves actual task outcomes over a credible alternative under the relevant costs. Treat predictive accuracy and decision quality as separate measurements. A model that predicts well on logged data may still fail on actions selected by a new policy.

## Evidence boundary

`arxiv:1911.08265v2`, [MuZero](https://arxiv.org/abs/1911.08265v2), abstract, inspected 2026-10-31. Access: **abstract only**. The authors describe a learned model predicting reward, policy, and value for search. This motivates task-relevant modeling; this pass has not audited experimental results or established transfer to recommendation, language agents, or another target domain.

`arxiv:2301.04104` (DreamerV3) is a further reading candidate in the club's registry for learning through imagined trajectories. Its full paper was not inspected for this card and it supplies no additional validated claim here. Search with a model and policy training in imagined experience should be compared as different uses of a model.

## Alternatives, test, and revision

Compare a suitable model-free policy or supervised baseline with a model used for planning or policy learning. Include an available simulator or simpler dynamics model when that is a serious alternative. Measure real or justified held-out task outcomes alongside model error, rollout horizon, feedback/interaction use, and total decision cost. Look for errors the policy can exploit and worsening predictions under distribution shift.

For recommendation, distinguish proposing an item from predicting the response to serving it. Offline observational prediction alone does not establish effects of interventions; assess action coverage and the assumptions of any off-policy estimate, or propose a suitable controlled evaluation. Do not report an unperformed online test as evidence.

Define a useful decision gain and resource limits for the actual setting. No gain over a strong baseline, model exploitation, or infeasible inference cost would argue for shorter horizons, a narrower model, more evidence, or retaining the baseline.

History: 0.1.0 creates a provisional decision rule and explicit transfer limits. No independent review, reproduction, or project adoption is claimed.
