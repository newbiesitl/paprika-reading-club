# Learning and search under a resource budget

- ID / version: `learning-and-search` / `0.1.0`
- Updated: 2026-10-31
- Lifecycle: proposed
- Independent scientific review: pending
- Local adoption: unassessed; no target-project trial recorded
- Origin: source-inspired method proposal; the club's research direction is human-selected

## Decision and applicability

Should the project invest in learning or search beyond its current supervised or specialist baseline? Apply when an outcome can be evaluated, the feedback is meaningful for the real objective, and the available data, interaction, training, and inference budgets permit a useful comparison. Inspect those conditions before recommending an algorithm.

Without trustworthy feedback or feasible interaction, a demonstration-free or RL route may be unsuitable. A fixed deployment deadline or latency ceiling may favor the current design even when a longer research program is worthwhile.

## Proposed rule

Identify the exact assumption or bottleneck to relax. Compare the existing approach with a feasible learning/search alternative, asking which improves as the relevant resources increase. Keep supervised-only, supervised-then-feedback, and demonstration-free alternatives distinct; compare them only when the task supports each. The mechanism hypothesis is that feedback and search can discover solutions beyond the examples or fixed rules currently supplied.

## Evidence boundary

| Source and locator | Access in this authoring pass | Supports | Does not establish |
| --- | --- | --- | --- |
| `sutton2019bitter`, [The Bitter Lesson, 2019-03-13](https://www.cs.utexas.edu/~eunsol/courses/data/bitter_lesson.pdf), concluding paragraphs | Full essay | Sutton's historical argument for methods that exploit increasing computation through learning and search | A theorem, target-system result, or universal instruction to discard useful structure |
| `arxiv:1712.01815v1`, [AlphaZero](https://arxiv.org/abs/1712.01815v1), abstract | Abstract only | An author-reported example of self-play learning in rule-defined board games | That another domain supplies equivalent feedback, or that this pass audited its experiments |

The decision procedure above is a proposal derived from these ideas, not a reported experiment. Confidence in transfer remains unestablished.

## Alternatives, test, and revision

Retain a strong supervised/specialist baseline, and consider a hybrid that preserves useful structure. A proposed pilot changes one mechanism where feasible, reports all meaningful resource costs, and evaluates held-out task outcomes. Compare more than one budget only if estimating a resource trend matters and is affordable; one operating point cannot demonstrate a scaling trend.

Define practical improvement and cost ceilings from the target problem. Reward gaming, degraded held-out outcomes, or a baseline with a better quality/cost tradeoff would weaken the proposal. A failed pilot must be examined for implementation and feedback problems before generalizing its conclusion.

History: 0.1.0 creates a provisional rule and explicit applicability limits. No independent review, reproduction, or project adoption is claimed.
