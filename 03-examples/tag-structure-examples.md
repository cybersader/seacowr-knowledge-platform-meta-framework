---
title: Tag Structure Examples
publish: true
permalink:
date created: Monday, March 17th 2025, 11:11 am
date modified: Wednesday, March 19th 2025, 12:49 pm
source: cybersader/cyberbase — 📁 54 - Obsidian Vault Organization/Tag Structure Examples
---

# Tag structure examples

Cross-references:

- [Cyberbase tag structure](cyberbase/tag-structure.md) — the canonical worked example.
- [Vault folder & tag structure (working notes)](cyberbase/vault-folder-and-tag-structure.md) — earlier brainstorm.
- [Folders vs tags vs links vs metadata](../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md) — when to choose which primitive.

> [!info] This is a work in progress. If you have better examples, contribute via PR — see [CONTRIBUTING.md](../CONTRIBUTING.md).

## My current tagging structure

> [!tldr] My tag structure uses my [SEACOW(r)](../01-framework/meta-framework.md) knowledge platform organization framework.

See [cyberbase/tag-structure.md](cyberbase/tag-structure.md) for the full implementation.

## Problems in tagging

A running list of unsolved or under-solved problems with tag-based organization
in Obsidian (and similar systems):

- **Folders ↔ tags** — formatting folder paths to snake-case nested tags. The
  [obsidian-folder-tag-sync](../02-tools/plugins/dynamic-tags-folders/README.md)
  plugin addresses this with regex transformation rules.
- **Where do untagged notes go?** A consistent fallback location is needed.
- **How do we move notes to certain folders based on parent tags with nested
  tags?** (Untagged go to an unstructured section.)
- **How do folder notes affect this?**
- **Most tag-related plugins use regular tags and don't allow appending
  things for structuring.**
- **What's the actual alphabetic order in this?** See
  [Obsidian tag limitations and unicode order](../02-tools/platform-notes/obsidian-tag-limitations.md).
