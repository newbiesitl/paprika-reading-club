# Doc-to-LoRA: Learning to Instantly Internalize Contexts

- Source ID: `arxiv:2602.15902`
- Authors: Rujikorn Charakorn; Edoardo Cetin; Shinnosuke Uesaka; Robert Tjarko Lange
- Year: 2026
- Version: v1, 2026-02-13
- [Primary source](https://arxiv.org/abs/2602.15902v1)
- Provenance: `assistant-discovered`
- Metadata verified: 2026-10-31, primary source
- Current-pass access: `abstract-only`
- Human reading status: unknown
- Independent scientific review: pending
- Category: [Memory Networks](README.md)
- Relationship to MemT-1: `evaluated-baseline-alternative-mechanism`

## Why read it

A context-internalization comparator evaluated in MemT-1.0; a different mechanism from recurrent memory.

## Initial source orientation

Doc-to-LoRA uses a hypernetwork to generate a LoRA adapter from a context. Subsequent queries use that adapter without re-consuming the original context.

## Proposed reading question

Can generated adapters support accumulated experience, and how does adapter construction compare with recurrent writes?

Use the [paper-note template](../../templates/paper-note.md) for a full reading. This is an initial curation note, not a completed scientific review.
