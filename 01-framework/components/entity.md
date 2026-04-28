---
title: Entity (E) — SEACOW(r) component
publish: true
---

# Entity (E)

**Question:** WHO accesses or interacts with this?

Entities create natural **boundaries**. They drive read-vs-write split, public-vs-private split, audience-specific Outputs, and the "what should this person see?" decisions that Capture and Output rely on.

## Examples

- Just you (personal knowledge base)
- Multiple teams (engineering, marketing, sales, security)
- Public audiences (blog readers, recruiters, customers)
- AI agents (Claude, Cursor, custom tools)
- Mix of internal + external stakeholders (clients + your own team)
- Future-you (not present-you) — a useful Entity for personal vaults

## Analysis: questions to ask

- Are there **read-only** vs **read-write** Entities?
- Do different Entities need **different views** of the same content?
- Are there **audience-specific Outputs** (recruiter resume vs technical resume)?
- Do Entities have **different Capture mechanisms** (clippings for you, submissions for the team)?
- Are Entities **anonymous** (public web visitors) or **identified** (named team members)?

## How Entity shapes the rest

| Entity boundary | Implication |
|---|---|
| Personal-only | Looser conventions; you can rely on memory and ad-hoc links |
| Team / collaborator | Conventions must be explicit; naming and ontology matter |
| Public audience | Outputs must self-explain; assume zero context |
| AI agent | Consistency for parsing; avoid metaphor-heavy structure |
| Mixed (you + public) | Two Output surfaces (your private working files + the published version) |

## Cascading Entities

When folder structures cascade, **child folders inherit Entity context** — and they can *gain* additional Entity context but typically can't *lose* it. A folder marked `team-only` shouldn't have a public child unless the structure makes the boundary explicit.

(See [rules.md](../rules.md) for the gain-not-lose convention.)

## Anti-patterns

- ❌ Designing for "everyone" — that's nobody. Pick named Entities.
- ❌ Forgetting that AI agents are Entities — they parse your structure, and inconsistent naming costs you.
- ❌ Conflating Entity with Output. *Audience* is a property of Output but the *Entity* concept also applies to Captures (who's submitting?) and Work (who's processing?).

## Cross-references

- Audience-driven Outputs: [output.md](output.md)
- Entity in cyberbase's instantiation: [../../03-examples/cyberbase/](../../03-examples/cyberbase/)
