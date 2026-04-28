---
title: Open Questions
publish: true
---

# Open Questions

The single warm-zone of this otherwise-cooled repo. These are questions that
have been raised in cyberbase or elsewhere but haven't been resolved into a
deep-dive or a rule yet.

If you have an answer, sketch, or counter-question — open an issue or a PR.

## Framework structure

- **Is `r` (relation) a fundamental Activity or a sub-aspect of Work?**
  Argued both ways in [meta-framework.md](../01-framework/meta-framework.md).
  Lowercase-r is the current compromise. Worth resolving with a decisive worked example.
- **Should `r` be a Capture/Work bridge, an Output sub-component, or its own first-class concept?**
  Different worked examples treat it differently.
- **Activity stacking restrictions** — at what depth can the gain-not-lose rule break? See [rules.md](../01-framework/rules.md).

## Practical tagging

- Where do **untagged notes** go in a SEACOW(r)-organized vault? A consistent
  fallback location is needed but not yet specified.
- How should **folder notes** affect tag-folder mappings (especially in
  obsidian-folder-tag-sync)?
- **Plugin alignment** — most tag-related plugins use plain tags and don't
  allow appending things for structuring. How should rule-packs handle this?
- What's the **actual alphabetic order** Obsidian uses, and how do we make
  sorting rules portable across platforms (Obsidian / OS file explorer / sync clients)?

## Polyhierarchy & duplication

- Do you **duplicate ontologies under archives** or no?
- How do you avoid duplicating time-based content under archive-focused folders?

## Folder vs tag arbitration

- When two SEACOW(r) instantiations disagree (one uses folders for an
  Activity, another uses tags), is there a way to convert between them
  automatically? (Cf. [obsidian-folder-tag-sync](../02-tools/plugins/dynamic-tags-folders/README.md).)

## Missing comparisons

- The [vs-comparisons](../04-comparisons/) folder has stubs for PARA,
  Zettelkasten, Johnny Decimal, LATCH, ARCO/ACE/STIR. Need more depth, examples,
  and explicit "when to choose which" guidance.

## SEACOW(r) for AI agents

- Frameworks designed for human PKM rarely consider AI agents as Entities.
  How does the SEACOW(r) lens shift when a key Entity is a Claude Code or
  Cursor instance? See [../06-applications/claude-code-projects.md](../06-applications/claude-code-projects.md) (stub).

## Contributing answers

These should each grow into either:

- A new `05-deep-dives/<topic>.md` (when answered substantively), or
- A new rule in `01-framework/rules.md` (when answered as a constraint), or
- A `04-comparisons/<topic>.md` (when answered by comparison to another framework).

When you do split one out, remove it from this page and link to the new home.
