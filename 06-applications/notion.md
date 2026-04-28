---
title: SEACOW(r) for Notion
publish: true
---

# SEACOW(r) for Notion

> [!note] Stub. PRs welcome — see [CONTRIBUTING.md](../CONTRIBUTING.md).

How to apply SEACOW(r) to a Notion workspace. Notion's organizational
primitives differ from Obsidian's — its **databases** and **relations** make
some SEACOW(r) components easier to express, while its **lack of free-form
folders** makes others harder.

## Notion's organizational primitives

- **Pages** — the universal container; can nest arbitrarily.
- **Databases** — structured collections of pages with typed properties.
- **Relations** — typed links between database entries (the killer feature).
- **Properties** — typed metadata on database entries (text, select, multi-select, date, person, file, etc.).
- **Mentions** — `@`-style references to other pages, people, or dates.
- **Sub-pages** — pages can contain other pages (the closest thing to folders).

## Mapping SEACOW(r) → Notion

| Component | Notion primitives |
|---|---|
| **System** | Notion's affordances themselves; properties on system pages (templates, settings) |
| **Entity** | Person properties on databases; team workspaces; permissions per page |
| **Capture** | An "Inbox" database; a quick-capture template; the mobile quick-add |
| **Work** | Project databases with status fields; sub-pages of projects |
| **Output** | Public-shared pages or databases; "Wiki" pages with curated views |
| **relation** | Database relations (the explicit graph layer) + mentions |

## Notable differences from Obsidian

- Notion's **databases-with-relations** are a much stronger relation layer than Obsidian's tags + wikilinks. SEACOW(r)'s `r` is *more* load-bearing in Notion — you'll often want it as a first-class component, not subsumed under Work.
- Notion **lacks file-system-like folders** outside of sub-pages. The "single hierarchy" constraint is even tighter than in Obsidian — you almost always need relations to recover polyhierarchy.
- Notion's **multi-select properties** subsume what Obsidian uses tags for, with stronger schema discipline (controlled vocabulary by default).

## Recommended starting structure

*(Sketch — needs a worked example.)*

- A top-level **Wiki** page (Output for the primary Entity).
- A **Projects** database (Work).
- An **Inbox** database (Capture).
- A **People** database related to Projects (Entity).
- A **Topics** database related to Projects + Wiki entries (relation).

## Open questions

- How to handle multiple Entities (workspaces) cleanly when content needs to be visible to a subset?
- Notion's permissions model is page-level — how does that map to SEACOW(r) Entity boundaries?

Contributors: please send a worked example as a PR. See [CONTRIBUTING.md](../CONTRIBUTING.md).
