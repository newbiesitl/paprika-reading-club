# Role skills

The [company manifest](../company/company.json) selects Paprika Inc’s bundled packs for the Literature Reviewer (`research-core`) and Backend Engineer (`engineering-core`). Their contracts describe when to use them. The independently maintained [Paprika ML Research source](../skills/paprika-ml-research/SKILL.md) remains under the Methodologist’s ownership.

## Reproduce the local installation

Use the installed Paprika Inc 0.3.10 helper in the selected Git project. Resolve `PAPRIKA_INC_ROOT` from the actual installed plugin location; do not copy another machine’s private paths or runtime journal.

```sh
node "$PAPRIKA_INC_ROOT/skills/paprika-inc/scripts/inc.mjs" skills plan --repo "$PWD" --roles literature-reviewer,backend-engineer
node "$PAPRIKA_INC_ROOT/skills/paprika-inc/scripts/inc.mjs" skills install --repo "$PWD" --roles literature-reviewer,backend-engineer
node "$PAPRIKA_INC_ROOT/skills/paprika-inc/scripts/inc.mjs" skills status --repo "$PWD" --roles literature-reviewer,backend-engineer
```

The installer materializes the selected skills under `.agents/skills/` and retains bundled licenses, portability guidance, and provenance. Those installation copies are ignored by Git; this repository versions the role selections and installation procedure. The private install journal stays under Git’s common directory. Preserve conflicts with unmanaged or modified skill directories for reconciliation rather than overwriting them.

| Pack | Installed skills | Bundled provenance |
| --- | --- | --- |
| `research-core` | `paper-lookup`, `literature-review`, `citation-management`, `scientific-critical-thinking` | Scientific Agent Skills 2.72.0, commit `a1043ef544e3a100c28e70a736b6cf32554d0677` |
| `engineering-core` | `paprika-code-review` | Adapted engineering guidance pinned to `2c606141936f1eeef17fa3043a72095b4765b9c2` and `742e0abae1501e12d1254a81d05f16bba10d08c1` |

Read each selected `SKILL.md` and `INC-PORTABILITY.md` before use. Integrity checks verify the bundled bytes; native discovery, API authentication, full-text access, integration behavior, and scientific or engineering quality require separate evidence. Missing optional integrations do not block basic Markdown synthesis or analytical review. Skill selection does not restrict discovery to one role or grant execution authority.

The user-selected chat settings are GPT-6 Astra with extra-high reasoning for Literature Reviewer and GPT-6.1 Sol with extra-high reasoning for Backend Engineer. These are creation preferences, not automatic configuration of other chats. Native bindings and setup receipts remain private.
