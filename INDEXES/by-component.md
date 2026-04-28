---
title: Index — by SEACOW(r) component
publish: true
---

# Index — by SEACOW(r) component

Slice the repo by which SEACOW(r) component each page primarily addresses.

| Letter | Component | Definition page | Deep-dive(s) | Worked example | Application |
|---|---|---|---|---|---|
| **S** | System | [components/system.md](../01-framework/components/system.md) | [folders-vs-tags-vs-links-vs-metadata.md](../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md) · [information-organization-systems.md](../05-deep-dives/information-organization-systems.md) | [cyberbase/folder-structure.md](../03-examples/cyberbase/folder-structure.md) | [02-tools/platform-notes/](../02-tools/platform-notes/) · [06-applications/](../06-applications/) |
| **E** | Entity | [components/entity.md](../01-framework/components/entity.md) | [choosing-a-tag-structure.md § 3](../05-deep-dives/choosing-a-tag-structure.md#3-applying-the-seacowr-meta-framework) | [cyberbase/tag-structure.md (`#--alice/...`)](../03-examples/cyberbase/tag-structure.md) | [obsidian.md](../06-applications/obsidian.md) · [corporate-fileshares.md](../06-applications/corporate-fileshares.md) |
| **A** | Activities | [components/activities.md](../01-framework/components/activities.md) | [rules.md](../01-framework/rules.md) | [cyberbase/](../03-examples/cyberbase/) (whole folder) | [obsidian.md § ARC](../06-applications/obsidian.md) |
| **C** | Capture | [components/capture.md](../01-framework/components/capture.md) | [ideas-for-knowledge-organization.md § Workspace](../05-deep-dives/ideas-for-knowledge-organization.md) | [cyberbase/folder-structure.md (`⬇️ Inbox`)](../03-examples/cyberbase/folder-structure.md) | [obsidian.md](../06-applications/obsidian.md) |
| **O** | Output | [components/output.md](../01-framework/components/output.md) | [choosing-a-tag-structure.md](../05-deep-dives/choosing-a-tag-structure.md) · [knowledge-organization.md](../05-deep-dives/knowledge-organization.md) | [cyberbase/folder-structure.md (`📁 01-06`)](../03-examples/cyberbase/folder-structure.md) | All `06-applications/` |
| **W** | Work | [components/work.md](../01-framework/components/work.md) | [knowledge-organization.md § Opinionated systems](../05-deep-dives/knowledge-organization.md) · [ideas-for-knowledge-organization.md](../05-deep-dives/ideas-for-knowledge-organization.md) | [cyberbase/new-note-workflow.md](../03-examples/cyberbase/new-note-workflow.md) | [claude-code-projects.md](../06-applications/claude-code-projects.md) |
| **r** | relation | [components/relation.md](../01-framework/components/relation.md) | [folders-vs-tags-vs-links-vs-metadata.md](../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md) · [combining-tags-links-folders.md](../05-deep-dives/combining-tags-links-folders.md) | [cyberbase/tag-structure.md (RELATION tags)](../03-examples/cyberbase/tag-structure.md) | [obsidian.md](../06-applications/obsidian.md) (MOCs, links, dataview) |

## Cross-component tooling

Some tools span multiple components:

- [obsidian-folder-tag-sync plugin](../02-tools/plugins/dynamic-tags-folders/README.md) — bridges Folder (S) ↔ Tag (System affordance for Capture/Output/Work/relation). The polyhierarchy enabler.
- [seacow-conventions skill](../02-tools/skills/seacow-conventions/SKILL.md) — applies the lens to all components.
- [seacow-scaffolder agent](../02-tools/agents/seacow-scaffolder.md) — uses the lens to design new structures.
