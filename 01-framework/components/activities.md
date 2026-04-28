---
title: Activities (A) — SEACOW(r) component
publish: true
---

# Activities (A)

The umbrella for the three things that **happen to information**:

- [Capture (C)](capture.md) — where information *enters*
- [Work (W)](work.md) — where information is *processed*
- [Output (O)](output.md) — where information *exits* to a consumer

Plus a fourth, lower-case sub-component:

- [relation (r)](relation.md) — how things *connect*

## Why three core activities?

Engineers think in **inputs → function → outputs**. Knowledge platforms are no
different: information *enters* (Capture), gets *transformed* (Work), and
*leaves* for some consumer (Output). Naming these three ensures every piece of
your structure has a purpose tied to one of them.

## Why is `r` lowercase?

Relation is debated. One view: links/tags/MOCs are how you *do* knowledge Work,
so Relation is just a sub-aspect of Work. The other view: bridging structures
(MOCs, dataview, knowledge graphs) are distinct enough to deserve their own
component because they specifically *connect across* Captures, Works, and
Outputs without belonging to any of them.

The lowercase `r` is a deliberate signal: include it when it's load-bearing in
your design, drop it when Work suffices.

## The fundamental rule

The same item can serve **multiple Activities** at once — but ideally not in
ways that break consistency. A Clippings folder is mostly Capture, but it can
also serve as Output (a published "see what I'm reading" page) and Work (a
synthesis project pulls from it). When an item spans Activities, name the
spanning explicitly.

(See [rules.md](../rules.md) for the gain-not-lose rule and nesting limits.)

## Activity stacking and restrictions

A frequent advanced approach: **restrict how Activities can stack**. For
example:

- A pure Capture node can't have a pure Output child without an intermediate
  Work step.
- An Output sub-tree should stay Output (don't put raw Captures inside a
  finished Output area — they break the audience contract).
- Knowledge can **gain** Activities as you traverse down (a folder marked
  Capture+Work can have a Capture+Work+Output child) but typically can't *lose*
  them.

These aren't universal — they're the kind of rules SEACOW(r) asks you to
*decide on* for your context.

## Cross-references

- Per-component pages: [capture](capture.md), [output](output.md), [work](work.md), [relation](relation.md)
- Rule-setting language: [../rules.md](../rules.md)
- Real worked example of activity rules: [../../03-examples/cyberbase/tag-structure.md](../../03-examples/cyberbase/tag-structure.md)
