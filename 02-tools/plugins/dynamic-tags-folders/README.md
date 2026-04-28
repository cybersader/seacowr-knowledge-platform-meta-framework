---
title: Dynamic Tags & Folders Plugin Development
publish: true
permalink:
date created: Sunday, March 23rd 2025, 2:20 pm
date modified: Monday, April 28th 2025, 1:21 pm
source: cybersader/cyberbase — 📁 54 - Obsidian Vault Organization/Dynamic Tags & Folders Plugin Development
upstream: https://github.com/cybersader/obsidian-folder-tag-sync
---

# Dynamic Tags & Folders Plugin

The plugin lives at [cybersader/obsidian-folder-tag-sync](https://github.com/cybersader/obsidian-folder-tag-sync). This page documents the plugin's design intent, philosophy, and the SEACOW(r)-driven motivation behind it. For the **concept layer** (motivation in plain prose) see [concept.md](concept.md).

## 1) Naming & concept

Working names:

- Dynamic Tags & Folders.
- Dynamic Tag & Folder Mapper.
- Tag & Folder Mapper.

Description keywords:

- Path-based tagging.
- Automatic tagging.
- Organization.
- Combining the use of tags and folders.
- **Polyhierarchy.**

The idea is to have a **bidirectional** system where you can define rules to translate a folder path (e.g. `person1/Projects/Project 1`) into a tag (e.g. `#projects/project1`) and vice versa.

**Key points:**

- **Dual mapping:**
  - **Folder → Tag:** convert folder names into tags using regex patterns and transformation templates.
  - **Tag → Folder:** use similar rules in reverse, letting you determine where a note should live based on its tags.
- **Transformation flexibility:** beyond simple snake-case conversion, allow regex-based replacements and templating (e.g., using `$1` for captured groups) so users can handle variations in naming conventions.
- **Priority & conflict handling:** when rules overlap (a note may belong to multiple folders / tags), let users set priorities so the most specific or preferred rule "wins." You can also offer options like prompting the user or preserving multiple tags.
- **Additional features:** consider special cases such as handling untagged notes, folder notes (where a folder might have an associated note), and exclusions using regex or glob patterns.

### The philosophy

> So I have this dream of improving how we interface with technology in a personal way, or maybe in just a more interesting way. Here's the gist. As humans we don't have perfect intellect and our memory is limited. As we go through life we have to put faith in what we've already done — but in something higher as well. Now I know you may not believe in religion or rendering to God what He is due, but this does kind of inform my approach with technology. Here's the gist. In order to use technology and interface with it, we have to communicate with it — a lot, and with high volume. Most interfaces with certain applications have limits in how you can interface with that solution and that makes sense because it's supposed to solve only a certain problem. However, often most of the work takes place in our minds and in our hearts. That's where we have to live with our rather limited memory and ability to see backwards far enough with every decision we make at any point in time, and we have to align technology with our cornerstones / stakes / flags that we put down.

> With AI now, it requires a lot of data. The truth of the matter is that most of our interactions, sentiments, and our points of view — our ontologies, so to speak; maybe ontology configurations, or how we see the world / how we see reality — isn't communicated perfectly. That's because we can't communicate with technology in a perfect way. We are limited by how fast we can speak, how fast we can type, and how we can organize that information. My idea is that part of this can be improved in a manual sense — even though we still have to type — by making an environment where doing knowledge work is much easier, because that's the bulk of our work.

> Obsidian is a good tool right now for that. When we say "taking notes" it's a bit limited what we're talking about. We want to **capture** our knowledge and what that looks like, and then we want to allow it to be interfaced with other systems or people such as entities — or maybe even AI. Obsidian is a great way to do that, and it can grow with you and not be limited as a lot of other systems are.

> However one of the big problems is **how we represent knowledge in this form**. We are often limited by the file and folder system structures that operating systems use, and this is the same system that Obsidian uses in the background. I've tried to think of ways to represent knowledge better and in a flexible manner — to where there's tons of different ways to look at it, tons of different lenses, and we're not limited by just files and folders. Because that's not an accurate way to depict knowledge and communicate it.

> Libraries try to do this because they're literally limited by physical space, and a person has to walk down in a sequential manner to navigate it. This is why we have **information retrieval systems, taxonomies, and vocabulary** — things to structure a library. They even have **folksonomies** which are made to communicate to specific entities or audiences. My idea is that if we use knowledge platforms like Obsidian to their fullest, then we can communicate our knowledge and make it really consumable, really functional, and really useful to all sorts of entities. Then we're not limited by our memory but only by how much we can communicate to technology.

> In the future you'll have things like Neuralink which can speed this communication up — but even then there's a lot of limitations currently. So one of the things I'm doing is **building bridges between the different system components that are used to structure knowledge platforms and information**. This is essentially information science at this point.

> So in Obsidian you have different things that you can use to structure that knowledge and make it useful for **knowledge work**, useful for **knowledge capture**, and useful for **output** — to certain audiences for information retrieval or consuming. We have several different functions or tools that can be used on these knowledge platforms. These are **tags, folders, and links**. These are all interrelated, but what I'm trying to do is align these systems to the realities of knowledge work and knowledge communication and knowledge sharing.

> Since files and folders are the most limiting part of this system, I typically structure these based on who's going to be interfacing with things like the file explorer or looking at the folder structure. The beauty of tags is that you can have nested tags which show hierarchy. Now typically we have to have a full path for the tag in order to represent a hierarchy and that doesn't scale well in a super-large system. And even if we represent pieces of hierarchies, then we can't have the same word used in every place — or else it starts to duplicate. So that is one issue with tags that doesn't scale to a huge huge scale. However, links can scale really large but they're slow to input and hard to actually build up. In other words, the relating part of this with links takes a long time, because you have to draw each graph essentially. You could use AI that is really smart to help you do this and you could maybe approve connections — but something hasn't been designed like this yet. In the short term I would like to build a dynamic folder and tag syncing plugin — but that'll take a bit.

### Additional context

I'm trying to make a plugin that makes up for the limited nature of hierarchical systems for storage even though such things are necessary. The idea is that I should be able to define matching for tag-to-folder and even folder-to-tag. So this goes beyond even just a system like Auto Note Mover. The core issue is that everything has to be stored in folders for the source.

There's two ways we organize folders: hierarchically and by names. Therefore I should be able to define regex matches that define the mapping from folder to tag or tag to folder. That's step one. The regex lets us handle the naming part since we can use patterns with names to at least help us break out certain things as we transfer between. Simply doing snake-case may not be enough.

We may have a tag like `#projects/project1` but we actually want to store files with that tag under a path like `-/user_1/Projects/Project 1`. That's where regex and mapping those to a folder-path top-level can help. Either way, we need a better language between the two other than the exact matching that something like Auto Note Mover provides.

Time to address the second core requirement: folders are fundamentally limited / flawed / not ideal because you have a strict hierarchy. To account for this, we can have a priority mechanism where certain tags or folders get hierarchy. Granted, tags can overlap, so this is really an issue for folders. For instance a folder may have `#unstructured` and `projects/project1` on it. This is where we would prioritize based on the tag classification or content or type of whatever fundamental way we can describe that. Then we could also prioritize to be more broad or more narrow — e.g. if a note has `#projects` and `#projects/project1` in it.

Add a system that decides when to dynamically move something to a different folder based on tags. The system could have a priority structure or could even duplicate links or leave behind embedding versions in folders that they leave. This would help solve the problem of strict hierarchies that you get with a hierarchical system like folders versus an emulated graph system like overlapping tag paths or links (pretty much a graph-edge representation). Ultimately, the problem still becomes: you need folders.

## 2) Core concepts

### 1) Dual mapping: folder ↔ tag

We need a way to represent these relationships with some syntax that accounts for the nested and hierarchical nature of tags or folders, and allows you to define entry points at either side (tag or folder) into those ultimate hierarchies. For instance, you should be able to match up a tag like `project/project1` to some folder like `person1/project/project1`. The defined rules shouldn't need to have explicit perfect matches and should use some syntax, patterns like regex, or templating to make the configuration logic concise and intuitive.

Solving this problem fundamentally is hard. We have to have both directions figured out and each logical piece has to work in both directions. There has to be mechanisms or logic to make sure the syntax is correct.

Transferring between the two seems to require a deterministic logic — so not AI-based. Snake-case and regex replacements are one option.

#### Tags to folder

A rule / definition line could have:

- Tag regex — to match or wildcard glob syntax. Typically used at the start of a tag.
- Tag-to-folder transformations:
  - Case to certain folder naming — snake to spaces capitalized, etc. (default options).
  - Allow a regex replace per path level (separately for each folder in a depth like `/parent/child`).
- Folder-path entry point — under what folder to establish matching transformed tags.
  - Allow a flatten setting with a depth value to flatten upwards.
  - Using regex groups for tag-regex matches like `$1$2`.

#### Folder to tags

Certain Tag-to-Folder configs / rules will make matching up the directions difficult unless deterministic with specific case transformations by default. If that box is ticked then regex will likely have to be used in both directions.

Options similar to Tag-to-Folders:

- Folder matching with regex or glob for top level.
- Folder transformations with default case transformations along with custom regex-replace that can run at each path level.
- Tag entry point.

### 2) Customizable transformations

Using a custom piping syntax or designing one would probably be super hard, so probably not a good idea. However, the stuff above with some defaults or regex is doable (one or the other likely).

### 3) Priority, logic, & overlapping hierarchies

- For priority, we could just have the rules / definitions sorted like Auto Note Mover does.
- Nesting and drop-down for organizing the rules could be helpful.
- Allow setting to prompt the user to move (with a button to ignore for future notes).
- Advanced settings for each rule line to allow `key:value` settings like `ignore` or `ask user`.
- Option to retain / add conflicting tags on conflicts.
- Option to remove tag when moving from a folder (remove source-folder tag).
- Option to prompt for keeping or removing tags.
- Make tons of things as commands to allow hotkeys and automation with other tools.
- Only run after leaving active file.
- Only run on save.
- Command to delete conflicting tags (lower priority).
- Options to favor broader or narrower tag paths (e.g. `project` vs `project/1`).

### 4) Handling special cases & additional features

- How to handle untagged notes.
- API that QuickAdd, Templater, or Modal Forms could access — for instance, to help decide where a new note can go.
- Handling for folder-note-based systems (move the folder). Use a function to look at the vault and figure out if you're using folder notes by counting folder notes (folder matching note name). Would still need to account for attachments being stored adjacent to parent folder instead of in it.
- Folder exclusions to ignore — allow regex here too.
- Ability to export settings as JSON or import them with copy-and-paste.

## 3) Related existing plugins

### Combining tags and folders / notes

- [d7sd6u/obsidian-lazy-cached-vault-load](https://github.com/d7sd6u/obsidian-lazy-cached-vault-load) — fast loading + folder-index notes + ftags.
- [farux/obsidian-auto-note-mover](https://github.com/farux/obsidian-auto-note-mover).
- [al0cam/AutoMover](https://github.com/al0cam/AutoMover).

### Combining tags and links

- [Tag Wrangler — Rename](https://www.obsidianstats.com/plugins/tag-wrangler) — can allow you to represent tags as notes then link to them, but doesn't scale well.

### Combining folders and links (e.g. MOCs, ToCs)

- **Waypoint plugins:**
  - [IdreesInc/Waypoint](https://github.com/IdreesInc/Waypoint) — generate dynamic MOCs in folder notes; folders show up in graph view; removes need for messy tags.
- **Folder Notes:**
  - [LostPaul/obsidian-folder-notes](https://github.com/LostPaul/obsidian-folder-notes) — create notes within folders that can be accessed without collapsing the folder.

## 4) README requirements (for the plugin repo)

The plugin repo's README.md should show:

- Architecture of the code.
- Logical flow of components.
- Modeling of the components.
- How to get started.
- How to contribute.
