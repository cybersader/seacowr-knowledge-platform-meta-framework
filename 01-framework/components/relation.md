---
title: relation (r) — SEACOW(r) component
publish: true
---

# relation (r)

**Question:** How do things CONNECT across the structure?

> Lower-case `r` because it's debatable whether Relation is a *core* Activity or just an aspect of [Work](work.md). Include it when the connecting layer is load-bearing in your design; drop it when Work suffices.

Relation is the **graph layer** — the thing that lets you traverse your
knowledge platform sideways instead of only up-and-down through the hierarchy.
Without Relation, you're stuck in a single tree.

## Examples

| System | Relation primitives |
|---|---|
| Obsidian | Wikilinks, tags, graph view, Dataview queries, properties, MOCs |
| File share | Shortcuts, README index files, pinned items |
| Code repo | Imports, references, dependency graphs, cross-links in docs |
| Notion | Relations (database fields), mentions, backlinks |
| Physical | Cross-reference notes, index cards, tabs |
| Wikis | Wikilinks, categories, transclusions, navboxes |

## Analysis: what to ask

- How do you **link related items**?
- How do you **track dependencies**?
- How do you **navigate cross-cutting concerns** that don't fit one folder?
- What's your **graph / network layer**?
- Are relations **manual** (hand-written links) or **derived** (queries, tags)?

## Relation conventions

- **Relations stay flat** — unlike Output, Relation usually shouldn't be deeply
  nested. Tags two levels deep are usually plenty; deeper signals you're using
  Relation as a poor-person's Output hierarchy.
- **One-way vs two-way** — wikilinks are one-way by default but Obsidian shows
  backlinks; design for the back-direction explicitly.
- **Tag types vs Tag instances** — types describe (`status/draft`); instances
  identify (`person/cybersader`). Don't mix the two semantics on the same tag tree.
- **MOCs are Relation made explicit** — Maps of Content are hand-curated index
  notes that turn implicit graph edges into navigable lists.

## When Relation deserves its own component (vs being subsumed under Work)

Promote Relation to its own component when:

- You have **bridging structures** that exist *only* to connect (MOCs,
  dataview index notes, knowledge graphs).
- You have **cross-cutting tags** that span Captures, Works, and Outputs.
- You have **distinct rules** for how relations are formed (e.g. "MOCs are
  curated, not auto-generated").

Otherwise, fold Relation under [Work](work.md) — link tables and dataview
queries are just Work artifacts that happen to bridge things.

## Anti-patterns

- ❌ Using tags as a second folder hierarchy — defeats the polyhierarchy point.
- ❌ Linking everything to everything — graph noise. Relations should be
  meaningful.
- ❌ Auto-generating MOCs from tags without curation — the curation *is* the
  Relation work.

## Cross-references

- Folders vs tags vs links vs metadata: [../../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md](../../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md)
- Combining the primitives: [../../05-deep-dives/combining-tags-links-folders.md](../../05-deep-dives/combining-tags-links-folders.md)
- Dynamic folder ↔ tag bridging: [../../02-tools/plugins/dynamic-tags-folders/README.md](../../02-tools/plugins/dynamic-tags-folders/README.md)
