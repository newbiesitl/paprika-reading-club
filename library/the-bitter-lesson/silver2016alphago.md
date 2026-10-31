# Mastering the game of Go with deep neural networks and tree search

- Source ID: `doi:10.1038/nature16961`
- Authors: David Silver and others
- Year: 2016
- Version: published 2016-01-27; Nature 529, 484–489; AlphaGo
- [Canonical publication](https://doi.org/10.1038/nature16961)
- [Primary research listing and abstract inspected](https://research.google/pubs/mastering-the-game-of-go-with-deep-neural-networks-and-tree-search/)
- [Author-hosted paper PDF](https://storage.googleapis.com/deepmind-media/alphago/AlphaGoNaturePaper.pdf)
- Provenance: `assistant-identified-from-user-example`
- Metadata verification: checked against primary research and publisher records on 2026-10-31
- Current-pass access: `abstract-only`
- Human reading status: unknown
- Independent scientific review: pending
- Category: [The Bitter Lesson](README.md)

## Why it is in this library

The human requested AlphaGo and AlphaZero under Sutton's The Bitter Lesson category. The assistant identified this original AlphaGo paper as the supervised-learning and self-play starting point for that comparison.

## Initial source orientation

AlphaGo combines policy and value networks with Monte Carlo tree search. Its training pipeline uses human expert games and reinforcement learning from self-play. This makes it a useful comparison with the later [AlphaZero preprint](arxiv-1712.01815.md), which investigates learning without human demonstrations.

## Reading question

Which benefits come from human demonstration bootstrapping, self-play improvement, value estimation, and search? What changes when the demonstrations are removed?

Use the [paper-note template](../../templates/paper-note.md) for full reading and evidence checks. Category selection does not establish endorsement of every source claim.
