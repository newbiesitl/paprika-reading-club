# Core research ideology

The Research Director explicitly selected the two pillars below during initialization. The direction is human-confirmed; the technical framing and evaluation practices are assistant proposals for review. This records expressed research preferences, not a claim to reconstruct private reasoning.

## 1. Learn beyond imitation

Use supervised learning as a useful starting point, then seek improvement through reinforcement learning, exploration, search, and interaction. Also investigate learning without human demonstrations when the environment and learning signal make that feasible. Human examples should enable progress without becoming a permanent ceiling on the solutions or representations a system can discover.

The human cited AlphaGo to AlphaZero, LLM supervised fine-tuning to RL, and learned byte-level hierarchies as motivating examples. These illustrate different ways to relax human-imposed assumptions; they do not all use the same training mechanism.

| Example | What may become less dependent on human design | Distinction to preserve |
| --- | --- | --- |
| AlphaGo → AlphaGo Zero / AlphaZero | Human expert trajectories | Earlier AlphaGo combined demonstrations and RL; the Zero systems learn by self-play without those demonstrations. Rules, objectives, architecture, and search still matter. |
| LLM SFT → RL | Restriction to imitating provided answers | This is the human's preferred investigation path, not a claim that every RL method escapes imitation or that pretrained knowledge disappears. |
| Fixed tokenization → learned byte hierarchies | A fixed segmentation of the input | HNet investigates learned representations through end-to-end training; this example is not evidence of RL. |

“Escaping local minima” expresses an ambition to move beyond narrow human priors. It is not an established guarantee about an optimizer. “Broader search space” is the operational aim: every experiment still has constraints imposed by its objectives, environment, observations, model class, and resources. Removing a useful prior can also make learning less efficient.

Sources: [AlphaGo Zero author account](https://deepmind.google/blog/alphago-zero-starting-from-scratch/), [AlphaZero](../library/the-bitter-lesson/arxiv-1712.01815.md), and [From Tokens to Bytes I](../library/the-bitter-lesson/cartesia2026tokensbytes.md).

## 2. Learn world models for planning and discovery

World modeling is a main research ideology explicitly selected by the human. Earlier discussions about OneRec, behavioral prediction, exploration, and causal world models provide context for this preference; they do not establish endorsement of a particular paper or implementation.

Proposed formulation: learn representations of the environment and how actions change it; use predicted consequences to compare plans, explore, and improve behavior; test those predictions against further interaction. Study both models that support search and models that support learning from imagined experience. [MuZero](../library/arxiv-1911.08265.md) and [DreamerV3](../library/arxiv-2301.04104.md) are assistant-suggested starting references.

Keep separate:

- **Action generation:** predicts or proposes what to do.
- **World modeling:** predicts relevant consequences given a state/history and candidate action. A task-relevant latent model need not reconstruct every observable detail.
- **Causal reasoning:** supports claims about interventions under stated assumptions. Good observational prediction alone does not establish counterfactual validity.

For recommendation, generating an item sequence is different from predicting a user's response to serving it. For control, successful imagined behavior must be checked in the environment; model error can compound or be exploited by a policy. These are proposed review questions, not findings already established for the recovered papers.

## Shared methodological anchor

[The Bitter Lesson](the-bitter-lesson.md) is the human-selected foundation: investigate methods whose learning and search improve with resources, while measuring where specialist structure still helps. The combined direction is **learn representations, learn consequences, and improve decisions through experience and search**.

## Proposed evaluation practice

1. Identify the exact human assumption being relaxed: labels, demonstrations, token boundaries, features, dynamics, or a handcrafted policy.
2. Compare supervised-only, supervised-then-RL, and demonstration-free learning when each is meaningful. Count pretraining data, interaction, compute, search cost, and evaluation budget.
3. Compare fixed and learned representations separately from changes in the learning objective.
4. Compare a world-model approach with a credible alternative under matched budgets. Measure actual task outcomes as well as predictive accuracy, uncertainty, model exploitation, and distribution shift.
5. State what result would contradict the hypothesis. Broader exploration or a more general architecture is not itself evidence of a better solution.

The Research Director chooses experiments and accepts methodology changes. These priorities do not authorize autonomous experiments, spending, publishing, or background work.
