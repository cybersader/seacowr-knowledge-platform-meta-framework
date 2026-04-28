---
title: SEACOW(r) for Obsidian
publish: true
source: cybersader/cyberbase — 📁 54 - Obsidian Vault Organization/.claude/CLAUDE.md (split — Obsidian-specific use-case content)
---

# SEACOW(r) for Obsidian

How to apply the SEACOW(r) framework to an Obsidian vault. Obsidian is the
most-developed application of the framework — it's where SEACOW(r) was
originally invented (in [cyberbase](https://github.com/cybersader/cyberbase)).

For the framework definition, see [../01-framework/meta-framework.md](../01-framework/meta-framework.md).
For the platform's organizational primitives, see [../02-tools/platform-notes/](../02-tools/platform-notes/).

## The core problem (Obsidian-specific framing)

**Challenge:** file systems are hierarchical (strict trees), but knowledge is
networked (graphs). Obsidian is built on a file system, so it inherits the
hierarchy constraint — and then layers tags, links, and properties on top to
recover graph behavior.

**Reality:**

- Obsidian *must* use a hierarchical file system for storage.
- Human knowledge doesn't fit neatly into hierarchies (overlapping contexts, multiple perspectives).
- Different audiences need different organizational lenses.

**SEACOW(r)'s answer for Obsidian:**

- Use **folders** for the most common audience / perspective (the hierarchical constraint).
- Use **tags** for flexible, overlapping ontologies (graph-like flexibility).
- Use **links** and **MOCs** for specific relationships and bridging structures.
- Use **frontmatter / properties** for structured attributes.
- **Sync** between folders and tags to bridge the gap (the [Dynamic Tags & Folders plugin](../02-tools/plugins/dynamic-tags-folders/README.md)).

## The four primitives in Obsidian

(See [../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md](../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md) for the general decision matrix; this section is the Obsidian-specific instantiation.)

### Folders

- ✅ Required for file storage.
- ✅ Visual hierarchy in the file explorer.
- ✅ Good for primary audience / perspective.
- ❌ Single hierarchy (can't overlap).
- ❌ Inflexible (moving files is tedious).

### Tags

- ✅ Overlapping categories.
- ✅ Easy to add / remove.
- ✅ Multiple ontologies.
- ❌ Require full path for hierarchy.
- ❌ Don't scale well at huge scale (full-path duplication; see also [../02-tools/platform-notes/obsidian-tag-limitations.md](../02-tools/platform-notes/obsidian-tag-limitations.md)).

### Links

- ✅ True graph edges.
- ✅ Scales infinitely.
- ✅ Bidirectional awareness (Obsidian shows backlinks).
- ❌ Slow to create.
- ❌ Hard to visualize at scale.
- ❌ Requires active maintenance.

### Metadata (frontmatter / properties)

- ✅ Structured data.
- ✅ Queryable via Dataview.
- ✅ Type-safe (with property types).
- ❌ Not visible in the graph view by default.
- ❌ Requires manual input.

**Ideal combination:** use all four strategically.

- **Folders:** primary organizational axis (the *output* surface for your main Entity).
- **Tags:** secondary / tertiary axes, clustering.
- **Links:** specific relationships, MOCs.
- **Metadata:** structured attributes (status, dates, related entities).

## Tag prefix strategy

**Purpose:** control sorting and group related functionality.

**Common prefixes** (the cyberbase convention):

| Prefix | SEACOW(r) component | Example |
|---|---|---|
| `#--` (double dash) | Entity (people / teams) | `#--alice/projects/x` |
| `#-` (single dash) | Capture (inbox, clippings) | `#-clip/articles` |
| `#_` (underscore) | Output / public-facing | `#_public/docs/security` |
| `#/` (slash only) | System / template | `#/templates` |
| `#word` (no prefix) | Relation / keyword | `#malware`, `#concept` |

**ASCII sorting order:**

```
#-- (dash + dash)
#-  (single dash)
#/  (slash)
#_  (underscore)
#a  (letters)
#😀 (emoji — high Unicode)
```

For depth, see [../03-examples/cyberbase/tag-structure.md](../03-examples/cyberbase/tag-structure.md). For technical constraints (which characters Obsidian allows in tags, sorting collation), see [../02-tools/platform-notes/obsidian-tag-limitations.md](../02-tools/platform-notes/obsidian-tag-limitations.md).

## Folder organization principles

**High-level structuring** (from [../03-examples/cyberbase/vault-folder-and-tag-structure.md](../03-examples/cyberbase/vault-folder-and-tag-structure.md)):

- Design for the **primary Entity** (audience).
- Order by **LATCH:** Location, Alphabet, Time, Category, Hierarchy.
- Separate **workflow process** from **content ontology** — folders structure process, tags structure content.
- Use folders for **actionability** (e.g., the PARA method).

**Common approaches you'll see in Obsidian vaults:**

- PARA (Projects, Areas, Resources, Archive).
- ACE (Atlas, Calendar, Efforts).
- EJK (Efforts, Journal / Time, Knowledge).
- Workflow-based (Inbox, Processing, Output).
- D.E.E.Z.N.U.T.S. ([Reddit summary linked from knowledge-organization.md](../05-deep-dives/knowledge-organization.md)).

**Folder Notes** are an optional Obsidian pattern where folders have an
associated index note of the same name. Pros: show up in graph view, provide
navigation context. Cons: requires discipline to maintain.

## ARC-aligned tag and folder usage

**ARC** (Add → Relate → Communicate) — Nick Milo's PKM rhythm — maps cleanly
to SEACOW(r) Activities:

| ARC | SEACOW(r) | Tags | Folders |
|---|---|---|---|
| **Add** | Capture | `#-clip/`, `#-inbox` | Inbox folders, Daily Notes |
| **Relate** | Work + relation | `#keyword`, `#concept`, MOCs | Project folders, MOC folders |
| **Communicate** | Output | `#_public/docs/...` | Docs folders, publishing folders |

See [../03-examples/cyberbase/new-note-workflow.md](../03-examples/cyberbase/new-note-workflow.md) for the operational workflow.

## Obsidian-specific best practices

### 1. Start simple, scale up

- Don't over-engineer initially.
- Let structure emerge from use.
- Refactor incrementally.

### 2. Design for recall (LATCH)

- **L**ocation — where is it?
- **A**lphabet — what's it called?
- **T**ime — when was it created / relevant?
- **C**ategory — what type is it?
- **H**ierarchy — how does it relate?

### 3. Separate process from content

- Folders → workflow stages.
- Tags → content ontology.
- Don't duplicate unnecessarily.

### 4. Multiple perspectives

- Folders for primary audience.
- Tags for alternative views.
- Links for specific relationships.

### 5. Consistent naming

- Choose case convention (snake_case, Title Case, kebab-case).
- Stick to it within each system.
- Document your conventions.

### 6. Folder Notes (optional)

- Index folders with notes of the same name.
- Pros: show up in graph, provide context.
- Cons: requires discipline to maintain.

## Use cases & examples

### Example 1: cybersecurity vault

**Folders** (workflow-based):

```
01 - Inbox/
02 - Projects/
03 - Knowledge Base/
04 - Tools & Scripts/
05 - Archive/
```

**Tags** (content-based, SEACOW(r)):

```
#-clip/articles            (Capture)
#--cybersader/projects     (Entity + Work)
#_public/cyber/appsec      (Output)
#malware                   (Relation)
#/templates                (System)
```

### Example 2: personal knowledge management (PARA)

**Folders:**

```
Projects/
Areas/
Resources/
Archive/
```

**Tags:**

```
#active            (Status)
#idea              (Type)
#person/alice      (Entity)
#topic/ai          (Content)
```

### Example 3: academic research

**Folders** (subject-based):

```
Computer Science/
  Databases/
  AI & ML/
Mathematics/
  Statistics/
```

**Tags** (research process):

```
#to-read
#in-progress
#completed
#cite-in-paper
#research/database-theory
```

## Troubleshooting common issues

### "My tags are messy and unsorted"

→ See [../02-tools/platform-notes/obsidian-tag-limitations.md](../02-tools/platform-notes/obsidian-tag-limitations.md).
→ Use prefixes to control sorting.
→ Reference [../03-examples/cyberbase/tag-structure.md](../03-examples/cyberbase/tag-structure.md) for examples.

### "I can't decide between tags and folders"

→ See [../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md](../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md).
→ See [../05-deep-dives/choosing-a-tag-structure.md](../05-deep-dives/choosing-a-tag-structure.md).
→ Use both: folders for primary axis, tags for flexibility.

### "My tag structure doesn't scale"

→ See [../03-examples/cyberbase/vault-folder-and-tag-structure.md](../03-examples/cyberbase/vault-folder-and-tag-structure.md) (LATCH principles).
→ Apply SEACOW(r) constraints — particularly the gain-not-lose rule and Capture nesting limit.
→ Refactor incrementally, not all at once.

### "I want to migrate folder structures"

→ This is exactly what the [Dynamic Tags & Folders plugin](../02-tools/plugins/dynamic-tags-folders/README.md) solves.
→ Use transformation rules to maintain tag context while moving files.

## Resources

### Within this repo

- [01-framework/](../01-framework/) — the conceptual layer.
- [02-tools/](../02-tools/) — Obsidian tools, plugins, and platform notes.
- [03-examples/cyberbase/](../03-examples/cyberbase/) — cyberbase as the canonical worked Obsidian example.
- [05-deep-dives/](../05-deep-dives/) — long-form theory.

### External

- [Obsidian Help — Tags](https://help.obsidian.md/tags).
- [Obsidian Forum](https://forum.obsidian.md/).
- [cybersader/cyberbase](https://github.com/cybersader/cyberbase) — the public vault that uses this framework.
- [cybersader/obsidian-folder-tag-sync](https://github.com/cybersader/obsidian-folder-tag-sync) — the polyhierarchy plugin.
- [cybersader/awesome-obsidian-and-cyber](https://github.com/cybersader/awesome-obsidian-and-cyber) — curated Obsidian + cybersecurity resources.
