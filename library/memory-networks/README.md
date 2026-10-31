# Memory Networks

Memory networks are an explicit research focus selected by the human. This category starts from [MemT-1.0](arxiv-2610.26825.md) and asks how models can accumulate, revise, and use information through persistent learned state.

The first reading priority is the direct lineage, followed by evaluated alternatives and broader architectural comparisons. This order is a curator recommendation, not a performance ranking.

## Related readings

| Paper | Relationship to MemT-1 | Comparison axis |
| --- | --- | --- |
| [Metis](arxiv-2607.26760.md) | Direct predecessor | Native state updated by forward computation |
| [Gated DeltaNet-2](arxiv-2605.22791.md) | Update-rule lineage | Separate erase and write gates |
| [δ-mem](arxiv-2605.12357.md) | Evaluated comparator | Small delta-rule state coupled to attention |
| [LiveMem](arxiv-2608.02515.md) | Evaluated comparator | Persistent state across context turnover |
| [MEMORYLLM](arxiv-2402.04624.md) | Evaluated comparator | Self-updating latent memory pool |
| [Doc-to-LoRA](arxiv-2602.15902.md) | Evaluated alternative | Context encoded into generated adapters |
| [Titans](arxiv-2501.00663.md) | Broader architectural comparison | Attention plus learned long-term neural memory |
| [TTT layers](arxiv-2407.04620.md) | Broader conceptual comparison | A learned model serves as recurrent state |

The lineage and evaluated-comparator labels follow [MemT-1's introduction, architecture, and evaluation references](https://arxiv.org/html/2610.26825v2). Titans and TTT are additional architectural connections proposed by the curator. Each note links to its own primary source. New recommendations are verified at the metadata/abstract level; they have not received full independent scientific review.

## Proposed reading order

Metis → Gated DeltaNet-2 → MemT-1 → δ-mem / LiveMem → MEMORYLLM. Then compare Titans, TTT, and Doc-to-LoRA to explore different locations and update rules for memory.

## What to compare

1. **State and lifetime:** what persists between turns, between sessions, and after context eviction? Which trained weights stay fixed?
2. **Write, read, and forget:** how are new facts incorporated, contradictions corrected, and old facts retained or removed?
3. **Capacity and cost:** measure memory size, write cost, query latency, and total interaction cost under matched budgets.
4. **Evidence:** compare recall, temporal updates, procedural transfer, interference, and retention of general abilities. Keep benchmarks and model sizes comparable.

External retrieval, recurrent state, generated adapters, and test-time parameter updates offer different mechanisms. A persistent memory is not automatically a predictive world model; a proposed bridge to [world modeling](../../methodology/core-ideology.md#2-learn-world-models-for-planning-and-discovery) is whether retained experience improves prediction and planning on new situations.

[All sources](../INDEX.md) · [Research agenda](../../agenda/AGENDA.md) · [Reading queue](../../reading/QUEUE.md)
