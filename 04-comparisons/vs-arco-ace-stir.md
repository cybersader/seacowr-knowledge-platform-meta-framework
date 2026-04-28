---
title: SEACOW(r) vs ARCO / ACE / STIR
publish: true
---

# SEACOW(r) vs ARCO / ACE / STIR

> [!note] Stub. PRs welcome.

A cluster of process-based PKM frameworks that all live in roughly the same conceptual neighborhood. SEACOW(r) is **upstream** of all three — they're each Work-area methodologies that SEACOW(r) can subsume.

## ARCO

**ARCO** — book-metaphor framework:

- **A**tlas — book of maps (relations, MOCs).
- **R**eference — book of facts and external links.
- **C**alendar — book of events.
- **O**rganizer — book of tasks and projects.

Mapping:

| ARCO | SEACOW(r) |
|---|---|
| Atlas | relation (curated index notes) |
| Reference | Capture (sourced facts and links) |
| Calendar | Work (time-bounded artifacts) |
| Organizer | Work (action-bounded artifacts) |

## ACE

**ACE** — derived from STIR (see below):

- **A**tlas — for the *space* of knowledge and ideas.
- **C**alendar — for moments in *time*.
- **E**fforts — for projects of *importance*.

(The "R" in STIR — *relatedness* — becomes the *links* between ACE entries.)

Mapping:

| ACE | SEACOW(r) |
|---|---|
| Atlas | relation + Output (audience-facing maps) |
| Calendar | Work + relation (time-bounded) |
| Efforts | Work (project-bounded) |
| (Links between them) | relation |

## STIR

**STIR** — four ways to organize information:

- **S**pace
- **T**ime
- **I**mportance
- **R**elatedness

STIR is a retrieval / categorization framework, similar in spirit to LATCH.

Mapping: STIR is a **dimensions-of-organization** framework, like LATCH —
orthogonal to SEACOW(r). You use STIR (or LATCH) inside SEACOW(r)'s Output
layer to decide *how* to sort and find things.

## When to choose any of these

- You want a **prescriptive PKM rhythm** rather than a meta-lens.
- The book metaphor (Atlas / Reference / Calendar / Organizer) helps you think.
- You like the "Aha — STI maps to ACE" insight.

## When to choose (or compose with) SEACOW(r)

- You're designing for **multiple Entities** (not just personal PKM).
- You need **explicit Capture / Work / Output separation** (which these frameworks blur).
- Your platform's **System** affordances vary — SEACOW(r) is platform-agnostic.

## Composition

These compose under SEACOW(r) as Work-area methodologies. For example:

```
your-vault/
├── 00-Inbox/             (Capture)
├── 01-Atlas/             (relation — MOCs, dashboards)
├── 02-Reference/         (Capture / Work — facts, sources)
├── 03-Calendar/          (Work — time-bounded)
├── 04-Efforts/           (Work — projects)
└── 05-Published/         (Output)
```

## See also

- [The Ultimate Folder System: A quixotic journey to ACE — Obsidian Forum](https://forum.obsidian.md/t/the-ultimate-folder-system-a-quixotic-journey-to-ace/63483).
- [05-deep-dives/knowledge-organization.md § Opinionated systems for Obsidian](../05-deep-dives/knowledge-organization.md).
- [05-deep-dives/ideas-for-knowledge-organization.md](../05-deep-dives/ideas-for-knowledge-organization.md) — the e-ACCESS extended version.
