---
title: Folders vs Tags vs Links vs Metadata
publish: true
permalink:
date created: Monday, March 17th 2025, 9:37 pm
date modified: Monday, March 17th 2025, 9:41 pm
source: cybersader/cyberbase — 📁 54 - Obsidian Vault Organization/Folders vs Tags vs Links vs Metadata
---

# Folders vs tags vs links vs metadata

The four organizational primitives in most knowledge platforms. SEACOW(r)
doesn't tell you which to use — it tells you what each one *should answer*.
Use this page to choose deliberately.

## Quick decision matrix

| Primitive | What it's for | What it costs |
|---|---|---|
| **Folders** | Strict structure or ontology. Use this for **Output** / consumable to your general audience or yourself. Works in other systems (file explorer, OS, sync clients). | Limited by OS and Obsidian file/folder naming rules. **Polyhierarchy is hard** — each item gets exactly one folder home. |
| **Tags** | **Overlapping ontologies.** Cross-cut categorization. Clustering topics with additional keywords. Many parents per item. | Sorting is platform-specific (Obsidian uses Chromium collation; OS file explorer uses something else). Limited punctuation. Discoverability via Tag Pane is good but not as good as folders. |
| **Links** | **Relationships** to other notes. Very flexible — you can encode arbitrary semantics (transcludes, references, dependencies). | One-way by default (Obsidian shows backlinks but the link itself is one-way). Graph noise grows faster than usefulness if you link indiscriminately. |
| **Metadata / properties / frontmatter** | **Structured information about a note** — status, type, dates, author, related entities. Queryable via Dataview / Bases. | Frontmatter is invisible in reading view unless surfaced by plugins or callouts. Schema discipline required — typos create silent fragmentation. |

## Mapping primitives to SEACOW(r) activities

| SEACOW(r) component | Best primitive(s) | Why |
|---|---|---|
| **System** | Frontmatter for system-internal metadata; folders for system-required structure (templates, attachments) | System affordances should be *predictable* and *machine-readable*. |
| **Entity** | Tags + frontmatter | Entity is cross-cutting — same content may belong to several entities. Tags handle this; frontmatter encodes structured Entity properties. |
| **Capture** | Folders (shallow) + tags (flat) | Captures need a low-friction landing place. Shallow folders + a small flat tag vocabulary keep it fast. |
| **Work** | Folders (by process, not content) + frontmatter (status field) | Process structure cues *how* work flows. Status frontmatter cues *where* something is in the lifecycle. |
| **Output** | Folders (deep, audience-facing) + frontmatter (publish flag) | Output benefits from depth and from a clear "is this published?" signal. |
| **relation** | Links + tags (flat) + MOCs | Relation is precisely the graph layer. All three primitives compose; MOCs are curated relation explicitly. |

## When to convert from one primitive to another

- Tag becomes a folder when: it's *exclusive* (every note has at most one
  value) AND it's used for primary navigation by an Entity.
- Folder becomes a tag when: items legitimately have multiple parents AND the
  folder hierarchy starts forcing artificial choices.
- Link becomes a tag when: the same link appears across many notes — promote
  it to a shared classifier rather than copy-paste.
- Frontmatter becomes a tag when: a property is binary or short-enum AND you
  want it to sort in the Tag Pane.

## Anti-patterns

- ❌ **Tag-only design.** Without folders for Output, audiences can't browse
  your work. Tags are bad navigation for non-technical readers.
- ❌ **Folder-only design.** Forces every item into a single hierarchy; can't
  represent cross-cutting concerns.
- ❌ **Link-only design.** Great graph, no entry points. New visitors have
  nowhere to start.
- ❌ **Frontmatter-only design.** Invisible to most readers; queryable but not
  navigable.

## See also

- [Combining tags, links, & folders](combining-tags-links-folders.md) — how to compose them.
- [Choosing a tag structure](choosing-a-tag-structure.md) — applied tag decision-making under SEACOW(r).
- [relation component](../01-framework/components/relation.md) — when relation deserves first-class treatment.
