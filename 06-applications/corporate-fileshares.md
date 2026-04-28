---
title: SEACOW(r) for corporate fileshares
publish: true
---

# SEACOW(r) for corporate fileshares

> [!note] Stub. PRs welcome — see [CONTRIBUTING.md](../CONTRIBUTING.md).

How to apply SEACOW(r) to a corporate file share (Windows SMB, SharePoint
document libraries, Google Drive shared drives, Dropbox Business). These
systems are **folder-only** — no tags, no wikilinks, no graph layer beyond
shortcuts and index files.

## File-share primitives

- **Folders** — the only organizational structure.
- **Permissions** — per-folder, sometimes per-file (often the strongest constraint).
- **File names** — sortable, searchable, but limited to OS naming rules.
- **Shortcuts / aliases** — pointers between locations (the closest thing to a graph layer).
- **Index files** (README.md, README.txt, _index.html) — by convention, navigation hubs.
- **Search** — usually full-text, but no structured query.

## Mapping SEACOW(r) → fileshare

| Component | Fileshare primitives |
|---|---|
| **System** | The fileshare itself + its permissions model |
| **Entity** | Permission groups; team folders; per-user home folders |
| **Capture** | `Drop/`, `Inbox/`, `Submissions/` folders with broad write permissions |
| **Work** | `Active/`, `WIP/`, `Drafts/` folders, often per-team |
| **Output** | `Shared/`, `Public/`, `Reports/`, `Client Deliverables/` folders with read-only perms |
| **relation** | Shortcuts; README index files; sometimes a wiki sidecar |

## Key constraints

- **Single hierarchy.** Polyhierarchy is impossible without symlinks / shortcuts. Use shortcuts deliberately for the most-needed cross-links; don't try to express every relation that way.
- **Permission boundaries are Entity boundaries.** Folder permissions naturally map to SEACOW(r) Entities — use this rather than fighting it.
- **No live tags.** Frontmatter / metadata exists in some systems (SharePoint columns, Google Drive labels) but is uneven across platforms.
- **Sorting matters.** Numbered prefixes (`01-`, `02-`) are the only reliable ordering primitive. Use them for Output sub-trees.

## Recommended starting pattern

```
00-Inbox/                    (Capture)
01-Active-Projects/          (Work)
02-Areas/                    (Work)
03-Resources/                (Work + light Output)
04-Shared/                   (Output)
05-Archive/                  (cooled Work)
99-Admin/                    (System)
```

With folder permissions:

- `00-Inbox/` — broad write, narrow read.
- `01-Active-Projects/` — team write, team+read.
- `04-Shared/` — narrow write, broad read.

## Open questions

- How to handle "this file belongs in two projects" cleanly (the classic polyhierarchy failure mode in fileshares).
- How to enforce naming conventions when the system has no schema.

Contributors: a worked example would be valuable. See [CONTRIBUTING.md](../CONTRIBUTING.md).
