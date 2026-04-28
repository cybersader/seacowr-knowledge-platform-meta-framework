---
title: SEACOW(r) vs Johnny Decimal
publish: true
---

# SEACOW(r) vs Johnny Decimal

> [!note] Stub. PRs welcome.

## What Johnny Decimal is

**Johnny Decimal** is a numeric folder system:

- 10 **areas** at the top (10–19, 20–29, 30–39, …, 90–99).
- 10 **categories** per area (11, 12, 13, …, 19).
- 10 **IDs** per category (11.01, 11.02, …, 11.99).

The numbers force a deterministic file order and make every item
addressable by a stable ID (`11.04 — Project Apollo`). The system is rigid
on purpose: rigidity = predictability = retrieval.

## Mapping to SEACOW(r)

Johnny Decimal addresses **System** (platform discipline) and **Output**
(audience-facing retrieval). It doesn't speak to:

- **Entity** (single-user implied, though teams use it).
- **Activities** (no Capture / Work / Output split — everything just lives in the appropriate ID).
- **relation** (no graph layer — links are an add-on, not core).

| Johnny Decimal element | Maps to SEACOW(r) |
|---|---|
| Areas (10–19, 20–29) | Output / Work top-level partitions |
| Categories (11, 12, 13) | Sub-partitions |
| IDs (11.04) | Stable retrieval addresses (System affordance for findability) |
| The 10-of-each rule | Discipline / constraint (a System-level rule) |

## When to choose Johnny Decimal

- You're organizing a **bounded set of items** (your finances, your home filing cabinet, a corporate fileshare).
- You want **deterministic retrieval** above all else.
- You can **plan the partitioning up-front** (10 areas is enough; 100 categories is enough).

## When to choose (or compose with) SEACOW(r)

- You have **fluid, growing knowledge** that doesn't fit a fixed ten-bucket scheme.
- You need a **graph layer** (cross-references between disparate areas).
- You have **multiple audiences** with different views of the same content.
- You want to **distinguish raw input from finished output** (Johnny Decimal puts everything together, sorted by topic).

## Composition

Use Johnny Decimal as the **Output sub-tree's** retrieval scheme, with
SEACOW(r) governing the higher-level Capture / Work / Output split:

```
your-vault/
├── 00-Inbox/                    (Capture)
├── 01-Active/                   (Work)
├── 02-Output/                   (Output — JD-organized below)
│   ├── 10-19 - Knowledge Base/
│   │   ├── 11 - Frameworks/
│   │   ├── 12 - Research/
│   │   └── 13 - Tools/
│   ├── 20-29 - Projects/
│   └── 30-39 - …
└── 03-Archive/                  (cooled)
```

This is essentially what cyberbase does with `📁 01-Projects`, `📁 02-CyberNews`, `📁 03-Curations` — Johnny-Decimal-flavored numbering inside the Output layer. See [03-examples/cyberbase/folder-structure.md](../03-examples/cyberbase/folder-structure.md).

## See also

- [johnnydecimal.com](https://johnnydecimal.com/) — the canonical system.
- [johnnydecimal.com — concepts](https://johnnydecimal.com/10-19-concepts/11-core/11.01-introduction/).
