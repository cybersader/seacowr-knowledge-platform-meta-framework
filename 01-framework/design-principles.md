---
title: SEACOW(r) Design Principles
publish: true
---

# SEACOW(r) design principles

Cross-cutting principles that aren't specific to one component. Read these
after the [meta-framework](meta-framework.md) and the [components/](components/)
pages.

> **Note:** sections of this page are populated as part of the migration of cyberbase's
> `📁 54 - Obsidian Vault Organization/.claude/CLAUDE.md` and
> `KNOWLEDGE_BASE_PHILOSOPHY.md`. Migration commit: see `01-framework: split and
> redistribute cyberbase CLAUDE.md` in the log.

## Start with purpose and audience

Every structural decision should trace back to an answer to *why are you
organizing this?* and *who is it for?* Without these answers, you're guessing.
This is the same opening move described in the [meta-framework](meta-framework.md);
it bears repeating because it's the principle people skip.

## Separate process from content

Folders should structure your **knowledge work process**, not your content.
Tags, links, and properties structure your **content**. This is from the cyberbase
[Vault Folder & Tag Structure](../03-examples/cyberbase/vault-folder-and-tag-structure.md)
notes. The single most important application: don't build deep folder
hierarchies for topics — that's what tags / properties / links are for.

## Polyhierarchy is the norm, not the exception

Most knowledge has multiple parents. A note about "encryption in healthcare"
belongs under both `Cybersecurity` and `Healthcare`. Folder systems force you
to pick one parent; tag and link systems let you have many. SEACOW(r) is
neutral about which primitive you use — but it expects you to make the
poly-hierarchy decision *deliberately* in light of System constraints.

The [obsidian-folder-tag-sync](https://github.com/cybersader/obsidian-folder-tag-sync)
plugin solves this for the Obsidian System; see [../02-tools/plugins/dynamic-tags-folders/concept.md](../02-tools/plugins/dynamic-tags-folders/concept.md).

## LATCH for retrieval

Once content exists, retrieval is the second-half of the organization problem.
[LATCH](../04-comparisons/vs-latch.md) (Wurman: Location, Alphabet, Time,
Category, Hierarchy) is a useful pairing — SEACOW(r) decides *what to organize*,
LATCH decides *how to make it findable*. They compose; they don't compete.

## ARC: Add, Relate, Communicate

Nick Milo's ARC (Add → Relate → Communicate) is a Work-area rhythm that maps
naturally to SEACOW(r): **Add** is Capture+Work, **Relate** is the Relation
layer, **Communicate** is Output. ARC is a useful daily-practice rhythm; SEACOW(r)
is the structural lens.

## The temperature gradient (when used)

Some applications of SEACOW(r) use a temperature-gradient pacing model:

```
hot  → 00-inbox/        (raw captures, session notes)
       01-working/      (active synthesis)
       02-learnings/    (patterns extracted)
       03-reference/    (cool reference material)
cold → 04-archive/      (frozen, Johnny Decimal by domain)
```

Content moves from hot to cold over time. This is a *Work-area* pacing
discipline — it lives inside the Work component, not as a top-level layer.
Use it when you have multi-session persistence and want to track maturity. The
[knowledge-curator](../02-tools/skills/seacow-conventions/SKILL.md) skill (and
its sibling skill in the same workflow) is the AI-side enforcement layer.

## The KB-as-the-project's-brain principle (from cyberbase)

A philosophical principle from cyberbase: a project's knowledge base **is**
the project — not documentation written after the fact, but the live working
memory of the project. AI agents should:

- **Read** the KB before starting work.
- **Update** the KB as new information is learned.
- **Create new files** for new topics rather than dumping in chat or PR comments.
- **Link** between related files.

This makes the KB a first-class artifact and makes future sessions (human or
AI) able to pick up cold.

## Cross-references

- Meta-framework: [meta-framework.md](meta-framework.md)
- Rules: [rules.md](rules.md)
- Choosing among primitives: [../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md](../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md)
- LATCH: [../04-comparisons/vs-latch.md](../04-comparisons/vs-latch.md)
