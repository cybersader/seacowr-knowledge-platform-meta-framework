# SEACOW(r) Knowledge Platform Organization Meta-Framework

> A meta-framework / lens for designing knowledge organization in any platform.

SEACOW(r) is **not** a folder structure. It's a set of questions for analyzing
and designing organizational systems — Obsidian vaults, file shares, code repos,
Notion workspaces, even physical filing cabinets.

```
S — System         → What platform are we in? What does it afford?
E — Entity         → Who accesses this? What are the boundaries?
A — Activities
    C — Capture    → Where does information ENTER?
    O — Output     → Where does it EXIT to a consumer?
    W — Work       → Where does it get PROCESSED?
    r — relation   → How do things CONNECT? (graph layer)
```

Answer these for **your** context. Design a structure that fits. Don't copy
folder names — copy the thinking process.

---

## Start where you are

| You are… | Go here |
|---|---|
| New to SEACOW(r) | [00-start-here/](00-start-here/) — TL;DR, quick-start, glossary |
| Reading the theory | [01-framework/](01-framework/) — meta-framework, components, rules |
| Ready to apply it | [02-tools/](02-tools/) — skills, agents, plugins, platform notes |
| Looking for examples | [03-examples/](03-examples/) — cyberbase as a worked SEACOW(r) instance |
| Comparing to other systems | [04-comparisons/](04-comparisons/) — vs PARA / Zettelkasten / Johnny Decimal / LATCH |
| Going deep | [05-deep-dives/](05-deep-dives/) — long-form theory, decision matrices |
| Applying SEACOW(r) elsewhere | [06-applications/](06-applications/) — Obsidian, Notion, Claude Code, fileshares |

## Multiple ways in (different navigations of the same content)

- **[03-examples/framework-gallery.md](03-examples/framework-gallery.md)** — exhaustive side-by-side gallery of organizational frameworks with concrete folder/tag trees and SEACOW(r) mappings (PARA, PARAUT, BASB+CODE, Zettelkasten, FLAP, LYT/Ideaverse, evergreen-notes, ARC, ACE, STIR, ARCO, e-ACCESS, Johnny Decimal, LATCH, DIKW, LCC, LCSH, DDC, UDC, Ranganathan PMEST, controlled-vocab types, folksonomy, vault starters, cyber compliance frameworks, DEEZNUTS, EJK, and more).
- [INDEXES/by-audience.md](INDEXES/by-audience.md) — Newcomer / Practitioner / Architect lanes
- [INDEXES/by-component.md](INDEXES/by-component.md) — slice by S / E / A / C / O / W / r
- [INDEXES/by-task.md](INDEXES/by-task.md) — Learn / Design / Apply / Extend / Compare
- [INDEXES/by-depth.md](INDEXES/by-depth.md) — 60-sec / 5-min / 30-min reads
- [INDEXES/by-comparison.md](INDEXES/by-comparison.md) — SEACOW(r)-vs-X matrix (compact)

## What's in this repo

| Folder | Contains |
|---|---|
| `00-start-here/` | TL;DR, quick-start, glossary — the 5-minute path in |
| `01-framework/` | The canonical concept layer — meta-framework + S/E/A/C/O/W/r component pages + rules + design principles |
| `02-tools/` | The apply-it layer — `seacow-conventions` skill, `seacow-scaffolder` agent, plugin docs, platform notes |
| `03-examples/` | Concrete instantiations — cyberbase as the canonical worked example, plus tag/folder structure samples |
| `04-comparisons/` | Curation hub — SEACOW(r) vs PARA, Zettelkasten, Johnny Decimal, LATCH, ARCO/ACE/STIR |
| `05-deep-dives/` | Long-form reference — knowledge organization theory, decision matrices, choosing a tag structure |
| `06-applications/` | Outward — applying SEACOW(r) to specific platforms (Obsidian, Notion, Claude Code, corporate fileshares, code repos) |
| `INDEXES/` | Multiple navigation paths through the same content (by audience, component, task, depth, comparison) |
| `assets/diagrams/` | SVG/PNG diagrams (capture/work/output flow, etc.) |
| `.claude/` | Claude Code scaffold (skills + agents) for AI assistants working in this repo |

## Related work

- [cybersader/cyberbase](https://github.com/cybersader/cyberbase) — the user's canonical Obsidian Publish vault that originated SEACOW(r)
- [cybersader/crosswalker](https://github.com/cybersader/crosswalker) — Obsidian plugin for importing ontologies/frameworks (NIST, MITRE, CIS, etc.) — uses SEACOW(r) thinking for compliance crosswalks
- [cybersader/obsidian-folder-tag-sync](https://github.com/cybersader/obsidian-folder-tag-sync) — bidirectional folder↔tag mapping; enables polyhierarchy
- [cybersader/agentic-workflow-and-tech-stack](https://github.com/cybersader/agentic-workflow-and-tech-stack) — opinionated Claude Code + Obsidian + Zellij scaffold built on SEACOW(r)
- [cybersader/knowledge-work-foundations](https://github.com/cybersader/knowledge-work-foundations) — portable principles for structured cognitive work

## Status

**v0.1.0** — initial migration baseline. Concepts and worked examples are
imported from the cyberbase vault; per-framework comparison pages are stubbed
and will be filled incrementally. Issues and PRs welcome.

See [ROADMAP.md](ROADMAP.md) for what's queued next.

## Conventions

- **Markdown links, not wikilinks** — so GitHub renders correctly. Obsidian
  Publish still works on the same files (frontmatter is preserved).
- **Frontmatter preserved** — `publish`, `aliases`, `permalink`, `date created`,
  `date modified` are kept on migrated docs so the same files can be republished
  via Obsidian.
- **Numbered top-level folders are stable** — don't renumber once published; the
  numbers force a reading order (00 = entry, 06 = applications).
- **Kebab-case file names** — `obsidian-tag-limitations.md`, not
  `Obsidian Tag Limitations.md`.
- See [AGENTS.md](AGENTS.md) and [CLAUDE.md](CLAUDE.md) for AI-tool conventions.

## License

Documentation is licensed [CC BY 4.0](LICENSE). Reuse with attribution.
