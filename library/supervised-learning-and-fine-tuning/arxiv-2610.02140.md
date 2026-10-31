# Finetuning with Sampling: SFT Learns Better Than You Think

- Source ID: `arxiv:2610.02140`
- Authors: Aayush Karan; Sitan Chen; Yilun Du
- Year: 2026
- Version: v1, 2026-10-01
- [Primary source](https://arxiv.org/abs/2610.02140v1)
- [Author project page](https://aakaran.github.io/finetuning_with_sampling/)
- Provenance: `user-requested`
- Metadata verified: 2026-10-31, primary source
- Current-pass access: `abstract-and-author-project-page`
- Human reading status: unknown
- Independent scientific review: pending
- Category: [Supervised Learning and Fine-Tuning](README.md)

## Why read it

Selected by the human to seed the supervised-learning and fine-tuning category.

## Initial source orientation

The authors use MCMC-based projection sampling to reshape expert traces toward the learner's distribution before ordinary SFT. They report improved generalization and reduced forgetting relative to evaluated baselines. These are source claims; this entry does not establish that SFT universally matches or exceeds RL.

## Proposed reading question

How much of the SFT-versus-RL gap comes from training-data distribution rather than the objective itself?

Use the [paper-note template](../../templates/paper-note.md) for a full reading. This is an initial curation note, not a completed scientific review.

Additional checks: count trace generation and filtering costs; compare matched compute and information budgets; inspect the actual sampler against its formal assumptions. Finite pass@k differences alone do not prove a behavior has zero probability under the base model. These are proposed review checks, not findings of this curation pass.
