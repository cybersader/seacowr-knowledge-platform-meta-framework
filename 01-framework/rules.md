---
title: SEACOW(r) Rule-Setting Language
publish: true
---

# SEACOW(r) rule-setting language

SEACOW(r) is a meta-framework — its main contribution isn't a folder layout,
it's a **vocabulary for writing organizational rules**. This page collects the
rule conventions used most often in real instantiations.

## What a SEACOW(r) rule looks like

A rule defines an allowed (or forbidden) relationship between SEACOW(r)
components and platform structures. Examples:

- *"Capture tags should be no more than two levels deep."*
- *"An Output sub-tree's children must all be Output (no Captures inside)."*
- *"Knowledge can gain SEACOW component contexts as you traverse down, but cannot lose them."*
- *"Each Output area must declare its target Entity in its index README."*

The vocabulary mixes **SEACOW(r) component names** with **system-structure
words** (nested, flat, depth, length, naming-scheme).

## Standard rules (used in cyberbase and similar instantiations)

### 1. Gain-not-lose (cascade) rule

> Knowledge can **gain** SEACOW(r) contexts / components as you traverse down
> some knowledge structure, but it can't **lose** them.

If a folder is marked `Capture+Work`, its child can be `Capture+Work+Output`
but typically shouldn't be just `Output`. This keeps the cascade legible —
readers know that a child inherits its parent's purposes plus possibly more.

### 2. Capture nesting limit

> Capture tags / folders should be kept to **at most two levels** of nesting.

Deep Capture hierarchies are usually Work in disguise. If you find yourself
nesting beyond two levels inside a Capture area, that's a signal that you're
doing categorization (Work), not capture.

### 3. Output can nest deeply

Unlike Capture, Output benefits from depth — it's audience-facing
navigation. Johnny Decimal–style numbering works here (`01-Projects/`,
`02-Tools/`, `03-Frameworks/`).

### 4. Output is strictly Output

Once content is inside an Output sub-tree, don't mix raw Captures into it.
The audience contract requires consistency. (You can have Captures *also* be
Outputs — but the Capture-as-Output then has to honor the Output contract.)

### 5. Relation tags stay flat

> Relation tags stay flat unless they map to an Output structure.

Unlike folders (which often need depth) or properties (which are flat by
nature), tags work best as a flat or 2-level vocabulary. Deeper tag
hierarchies tempt people to use tags as a second folder system, defeating
the polyhierarchy benefit.

### 6. Entity tags cascade

Entity context cascades down a hierarchy: a folder marked for a specific
Entity passes that Entity context to all children. Children may add Entities
but typically can't remove the parent's.

### 7. System tags identify, don't classify

Tags about the System itself (e.g. `system/dataview-query`,
`system/template`) should *identify* what kind of System artifact this is, not
classify content. Keep them flat and scarce.

## Activity-stacking restrictions (advanced)

A frequent advanced rule is to restrict which Activities can stack at a given
depth. For example:

- A pure Capture node can't have a pure Output child without an intermediate
  Work step (Capture → Work → Output is the natural pipeline).
- Restricting this prevents the "raw input shows up in published Output"
  failure mode.

These are not universal — they're rules SEACOW(r) asks you to *decide on* for
your context. The point of the meta-framework is that you *write* these rules
explicitly, in a vocabulary your future self and your collaborators (human or
AI) can read.

## Diagnostic questions when applying a rule

When a candidate piece of content doesn't fit cleanly:

1. **Is this raw input or processed?** → Capture vs Work
2. **Is this finished or in progress?** → Work vs Output
3. **Who is this for?** → Entity
4. **Does this support the system itself?** → System area
5. **How does this connect to other things?** → Relation layer

## Cross-references

- Component pages — [components/](components/)
- Cyberbase tag rules in detail: [../03-examples/cyberbase/tag-structure.md](../03-examples/cyberbase/tag-structure.md)
- Decision matrix on primitives: [../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md](../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md)
