---
title: SEACOW(r) Glossary
aliases: [SEACOW Component Definitions]
publish: true
---

# SEACOW(r) Glossary

One-line definitions. For depth, follow the link to the component page.

| Letter | Name | One-line | Component page |
|---|---|---|---|
| **S** | System | The platform/technology context (Obsidian, Notion, Git repo, file share, physical filing cabinet…) | [System](../01-framework/components/system.md) |
| **E** | Entity | Who accesses or interacts with the knowledge. Personal, team, public, AI agent. | [Entity](../01-framework/components/entity.md) |
| **A** | Activities | Umbrella for the three operations: Capture, Output, Work. | [Activities](../01-framework/components/activities.md) |
| **C** | Capture | Where information enters the system (inboxes, clippings, raw input). | [Capture](../01-framework/components/capture.md) |
| **O** | Output | Where information exits to a consumer (publications, deliverables, shared artifacts). | [Output](../01-framework/components/output.md) |
| **W** | Work | Where information is processed (drafts, projects, synthesis). | [Work](../01-framework/components/work.md) |
| **r** | relation | How items connect across the structure (links, tags, MOCs, properties). Often the graph layer. Lowercase r because it's not always a fundamental activity — it can be subsumed under Work. | [Relation](../01-framework/components/relation.md) |

## Notational conventions

- **SEA(COWr)** — the canonical short form; the parens emphasize that C/O/W/r are sub-activities under A.
- **SEACOW(r)** — used in prose where the parens around `r` would clutter; same meaning.
- **WO(R)C(S)** — an early acronym variant, kept in the [meta-framework](../01-framework/meta-framework.md) for historical context.

## Companion concepts (not part of SEACOW)

- **Polyhierarchy** — multiple parent paths for the same item. SEACOW doesn't require it but is compatible with it. See [../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md](../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md).
- **Temperature gradient** — hot (raw inbox) → cold (archive). A pacing concept used by some applications of SEACOW; not the framework itself.
- **Maps of Content (MOCs)** — Obsidian-flavored index notes. A specific implementation of *relation*.
- **LATCH** — Location/Alphabet/Time/Category/Hierarchy. A retrieval/recall framework that pairs with SEACOW(r) (SEACOW says *what* to organize; LATCH says *how* to make it findable). See [../04-comparisons/vs-latch.md](../04-comparisons/vs-latch.md).
