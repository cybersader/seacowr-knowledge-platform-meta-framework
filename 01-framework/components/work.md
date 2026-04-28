---
title: Work (W) — SEACOW(r) component
publish: true
---

# Work (W)

**Question:** Where and how does information get PROCESSED?

> SEACOW(r) is **not prescribing** "you must have a `/Work/` folder." It's asking *where does active processing happen between Capture and Output?*

Work is the workshop. It's where you iterate, refine, synthesize, and turn raw
captures into something usable. Most of your time in a knowledge platform is
spent in Work; most of your structure decisions about *organizing for the
process* live here.

## Examples

| System | Work surfaces |
|---|---|
| Personal Obsidian vault | `Projects/`, `Zettelkasten/`, `Active/`, permanent notes, drafts |
| Corporate file share | `Teams/<name>/Active/`, `WIP/`, `Drafts/` |
| Code repo | `src/`, `tests/`, feature branches, `docs/drafts/` |
| Email | Flagged messages, project folders, drafts |
| Physical | Working files on desk, active project folders |

## Analysis: what to ask

- Where does **active processing** happen?
- What's the difference between **raw input** and **finished output**?
- Where do you **iterate, refine, synthesize**?
- What's **in progress** vs **done**?
- What's the **workspace** structure — by project? by area? by methodology (PARA, Zettelkasten, ARCO)?

## Work conventions

- **Work nesting should reflect process, not content** — if you nest by topic,
  you're really designing Output. If you nest by stage of work (`drafting/`,
  `reviewing/`, `archiving/`), you're designing for Process.
- **Work is the home of methodologies** — PARA, Zettelkasten, ACE, ARCO,
  Johnny Decimal — these are all *Work-area* methodologies for organizing the
  middle of the pipeline. SEACOW(r) sits one level above and helps you choose
  among them.
- **Work artifacts should track lifecycle** — frontmatter status fields
  (`draft / active / observed / stable / parked`) help distinguish work-in-progress
  from work-that-can-be-output.

## Work as the host of Relation

When `r` (relation) isn't given its own home, Relation lives in Work. MOCs,
dataview queries, link-tables — these are Work artifacts that bridge Captures
and Outputs.

## Work × Output transition

Moving content from Work to Output is the **publication event** — and it
should be deliberate. A common pattern:

1. Drafting in Work (`drafting/`).
2. Review pass (frontmatter `status: aligning`).
3. Promotion (move to Output sub-tree, status `stable`).

The transition can be a manual move, a frontmatter status change, or a Git
branch merge — depending on your System.

## Anti-patterns

- ❌ Work areas that grow infinite — set lifecycle conventions so things move
  to Output or Archive.
- ❌ Mixing Capture into Work without distinguishing — defeats the
  raw-vs-processed split.
- ❌ Building Work structures around topics instead of process — you'll end up
  with a fake Output area.

## Cross-references

- PARA / ARCO / Zettelkasten as Work methodologies: [../../04-comparisons/](../../04-comparisons/)
- The Relation question: [relation.md](relation.md)
- Cyberbase Work conventions: [../../03-examples/cyberbase/](../../03-examples/cyberbase/)
