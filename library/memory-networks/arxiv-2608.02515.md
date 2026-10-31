# LiveMem: Maintaining Memory State Continuity in Long-Running LLM Inference

- Source ID: `arxiv:2608.02515`
- Authors: Zhichen Liu and others
- Year: 2026
- Version: v2, 2026-08-07
- [Primary source](https://arxiv.org/abs/2608.02515v2)
- Provenance: `assistant-discovered`
- Metadata verified: 2026-10-31, primary source
- Current-pass access: `abstract-only`
- Human reading status: unknown
- Independent scientific review: pending
- Category: [Memory Networks](README.md)
- Relationship to MemT-1: `evaluated-baseline`

## Why read it

A persistent-state comparator evaluated in MemT-1.0.

## Initial source orientation

LiveMem keeps a fixed-capacity memory state across context turnover while bounding the main attention KV window. It studies continuity after source tokens are released.

## Proposed reading question

What information survives after its supporting tokens leave the active context?

Use the [paper-note template](../../templates/paper-note.md) for a full reading. This is an initial curation note, not a completed scientific review.
