---
title: SEACOW(r) vs LATCH
publish: true
---

# SEACOW(r) vs LATCH

> [!note] Stub. PRs welcome.

## What LATCH is

**LATCH** (Richard Saul Wurman, *Information Anxiety*) is the claim that
there are only **five fundamental ways to organize information**:

- **L**ocation
- **A**lphabet
- **T**ime
- **C**ategory
- **H**ierarchy (originally "Continuum")

Wurman's argument: every organizational scheme reduces to a combination of
these five primitives.

## Mapping to SEACOW(r) — they're orthogonal

LATCH and SEACOW(r) **don't compete** — they answer different questions.

- **SEACOW(r)** asks *what to organize* (System / Entity / Activities).
- **LATCH** asks *how to make it findable* (the retrieval / sort dimension).

You apply SEACOW(r) first to decide *what* sub-trees, tag-trees, or
property-schemas you need; you apply LATCH within each sub-tree to decide
how the items inside are sorted and findable.

| LATCH primitive | SEACOW(r) layer it most affects |
|---|---|
| **Location** | System (where it lives in the platform) |
| **Alphabet** | Output (audience-facing sort) |
| **Time** | Capture, Work (chronological surfaces) |
| **Category** | Output, relation (taxonomic groupings) |
| **Hierarchy** | System constraint + Output structure |

## When to use LATCH

- You're optimizing **retrieval** of finished content.
- You're designing **navigation** within an Output sub-tree.
- You want a checklist: "have I considered all five sort dimensions?"

## When to use SEACOW(r)

- You're designing **what categories** of content exist (Capture vs Work vs Output).
- You're deciding **which platform primitives** to use (folders vs tags vs links vs properties).
- You're addressing **multiple audiences** with different navigation needs.

## Composition

The natural composition: **SEACOW(r) outside, LATCH inside.**

- Use SEACOW(r) to decide your top-level shape — what's Capture, what's Work, what's Output, who the Entities are, what the System affords.
- Within each Output sub-tree, apply LATCH to decide sorting: alphabetical for a glossary, chronological for a timeline, hierarchical for a taxonomy, by-location for a regional index, by-category for a topical grouping.

## Example: cyberbase's Output

The cyberbase Output folders (`📁 01-Projects`, `📁 02-CyberNews`, `📁 03-Curations`, `📁 04-Cyber & Digital Trust`, `📁 05-Organizational Cyber`, `📁 06-Learning, Notes`) use:

- **Hierarchy** (the numbering creates a fixed top-level order).
- **Category** (each number is a domain).
- Within each number, often **Alphabet** or **Time**.

This is LATCH applied *inside* the Output layer that SEACOW(r) put there.

## See also

- [01-framework/design-principles.md § LATCH for retrieval](../01-framework/design-principles.md#5-latch-for-retrieval).
- [05-deep-dives/information-organization-systems.md](../05-deep-dives/information-organization-systems.md) — STIR / LATCH side-by-side.
- ["LATCH": Information Architecture from the Eyes of an Urban Indian User (Medium)](https://medium.com/@niveditachandra/latch-information-architecture-from-the-eyes-of-an-urban-indian-user-efd474a7bb37).
