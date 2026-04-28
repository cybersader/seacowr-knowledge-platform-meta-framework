---
title: System (S) — SEACOW(r) component
publish: true
---

# System (S)

**Question:** What platform / technology context are we in?

The System component is the substrate everything else runs on. It determines
your **affordances** (what's possible) and your **constraints** (what isn't).
You can't analyze Capture, Work, or Output meaningfully without first knowing
the System.

## Examples

- Obsidian vault with plugins (Templater, Dataview, Tag Pages, etc.)
- Windows SMB file share (folders only — no tags, no graph layer)
- Git repository (folders + frontmatter + README/index files)
- Notion workspace (databases, relations, pages, properties)
- Claude Code `.claude/` directory (skills, agents, settings, hooks)
- Physical office with file cabinets (rigid hierarchy, single-parent)

## Analysis: questions to ask

- Can you use **tags**? **Properties**? **Wikilinks**? Or only **folders**?
- Is the model **hierarchical**? **Graph-based**? **Database-like**? **Flat**?
- Who has **access**? What are the **permissions**?
- Is it **versioned**? **Searchable**? **Shareable**? **Backed up**?
- What's the **rendering surface** (markdown? rich text? a static site? a published vault?)
- What plugins / extensions / integrations are available?

## How System shapes the rest

| If your System... | …then |
|---|---|
| has tags + folders + links | you have *choices*; rules need to specify *which* primitive to use for what (see [folders-vs-tags-vs-links-vs-metadata](../../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md)) |
| has only folders (file share, OS) | you must encode polyhierarchy via shortcuts, indexes, or naming conventions |
| has databases + relations (Notion, Airtable) | the relation layer is structural, not implicit; design schemas first |
| has version control (Git) | distinguish "working" from "history" — Git's branches and commits encode some Activities for you |

## Anti-patterns

- ❌ Designing structure independent of the platform's affordances ("I'll use this exact tag system in a tag-less file share").
- ❌ Ignoring permissions — the System might forbid Entity boundaries you assumed possible.
- ❌ Treating *plugins* as free affordances — they're affordances *if* installed and *if* still maintained. Document the dependency.

## Cross-references

- Multi-platform comparison: [../../06-applications/](../../06-applications/)
- Platform-specific limitations: [../../02-tools/platform-notes/](../../02-tools/platform-notes/)
