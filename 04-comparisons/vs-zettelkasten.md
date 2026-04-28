---
title: SEACOW(r) vs Zettelkasten
publish: true
---

# SEACOW(r) vs Zettelkasten

> [!note] Stub. PRs welcome.

## What Zettelkasten is

**Zettelkasten** (German for "slip-box"; Niklas Luhmann's method) is a
note-taking and thinking system built around two principles:

- **Atomic notes** — one idea per note, written in your own words.
- **Dense linking** — every note connects to others; the value emerges from the network of connections.

Notes live in a flat structure with unique IDs (originally numeric like
`12.4a3`); navigation is via links and structure-notes (MOCs).

## Mapping to SEACOW(r)

| Zettelkasten concept | Maps to SEACOW(r) component |
|---|---|
| **Atomic notes** | Work artifacts |
| **Fleeting notes** | Capture (raw, pre-atomic) |
| **Reference notes** | Capture (sourced material with citation) |
| **Permanent notes** | Work (atomic, written in your own words) |
| **Hub notes / MOCs** | relation (curated index notes) |
| **Links between notes** | relation (the graph layer) |
| **Unique IDs** | System affordance (Luhmann's filing scheme) |
| **No explicit Output layer** | (gap — Zettelkasten doesn't address Output) |

Zettelkasten is **Work + relation heavy** in SEACOW(r) terms. It deliberately downplays:

- **Entity** (it's a personal thinking system; no audience consideration).
- **Output** (Luhmann eventually published from his slip-box, but the slip-box itself isn't designed for audience consumption).
- **Capture** (handled, but informally — fleeting / reference notes).

The strength is the **relation** layer — Zettelkasten is one of the most rigorous treatments of how to make explicit, valuable connections.

## When to choose Zettelkasten

- **Research-driven** personal vault.
- You want to **think in connections**, not categories.
- Your output is **long-form synthesis** (papers, books, essays) — eventually pulled from the slip-box.
- You're willing to invest in the **discipline** of writing in your own words and linking densely.

## When to choose (or compose with) SEACOW(r)

- You need an **explicit Output layer** (a public wiki, deliverables, audience-facing pages).
- You have **multiple Entities** (collaborators with different views, AI agents reading the system).
- You need to **mix Capture-heavy work** (web clippings, project logs) with the slip-box discipline.
- Your platform's **System** affordances (tags, properties, dataview) deserve their own first-class treatment.

## Composition

Zettelkasten and SEACOW(r) compose nicely. Run Zettelkasten as the Work +
relation discipline and use SEACOW(r) to design the surrounding Capture and
Output layers:

```
your-vault/
├── 00-Inbox/                    (Capture — fleeting notes land here)
├── 01-References/               (Capture — sourced material)
├── 02-Slip-box/                 (Work — atomic permanent notes; dense links)
├── 03-MOCs/                     (relation — hub notes)
└── 04-Published/                (Output — synthesis pulled from the slip-box)
```

## See also

- [groepl/Obsidian-Zettelkasten-Starter-Kit](https://github.com/groepl/Obsidian-Zettelkasten-Starter-Kit).
- [groepl/Take-Useful-Notes](https://github.com/groepl/Take-Useful-Notes).
- [12 Principles for using Zettelkasten — Obsidian Forum](https://forum.obsidian.md/t/12-principles-for-using-zettelkasten/51679).
