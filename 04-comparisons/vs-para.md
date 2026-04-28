---
title: SEACOW(r) vs PARA
publish: true
---

# SEACOW(r) vs PARA

> [!note] Stub. PRs welcome.

## What PARA is

**PARA** (Tiago Forte, *Building a Second Brain*) — a four-folder scheme:

- **P**rojects — short-term efforts with a defined outcome.
- **A**reas — ongoing responsibilities (health, finances, household).
- **R**esources — topics of long-term interest.
- **A**rchive — inactive items.

The ordering principle is **actionability**: most-actionable on top, least at the bottom.

## Mapping to SEACOW(r)

| PARA | Maps to SEACOW(r) component |
|---|---|
| Projects | Work (with explicit Entity = current you, lifecycle-bounded) |
| Areas | Work (long-running, Entity = you-as-role) |
| Resources | mixed Capture + relation — raw inputs grouped by topic |
| Archive | cooled Work / cooled Output |

PARA is a **Work-area methodology** in SEACOW(r) terms. It doesn't speak directly to:

- **System** (it's platform-agnostic, but doesn't address platform constraints).
- **Entity** (assumes a single user; doesn't handle multi-audience cases).
- **Capture** (Resources is closest, but conflates Capture with Work).
- **Output** (no explicit audience-facing layer — your "published" stuff is just a folder among Resources or Areas).
- **relation** (no explicit graph / linking discipline).

## When to choose PARA

- You're a **single user** doing **personal knowledge management**.
- You want a **turn-key scheme** — start using it today, no design phase.
- Your work is mostly **action-driven** (projects with deadlines, ongoing areas of life).

## When to choose (or compose with) SEACOW(r)

- You have **multiple audiences** (yourself + team + public).
- You need a **distinct Output layer** (publishing, sharing, deliverables).
- Your platform has **non-folder primitives** (tags, properties, relations) that PARA's folder model doesn't exploit.
- You want to **evolve** your structure based on observation, not lock in a four-folder scheme.

## Composition

You can run PARA *inside* SEACOW(r): use PARA as the Work-area methodology and add SEACOW(r)-aware Output and Capture layers around it.

```
your-vault/
├── 00-Inbox/                    (Capture — addition to PARA)
├── 01-Projects/                 (PARA P → Work)
├── 02-Areas/                    (PARA A → Work)
├── 03-Resources/                (PARA R → Capture+Work — flagged for SEACOW review)
├── 04-Archive/                  (PARA A → cooled)
└── 05-Published/                (Output — addition to PARA)
```

## See also

- [01-framework/meta-framework.md § Isn't PARA enough?](../01-framework/meta-framework.md#isnt-para-enough)
- [PARA Starter Kit](https://fortelabs.com/) (external).
- [groepl/Take-Useful-Notes](https://github.com/groepl/Take-Useful-Notes) — Zettelkasten-flavored alternative for research-heavy work.
