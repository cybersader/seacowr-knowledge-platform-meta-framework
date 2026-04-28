---
title: Cyberbase New Note Workflow
publish: true
permalink:
date created: Thursday, March 20th 2025, 11:42 am
date modified: Saturday, March 22nd 2025, 6:46 pm
source: cybersader/cyberbase — 📁 54 - Obsidian Vault Organization/Cyberbase New Note Workflow
---

# Cyberbase new-note workflow

Operational workflow for creating new notes inside cyberbase, given the
[folder structure](folder-structure.md) and [tag structure](tag-structure.md).

This is one concrete instantiation of SEACOW(r): the **System** is Obsidian
plus QuickAdd / Templater / Modal Forms; the **Entity** is Cybersader;
**Capture / Output / Work** map to the folders and frontmatter conventions
used here.

## Plugin links (canonical references)

- [obsidian-modal-form (Daniel Espino)](https://github.com/danielo515/obsidian-modal-form) — define forms for filling data, callable from anywhere you can run JS.
  - [Modal Form docs](https://danielorodriguez.com/obsidian-modal-form/)
- [Getting rid of QuickAdd with Templater (Obsidian forum)](https://forum.obsidian.md/t/getting-rid-of-quickadd-with-templater/96161)
- [Modal form — integrate forms into QuickAdd (Obsidian forum)](https://forum.obsidian.md/t/new-plugin-modal-form-integrate-forms-into-quickadd-templater-etc/67103/108)
- [Templater snippets (Zach Young)](https://zachyoung.dev/posts/templater-snippets/)
- [Obsidian Modal Forms Plugin: How to transform your data entry (YouTube)](https://www.youtube.com/watch?v=zVGyWaw3xZQ)

## QuickAdd

- Docs — [Getting Started | QuickAdd](https://quickadd.obsidian.guide/docs/)
- Tutorial — *Paul Dickson — Obsidian QuickAdd Plugin: How to Create Better Notes in Seconds* (YouTube clipping in cyberbase).

### Community scripts, templates, macros

- [Clothesline Method with QuickAdd](https://github.com/zsviczian/obsidian-excalidraw-plugin/discussions/138)
- [QuickAdd examples](https://quickadd.obsidian.guide/docs/#be-inspired)
- [QuickAdd Tasks user guide (Obsidian Publish)](https://publish.obsidian.md/tasks/Other+Plugins/QuickAdd)

## My QuickAdd workflow

This is dependent on the [folder structure](folder-structure.md).

Automating new notes with QuickAdd templates:

- **Current folder** — useful when adding to one of the OUTPUT-type (public-facing) folders.
- **Specific folders:**
  - `🕸️ UNSTRUCTURED`
  - `⬇️ INBOX, DROPZONE`

### Folder Notes compatibility

- Automatically create folder notes.
  - This setting breaks the link-appending feature with QuickAdd.

### Using Modal Forms plugin to add tags during creation

- See cyberbase's "QuickAdd Tag Selector" QuickAdd script (in cyberbase System/QuickAdd Scripts/).

### Using current-note frontmatter with new note (QuickAdd + Templater + Modal Forms)

Doing this required QuickAdd, Templater, and Modal Forms.

The persist-tags template lives in cyberbase under `Templates/New Note - Persist Tags.md`.

Related discussion:

- [QuickAdd — using active file frontmatter (Obsidian forum)](https://forum.obsidian.md/t/quickadd-using-active-file-frontmatter/78091/6)
- [obsidian-modal-form #269](https://github.com/danielo515/obsidian-modal-form/issues/269)
- [Form builder API](https://danielorodriguez.com/obsidian-modal-form/FormBuilder/)
- [Inherit/pass on metadata values from active file when creating new file (forum)](https://forum.obsidian.md/t/inherit-or-pass-on-metadata-values-from-active-file-when-creating-new-file/60522)
- [How to pass data between QuickAdd and Templater?](https://github.com/chhoumann/quickadd/discussions/78)
- [How can I get the contents of an internally linked note (forum)](https://forum.obsidian.md/t/how-can-i-get-the-contents-of-an-internally-linked-note/97761/4)

## QuickAdd overview

> [!summary] QuickAdd is a combination of 4 tools (called "choices").

### 1) Templates

> [!tldr] Add new notes.

**Uses:**

- Create new notes.
- Use predefined templates.
- Keep folders organized.

**Works with:**

- Obsidian Templates.
- Templater plugin.

### 2) Capture

> [!tldr] Add new content to certain notes.

**Uses:**

- To files and folders.
- Insert format syntax.
- Insert before / after.

**Works with:**

- Active notes.
- New notes.

### 3) Macro

> [!tldr] Advanced automation.

**Uses:**

- Powerful tools.
- Sequence of commands.

**Works with:**

- Obsidian commands.
- Editor commands.
- User JS scripts.
- Choices.

### + Multi

> [!summary] A folder to organize Templates, Captures, and Macros.
