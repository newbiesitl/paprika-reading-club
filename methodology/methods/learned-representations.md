# Test a learned representation against a fixed one

- ID / version: `learned-representations` / `0.1.0`
- Updated: 2026-10-31
- Lifecycle: proposed
- Independent scientific review: pending
- Local adoption: unassessed; no target-project trial recorded
- Origin: source-inspired method proposal

## Decision and applicability

Should a fixed segmentation, feature representation, or other interface become learned? Use this method when there is a concrete suspected bottleneck and access to suitable raw inputs, training resources, and comparable downstream evaluation. Stable interfaces, limited data, strict latency, or a useful domain prior may favor the existing representation.

## Proposed rule

Test whether adapting the representation to the task helps enough to justify its learning and execution costs. Keep changes in representation, architecture, learning objective, data, and budget separable where feasible. If several must change together, report a comparison between complete systems and avoid attributing all gains to representation learning.

## Evidence boundary

`arxiv:2507.07955v2`, [H-Net: Dynamic Chunking for End-to-End Hierarchical Sequence Modeling](https://arxiv.org/abs/2507.07955v2), abstract, inspected 2026-10-31. Access: **abstract only**. The authors describe learned, context-dependent segmentation within a hierarchical model. This supports investigating adaptive representations; the abstract has not been treated as an independently audited comparison. Full methods, ablations, implementation, and reproducibility still need inspection for a specific design commitment.

[PR #3](https://github.com/newbiesitl/paprika-reading-club/pull/3) groups H-Net with `cartesia2026tokensbytes` and the Bitter Lesson readings. A related architecture paper and article are not automatically independent evidence. This representation question is separate from RL and does not establish that a learned representation improves every task.

## Alternatives, test, and revision

Compare the current fixed representation, a credible alternative fixed representation where useful, and the proposed learned representation. Evaluate the same target inputs and downstream outcomes. For byte-versus-token language modeling, do not compare raw per-token loss as if the units were identical; use a justified common unit and end-task evaluation. Account for data exposure, training work, sequence length, memory, and end-to-end serving cost where relevant.

Propose ablations that isolate segmentation or hierarchy when practical. Examine domain shifts and inputs poorly represented by the existing preprocessing. Define a meaningful gain and latency/memory limits from the user's task. If gains disappear under comparable evaluation or costs exceed the feasible envelope, keep the fixed baseline or narrow the method's scope.

History: 0.1.0 records a provisional experimental decision rule. No independent review, reproduction, or project adoption is claimed.
