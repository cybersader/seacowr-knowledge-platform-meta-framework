---
title: Choosing a Tag Structure
aliases: [Choosing a Tag Structure in Obsidian]
publish: true
permalink:
date created: Wednesday, March 19th 2025, 11:04 am
date modified: Wednesday, March 19th 2025, 11:45 am
source: cybersader/cyberbase — 📁 54 - Obsidian Vault Organization/Choosing a Tag Structure in Obsidian
---

# Choosing a tag structure

> Originally written for Obsidian, but the principles generalize. Where the
> page calls out Obsidian-specific quirks, treat them as platform-specific
> instances of the general SEACOW(r) **System** consideration.

## 1. Introduction

Obsidian tags provide a **flexible** way to group notes across multiple folders and contexts, creating **overlapping ontologies** impossible with a strict folder hierarchy alone. However, Obsidian has **some limitations** (e.g., disallowing periods in tags), and certain **Unicode-based** tagging conventions can be slower to type — particularly on Windows.

Meanwhile, frameworks like **SEA(COWr)** can guide us to build **purposeful** structures — without necessarily *forcing* "SEA," "COW," or "RELATION" directly into the tag names. Instead, we use SEA(COWr) to define rules about **what** goes into tags and **how** they serve the knowledge system.

---

## 2. Why collation and sorting matter

### 2.1 The fundamental nature of sorting

On a **fundamental** level, all knowledge platforms must apply **some** kind of sorting or collation to strings (filenames, tags, etc.). Typically:

- **ASCII-based** sorting: Special characters (e.g., `!`, `#`, `-`, `_`) come before alphanumeric characters.
- **Unicode** sorting: Emojis and fullwidth characters often have code points that place them in different "blocks," which can cause them to appear *before* or *after* typical ASCII letters — depending on the environment.
- **Obsidian** uses the underlying **Chromium / Electron** collation approach, which might not match the OS file explorer exactly.

### 2.2 Taking advantage of sorting

Because these systems generally treat certain characters as "less" or "more" than letters, you can leverage that to **structure** your tag listing:

- **Underscores (`_`)** typically appear before letters in ASCII.
- **Hyphens (`-`)** often appear in a slightly different position.
- **Emojis** might come even *earlier* or *later* in the sorted list, depending on the environment.
- If you repeat certain characters (`--` or `___`), you can force them to appear at a certain order or to group them distinctly.

By understanding these fundamentals, you can create systematic, predictable "clusters" of tags that appear in specific segments of the Tag Pane or in alphabetical auto-completion lists. This is how you create a practical and powerful tagging system.

---

## 3. Applying the SEA(COWr) meta-framework

### 3.1 Quick recap of SEA(COWr)

**SEA(COWr)** is a conceptual approach to ensure you address:

1. **S**ystem — the environment or platform constraints (e.g., sorting, plugin compatibility).
2. **E**ntity — audience or user context (personal vs. team vs. public).
3. **A**ctivities — the core knowledge operations:
   - **C**apture
   - **O**utput
   - **W**ork
   - **(r)**elation (debatably could be nested under "Work").

> [!important] You don't literally name your tags with SEACOW(r) components. Instead, you define **rules** that involve each concept — like what naming schemes and knowledge-platform structures are allowed with relations between capture, output, work, etc. **SEA(COWr)** is a **mental model** to ensure you address each knowledge activity in your system.

### 3.2 Using SEA(COWr) as *rules*, not a naming convention

> [!hint] When defining SEACOWr rules, refer often to knowledge-platform **structures** and **contexts**.

A frequent advanced approach is **restricting** how the knowledge activities can stack. For instance:

1. **"We can add, but not remove, certain SEA(COWr) conceptual components in deeper levels."**
   - E.g., you can't use one logical level of tagging for capturing and then go down and leave out the original purpose of capturing from it. If that structural space starts becoming a place for more than merely capturing, then it has lost its original purpose.
2. **"You can't do advanced 'Work' or 'Output' activities under a 'Capture' structure / context."**
   - So the tags (and sometimes folders) that start with a CAPTURE-related context *cannot* have sub-tags for Work or Output-related contexts such as `#clippings/youtube/science/aerospace`. Structuring like this counts as a form of knowledge WORK or knowledge OUTPUT (a consumable taxonomy).

The next section shows how that might look in practice.

---

## 4. Core considerations when choosing your tag strategy

1. **Ease of typing vs. visual aesthetic**
   - Typing special Unicode or emoji tags is *slower*, especially on Windows (requiring the emoji panel).
   - Some advanced or fancy tag symbols look great but can disrupt **flow** during quick note-taking.
2. **Plugin compatibility**
   - Many Obsidian plugins assume your tags are "regular words" with no periods, colons, or advanced punctuation.
   - If you rely on plugins (e.g., Tag Wrangler, Dataview queries for tags), "simple" tags (letters, underscores, hyphens) often work best.
3. **Clustering & overlapping ontologies**
   - One big reason to use tags is the ability to assign multiple categories to a note (e.g., `#science` and `#client_project`).
   - Even if you create advanced hierarchical tags (e.g., `#science/biology`), you can still overlap them with other tags in the same note.
4. **Auto-completion and alphabetical sorting**
   - Obsidian auto-completes tags in the editor. Clear, consistent naming improves your speed and reduces confusion.
   - Alphabetical sorting in the Tag Pane means you might want to standardize prefixes or group tags by category:
     - Example: `#cluster_science`, `#cluster_history`, `#cluster_biology`.

---

## 5. Advanced example: SEA(COWr) tag hierarchy

Below is an **example** of how you might label tags using **repeated dashes** or **underscores** to force sorting order, plus **slashed** subcategories. Notice how **Capture** tags come first in the ASCII sorting (due to `_` or `-` usage), while **Output** tags might be higher or lower, etc.

### 5.1 Example "Lego blocks" in a tag structure

1. **`_/`** — Unstructured or "general categories" (top-level personal clusters):
   - `#_/science`
   - `#_/philosophy`
   - `#_/unstructured/random`
2. **`-/`** — Next-level category for "other purposes" or "meta stuff":
   - `#-/meta`
   - `#-/dev` (for development).
3. **`--/`** — Another deeper prefix indicating "system-level" topics or rare categories:
   - `#--/system_config`
   - `#--/obsidian_plugins`

#### Why multiple dashes?

- Multiple dashes **push** these tags farther up or down in an alphabetical list. For instance, `--/` might appear before `-/` or after, depending on how your environment sorts double-dashes vs. single.

### 5.2 Tying in SEA(COWr) activities

Imagine you define these rules:

- CAPTURE-related structures or contexts cannot use WORK or OUTPUT below them.
- WORK-related structures cannot have CAPTURE-related structures below them.
- RELATION structures can be used to bridge Work and Capture.
- CAPTURE-related structures can only be 2 logical levels deep.

Then, within each major activity, you exploit sorting with underscores or repeated dashes.

---

## 6. Collation tricks & frequency

### 6.1 Emojis vs. ASCII

- **Emoji** code points can appear *before* or *after* ASCII. On many systems, `#📌foo` might jump to the top or bottom.
- Because it's **slower** to type emojis, you might only reserve them for **low-frequency** tags (like a special "rare" or "archival" category).

### 6.2 Repeated characters & sorting "blocks"

- If you prefix a tag with `_` or `-` multiple times (`--`, `---`) you create "groups" that forcibly appear in a consistent order.
- Example:
  - `#--myTag`
  - `#---myTag`
  - `#____something`
- You can treat these like "lego blocks" — the more dashes, the deeper or more specialized the category, ensuring it sorts either above or below single-dash items.

### 6.3 Leading numbers

- Leading numbers (e.g., `0_`, `1_`, `2_`) create a straightforward linear hierarchy. Combining them with underscores or dashes can result in a robust structure:
  - `#0_capture_inbox`
  - `#1_work_in_progress`
  - `#2_output_final`
- This is simpler than relying on ASCII codes for punctuation because numeric ordering is **predictable**.

---

## 7. Handling Unicode & typing speed

### 7.1 Keyboard shortcuts for emojis

- On Windows, press `Win + .` (period) to open the emoji keyboard.
  - Slow if you do it frequently.
- Consider a text-expander tool (like **AutoHotkey** or **Espanso**) so typing `:rocket:` becomes `🚀`.

### 7.2 Fullwidth Unicode substitutes

- If you absolutely need "@" or "." in tags:
  - Use fullwidth symbols (`＠` U+FF20 or `．` U+FF0E).
  - Keep a snippet or text macro for quick insertion.
- **But** ensure you're comfortable with potential plugin/compatibility quirks.

### 7.3 Hyphen or underscore over "fancy" Unicode

- Often simpler to do `#capture_inbox` or `#capture-inbox` than messing with "look-alike" punctuation.
- Consistency is key: pick one delimiter (`-` or `_`) and stay with it.

---

## 8. Plugin options & sequences

### 8.1 Tag Wrangler

- Helps rename or merge tags if your structure changes.
- If you add new categories or rearrange nested tags, Tag Wrangler can bulk-update references.

### 8.2 Nested tags (core functionality)

- Simply add slashes in the tag: `#main/sub/child`.
- The Tag Pane will show collapsible tiers.

### 8.3 Dataview

- If you rely heavily on advanced queries (like searching `#todo` across multiple vault areas), keep tags short and straightforward.
- Dataview can also parse **YAML frontmatter** — so if you can't use certain punctuation in tags, consider storing them as frontmatter fields.

---

## 9. Further "lego block" examples

Below are some condensed sample patterns you can mix and match. Each bullet is a "lego block" that you can use to build your own system.

1. **`#/words/stuff`** — slashes define nested tags.
2. **`#(number_or_emoji)_word_here/ontologies`** — like `#1_todo/urgent`, `#2_todo/low`, or `#🎨_art/abstract`.
3. **`#-/other_purpose`** — single-dash prefix for "less common" categories.
4. **`#--/yet_another_section`** — double-dash prefix for "deep system" or "rare" categories.
5. **`#_/unstructured`** — underscore prefix for capturing top-level unstructured items.

Choose whichever combination keeps your tags:

- **Intuitive** to you (and your team, if collaborative).
- **Consistent** so you can quickly type or filter them.
- **Well-sorted** in Obsidian's Tag Pane or auto-complete.

---

## 10. Example tag systems

Below are a few **practical** examples to illustrate final naming patterns that align with SEA(COWr) logic (without *literally* using "SEA" or "COW" in the tag).

### 10.1 Simple alphanumeric + underscore

- `#capture_inbox` — raw unprocessed notes.
- `#work_in_progress` — items actively being edited.
- `#output_final` — ready-to-share content.
- `#science`, `#philosophy` — general knowledge clusters.
- `#team_client` — indicates notes for client projects or shared with a client.

### 10.2 Nested slashes for some categories

- `#capture/inbox`
- `#work/todo` / `#work/review` / `#work/done`
- `#output/final`
- `#cluster/science` / `#cluster/biology` / `#cluster/ai`

### 10.3 Hybrid with emojis

- `#🔍research`
- `#🚧wip` (work in progress).
- `#📤final_output`
- `#🏷cluster_science` / `#🏷cluster_history`
- Possibly a "tag root" prefix like `#🏷` or `#📂` for cluster tags, if you want them to sort together.

### 10.4 SEA(COWr) advanced

*(see [Cyberbase tag structure](../03-examples/cyberbase/tag-structure.md) for the canonical worked example).*

---

## 11. Final thoughts

- **SEA(COWr)** helps clarify **why** you're labeling notes (Capture, Work, Output, etc.), guiding the *logic* behind your tag sets.
- **Tag naming** is about balancing:
  - Speed of **typing**.
  - **Readability** in the Tag Pane.
  - **Plugin** compatibility.
  - Potential **aesthetics** (like emojis).
- For large projects or teams, **consistency** in your tagging convention is more important than the exact choice of hyphen, underscore, or emoji. If multiple people edit notes, ensure everyone agrees on the same approach.
- Don't be afraid to revise your tags over time — tools like **Tag Wrangler** or even simple "Find and Replace" can help you restructure as your system evolves.

---

### Quick reference

1. **Keep tags simple** for broad clusters (`#science`, `#history`).
2. For more complex logic (versions, semver, advanced punctuation), consider **nested tags** (`#version/1/4/2`) or **properties** in YAML.
3. Decide whether **emojis** or **Unicode** are worth the typing cost.
4. Use a **framework** like SEA(COWr) to define guidelines about how tagging should be structured.
