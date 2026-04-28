---
title: Dynamic Folders & Tags — Concept
aliases: [Automate Folders Based on Tags, Dynamic Folders Based on Tags, Dynamic Folders From Hierarchical Tags]
publish: true
permalink:
date created: Monday, March 17th 2025, 11:51 am
date modified: Monday, April 28th 2025, 12:27 pm
source: cybersader/cyberbase — 📁 54 - Obsidian Vault Organization/Dynamic Folders & Tags
---

# Dynamic Folders & Tags — concept

This is the **concept layer** behind the
[obsidian-folder-tag-sync plugin](https://github.com/cybersader/obsidian-folder-tag-sync) —
the underlying motivation and design rationale. For implementation details,
see the [plugin README](README.md).

## Related references

- *Plugin Development* — see cyberbase `📁 10 - My Obsidian Stack/`.
- *QuickAdd Tag Selector* — cyberbase `🕸️ UNSTRUCTURED/`. Select tags while adding new notes with QuickAdd.
- *Using Tags* — cyberbase `📁 10 - My Obsidian Stack/`.

## Related plugins

- **Automatic Tags plugin.**
- [adanielnoel/obsidian-index-notes](https://github.com/adanielnoel/obsidian-index-notes) — automatically generates index blocks based on tags.
- [farux/obsidian-auto-note-mover](https://github.com/farux/obsidian-auto-note-mover/tree/main).

## The core problem

Add a system that decides when to **dynamically move** something to a different folder based on tags. The system could have a priority structure or could even duplicate links or leave behind embedding versions in folders that they leave. This would help solve the problem of **strict hierarchies that you get with a hierarchical system like folders versus an emulated graph system** like overlapping tag paths or links (pretty much a graph-edge representation). Ultimately, the problem still becomes: **you need folders.**

## Make my own plugin?

Be awesome if I could say "anything the regex matches this in folder path gets a converted tag based on the path to snake case."

I want to create automatic tags based on folder paths in Obsidian so that the **folder hierarchy is represented in the tags**.

Okay. Let's build an Obsidian plugin that does this.

Could use a Dataview query at the top of the page, potentially — or the bottom with a template for it when it matches that regex I talked about.

## Problems in tagging this would address

- **Folders to tagging** — format to snake-case for folder path and make a nested tag.
- **Where do untagged go?**
- **How do we move to certain types of folders based on parent tags with nested tags?** (Untagged go to unstructured section.)
- **How do folder notes affect this?**
- **Most tag-related plugins will just use regular tags** and not allow appending things for structuring.
- **What's the actual alphabetic order in this?**

## Plugins that use or affect structure

- MyThesaurus.
- TagFolder.
- Tag Wrangler.
- Folder by tags distributor — doesn't handle unstructured notes other than sending them to root.
- Folder Notes.

## Manifesto

I'm trying to make a plugin that makes up for the **limited nature of hierarchical systems** for storage even though such things are necessary.

The idea is that I should be able to define matching for tag → folder and even folder → tag. This goes beyond even just a system like Auto Note Mover.

The core issue is that everything has to be stored in folders for the source. There's two ways we organize folders: **hierarchically** and **by names**. Therefore I should be able to define **regex matches that define the mapping from folder to tag or tag to folder.** That's step one. The regex lets us handle the naming part since we can use patterns with names to at least help us break out certain things as we transfer between. Simply doing snake-case may not be enough.

We may have a tag like `#projects/project1` but we actually want to store files with that tag under a path like `-/user_1/Projects/Project 1`. That's where regex and mapping those to a folder-path top-level can help. Either way, we need a **better language between the two** other than the exact matching that something like Auto Note Mover provides.

Time to address the second core requirement. Folders are fundamentally limited or flawed or not ideal because you have a strict hierarchy. To account for this, we can have a **priority mechanism** where certain tags or folders get hierarchy. Granted, tags can overlap, so this is really an issue for folders. For instance a folder may have `#unstructured` and `projects/project1` on it. This is where we would prioritize based on the tag classification or content or type of whatever fundamental way we can describe that. Then we could also prioritize to be more broad or more narrow such as if a note has `#projects` and `#projects/project1` in it.

## Core concepts

### 1) Dual mapping: folder ↔ tag

We need a way to represent these relationships with some syntax that accounts for the nested and hierarchical nature of tags or folders and allows you to define entry points at either side (tag or folder) into those ultimate hierarchies. For instance, you should be able to match up a tag like `project/project1` to some folder like `person1/project/project1`. The defined rules shouldn't need to have explicit perfect matches and should use some syntax, patterns like regex, or templating to make the configuration logic concise and intuitive.

However, fundamentally solving this problem is hard. We have to have both directions figured out and each logical piece has to work in both directions. There has to be mechanisms or logic to make sure the syntax is correct.

Transferring between the two seems to require a deterministic logic — so not AI-based. Snake-case and regex replacements are one option.

#### Tags to folder

A rule / definition line could have:

- **Tag regex** — to match or wildcard glob syntax. Typically you'll use this to match the start of a tag.
- **Tag-to-folder transformations:**
  - Case to certain folder naming — snake to spaces capitalized, etc. (the common default options).
  - Allow a regex replace per path level (separately for each folder in a depth in the path like `/parent/child`).
- **Folder-path entry point** — under what folder to establish matching transformed tags.
  - Allow a flatten setting with a depth value to flatten upwards (kind of like flattening objects).
  - Using regex groups for tag regex matches like `$1$2`?

#### Folder to tags

Certain Tag → Folder configs / rules will make matching up the directions difficult unless deterministic with specific case transformations by default. If that box is "ticked" then regex will have to likely be used in both directions.

The options will be similar to Tag → Folders:

- **Folder matching** with regex or glob for top level.
- **Folder transformations** with default case transformations along with custom regex-replace that can run at each path level.
- **Tag entry point.**

### 2) Customizable transformations

Using a custom piping syntax or designing one would probably be super hard so probably not a good idea. However, the stuff above with some defaults or regex is doable (one or the other likely).

### 3) Priority, logic, & overlapping hierarchies

- For priority we could just have the rules / definitions sorted like how Auto Note Mover does.
- Nesting and drop-down for organizing the rules could be helpful.
- Allow setting to prompt the user to move with button to ignore for future notes.
- Advanced settings for each rule line to allow for `key:value` settings like `ignore` or `ask user for prompt`.
- Option to retain / add conflicting tags on conflicts.
- Option to remove tag when moving from a folder (remove source-folder tag).
- Option to prompt for keeping or removing tags.
- Make tons of things as commands to allow for hotkeys and automation with other tools.
- Only run after leaving active file.
- Only run on save.
- Command to delete conflicting tags (in terms of lower priority).
- Options to favor broader or narrower tag paths (e.g. `project` vs `project/1`).

### 4) Handling special cases & additional features

- How to handle untagged notes.
- API that QuickAdd, Templater, or Modal Forms could somehow access — for instance to help decide where a new note can go.
- Handling for folder-note-based systems (move the folder). Use a function to look at the vault and figure out if you're using folder notes by looking at how many folder notes you have (folder matching note name). Would still need to account for attachments being stored adjacent to parent folder instead of in it (specific settings for this).
- Folder exclusions to ignore — allow regex here too.
- Ability to export settings as JSON or import them with copy-and-paste.

## See also

- [Plugin README](README.md) — implementation details.
- [folders-vs-tags-vs-links-vs-metadata](../../../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md) — why bridging matters.
- [combining-tags-links-folders](../../../05-deep-dives/combining-tags-links-folders.md) — composition strategies.
