---
title: Obsidian Tag Limitations & Unicode Order
publish: true
permalink:
date created: Wednesday, March 19th 2025, 10:43 am
date modified: Wednesday, March 19th 2025, 10:52 am
source: cybersader/cyberbase — 📁 54 - Obsidian Vault Organization/Obsidian Tag Limitations & Unicode Order
---

# Obsidian tag limitations & Unicode order

This document captures the **nuances, limitations,** and **caveats** of Obsidian tags, focusing on special characters and how Obsidian sorts and parses tags. It also includes references to community feature requests and known workarounds.

---

## 1. Overview of tag constraints

- **Obsidian tags** must start with `#` and can contain **letters, numbers, underscores, and many Unicode characters.**
- They **cannot** contain spaces, commas, or the more "special" punctuation typical in Markdown (e.g., `@`, `.`, `?`, `:`).
- **Periods (`.`)** are particularly problematic because they break the tag at the period.
- **Slash `/`** is allowed but triggers **nested / hierarchical tags** in Obsidian's tag pane (e.g., `#food/fruits/apple` is a nested tag).

In other words, Obsidian "stops" parsing a tag once it encounters disallowed punctuation. Many of these design choices stem from wanting to avoid collisions with Markdown syntax and from how tags are typically parsed by other note-taking apps.

---

## 2. Why are certain characters disallowed?

1. **Markdown conflicts.** Characters like `@`, `:` and especially `.` or `\` can conflict with existing Markdown features (links, headings, image syntax, etc.).
2. **Parsing ambiguity.** Obsidian needs to know when a tag begins and ends. Allowing full punctuation can lead to tricky edge cases (e.g., `#some.tag` might appear like `#some` plus text `.tag`).
3. **Backward compatibility & ecosystem.** Some community plugins assume certain delimiters. Expanding the character set can break or complicate plugin code.
4. **User expectation (hashtag conventions).** Many "hashtag" systems do not allow a period or more exotic punctuation. So Obsidian's devs align with that general standard.

---

## 3. Supported vs. unsupported characters

### Commonly **supported** for tags

- Letters: `a–z`, `A–Z`.
- Numbers: `0–9`.
- Underscore: `_`.
- Hyphen: `-`.
- Slashes: `/` (for nested tags).
- Many **emojis** and extended **Unicode characters** are allowed.

### Commonly **not supported** for tags

- **Period** (`.`).
- **Colon** (`:`).
- **Semicolon** (`;`).
- **Comma** (`,`).
- **Question mark** (`?`).
- **Exclamation mark** (`!`).
- **At symbol** (`@`).
- **Reserved OS path characters** such as `\` on Windows.

> **Note:** the exact set of disallowed characters can be gleaned from Obsidian's parser. If Obsidian sees them as "end-of-tag" punctuation, the tag breaks there.

---

## 4. Workarounds for unsupported characters

Since "." and certain other punctuation are off-limits, the community and Obsidian support have recommended several **alternative approaches**. Pick whichever suits your workflow best.

### 4.1 Replace with Unicode "look-alikes"

If you truly **must** have an ampersand, slash, or period shape in your tag, you can use **fullwidth** or **Unicode** equivalents:

- For `&`: `＆` (U+FF06 Fullwidth Ampersand).
- For `.`: `．` (U+FF0E Fullwidth Full Stop).
- For `@`: `＠` (U+FF20 Fullwidth Commercial At).

Pros: visually similar to the ASCII character.
Cons: harder to type or remember; might cause confusion with search or plugin usage.

### 4.2 Nested tags instead of periods

Since a period is frequently used to **denote subcategories** (e.g., `#version.1.4.2`), you can replicate that nesting via slashes:

```
#version/1/4/2
```

Pros: Obsidian's **tag pane** gives you a nice hierarchy. Searching is straightforward: `tag:#version/1/4/2`.
Cons: each sub-level becomes its own nested tag. You can't treat `#version/1` and `#version/1/4` as exactly the same entity.

### 4.3 Use properties or frontmatter

If you need the notion of a semver or "tag with punctuation," you can instead use **YAML frontmatter** or the **Properties UI** in Obsidian:

```yaml
---
version: 1.4.2
category: my.software
---
```

Then query with [Dataview](https://github.com/blacksmithgu/obsidian-dataview) or the built-in Properties.
Pros: perfect for structured data (like versioning or DOIs).
Cons: not as convenient to filter in Obsidian's built-in **Tag Pane** — you'll need Dataview or advanced search.

### 4.4 Convert tags to note links

Another approach is to treat "tags" as **wiki links** to dedicated notes:

- Example: instead of `#g.skill`, you do `[[tag.g.skill]]`, a note titled `tag.g.skill.md`.
- You can store these "tag notes" in a `Tags` folder and then link to them anywhere.

Pros: you can use **any** punctuation in a filename that Windows / your OS allows (besides `\ / : * ? " < > |`). Great for extremely robust "tag pages" (like MOCs).
Cons: they no longer appear in the Tag Pane. Searching them is more like searching links.

### 4.5 Embrace hyphens and underscores

A simpler alternative is to just **replace periods** with `-` or `_`, e.g. `#version_1_4_2`.

Pros: easiest to remember / type (no Unicode look-alike). Plays nicely with typical coding or "snake-case" conventions.
Cons: visually less "semantic" if you specifically want a dot or slash.

---

## 5. Sorting & collation details

Obsidian sorts folders / files / tags using **Chromium's `Intl.Collator`** JavaScript API. This means:

- Sorting can differ slightly from **Windows File Explorer** or your OS's default.
- Unicode has extensive rules about accent marks, numeric sorting, etc.
- If you rely on a custom locale, you may see differences in alphabetical order.

### Key points on sorting

- Typically, numbers (`0–9`) are sorted before letters in ASCII-based ordering.
- Fullwidth characters may appear at unexpected positions.
- Slashes cause hierarchical grouping in the **tag pane** specifically (not purely alphabetical).

---

## 6. Examples of structured tag systems

1. **Nested approach (slashes):**
   - `#project/alpha`, `#project/beta`.
   - `#version/1/4/2` for semver references.
   - `#people/john_smith` for a person.
2. **Status approach (underscores):**
   - `#todo_open`, `#todo_inProgress`, `#todo_done`.
   - `#draft_wip`, `#draft_final`.
3. **Emoji prefixing:**
   - `#📌pin`, `#⚠urgent`, `#✨idea`.
   - Offers quick visual scanning in the tag pane.
4. **Hybrid:**
   - `#people/john_smith` + `#role_developer` + `#🚀growth`.
   - Combining nested tags, underscores, and emojis as needed.

---

## 7. References & forum discussions

1. **Official help docs** — Obsidian Tags help page.
2. **Feature requests:**
   - ["Support special characters (like `.`, `@`) in tags"](https://forum.obsidian.md/t/support-special-characters-in-tags-etc/71870)
   - "Request to allow periods for semver (`#v1.2.3`)"
3. **Sorting quirks:**
   - [File order in Obsidian different from Windows File Explorer](https://forum.obsidian.md/t/file-order-in-obsidian-different-from-windows-file-explorer/93480)
   - [Alphabetic sort depends on `Intl.Collator` (Chromium) locale settings](https://forum.obsidian.md/t/alphabetic-sort-order-should-be-dependent-on-system-input-language/11149)
4. **Community workarounds:**
   - Nested tags plugin: [obsidian-graph-nested-tags](https://github.com/drPilman/obsidian-graph-nested-tags).
   - Using frontmatter or Dataview properties for DOIs / semver.
   - Replacing `.` with `_` or `-`, or using fullwidth `．`.

---

## Conclusion

Because **Obsidian tags** are designed to remain compatible with standard hashtag conventions, many special punctuation characters (periods, `@`, `:`) are treated as the **end** of a tag. While this **limits** certain naming schemes (like `#v1.2.3`), the community has devised **several workarounds**:

- Use **slashes** for nesting.
- Swap special symbols with underscores or **fullwidth Unicode** equivalents.
- Store version / DOIs in **frontmatter** or **wiki links**.
- Adopt a more flexible approach to tag naming (snake_case, hyphen-case, etc.).

Ultimately, how you handle these constraints will depend on your **workflow**, **search habits**, and **automation** needs. This reference aims to clarify the **"why"** behind these limitations and to provide workable solutions so you can build an **efficient** and **sustainable** tag system in Obsidian.
