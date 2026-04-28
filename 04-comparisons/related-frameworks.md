---
title: Related frameworks (library science, DIKW, others)
publish: true
---

# Related frameworks

> [!note] Stub. PRs welcome.

A grab-bag of frameworks that show up in the SEACOW(r) conversation but
don't yet have their own dedicated comparison page.

## Library science (LCSH, UDC, Ranganathan, ontologies, folksonomies)

**What it is:** the corpus of techniques developed for organizing physical
and digital library collections — controlled vocabularies, subject heading
lists (LCSH), classification schemes (LCC, DDC, UDC), authority files
(LCNAF), thesauri, taxonomies, ontologies, and folksonomies.

**Mapping:** library science vocabularies are mostly an **Output layer** problem
— how do you make a corpus *findable* by a public audience? In SEACOW(r) terms,
they're tools for the Output and relation components when the Entity is
"public library patron." A folksonomy is a SEACOW(r) Output structure where
the rules are derived from user tagging behavior rather than authoritative
classification.

**See also:**

- [05-deep-dives/knowledge-organization.md](../05-deep-dives/knowledge-organization.md) — extensive references and types-of-controlled-vocabulary list.
- [Librarianship Studies: Controlled Vocabulary](https://www.librarianshipstudies.com/2020/03/controlled-vocabulary.html).
- [Library of Congress Subject Headings (LCSH)](https://id.loc.gov/authorities/subjects.html).

## DIKW pyramid

**What it is:** Data → Information → Knowledge → Wisdom — a hierarchy of abstraction levels.

**Mapping:** DIKW is **vertical** (a maturity / abstraction axis); SEACOW(r)
is **horizontal** (where content lives in a platform). They're orthogonal.
You can apply both: a piece of "data" can sit in your Capture layer; the
"information" derived from it sits in Work; the "knowledge" you publish from
it sits in Output. DIKW says **what something is**; SEACOW(r) says **where
it lives**.

## D.E.E.Z.N.U.T.S.

**What it is:** an opinionated 8-folder PKM scheme:

- **D** — Dashboards (or Maps of Content).
- **E** — Efforts (active work).
- **E** — Extras (Templates, Archive).
- **Z** — Zettelkasten (atomic ideas).
- **N** — Network & People.
- **U** — Unsorted / Unfinished (inbox).
- **T** — Thoughts & Journal.
- **S** — Sources (raw materials).

**Mapping:** a turn-key folder scheme. SEACOW(r)-wise:

| D.E.E.Z.N.U.T.S. | SEACOW(r) |
|---|---|
| Dashboards | relation + Output |
| Efforts | Work |
| Extras (Templates/Archive) | System / cooled |
| Zettelkasten | Work + relation |
| Network & People | Entity (people) + relation |
| Unsorted / Unfinished | Capture |
| Thoughts & Journal | Capture (chronological) |
| Sources | Capture (sourced material) |

**Choose it when** you want a prescriptive scheme; **choose SEACOW(r)** when
you want to design something for your own context rather than copy.

## PARAUT (PARA + Unstructured + Taxonomies)

**What it is:** a corporate variant of PARA:

1. Projects, Workspaces.
2. Areas, Initiatives.
3. Resources, Topics.
4. Archive, Admin.
5. Unstructured.
6. Taxonomies, Ontologies.

**Mapping:** like PARA but with explicit Capture (Unstructured) and explicit
relation (Taxonomies) layers. Closer to SEACOW(r) in spirit. See
[vs-para.md](vs-para.md) for the broader PARA comparison.

## ARC (Add, Relate, Communicate)

**What it is:** Nick Milo's PKM rhythm — a daily-practice cadence rather than a folder scheme.

**Mapping:** ARC maps cleanly onto SEACOW(r) Activities — Add → Capture +
Work; Relate → relation; Communicate → Output. ARC is a *rhythm*; SEACOW(r)
is a *structure*. They're complements. See
[01-framework/design-principles.md § ARC](../01-framework/design-principles.md#6-arc-add-relate-communicate).

## e-ACCESS

**What it is:** an extended PKM scheme — Encounters / Atlas / Calendar /
Cards / Extras / Sources / Spaces.

**Mapping:** see [05-deep-dives/ideas-for-knowledge-organization.md § e-ACCESS](../05-deep-dives/ideas-for-knowledge-organization.md).

## Want this list extended?

If you've encountered an organizational framework that should be compared to SEACOW(r), open an issue or submit a PR. Format: see [04-comparisons/README.md § Pull-request welcome](README.md#pull-request-welcome).
