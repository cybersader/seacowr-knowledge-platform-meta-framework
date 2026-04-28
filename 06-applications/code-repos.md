---
title: SEACOW(r) for code repositories
publish: true
---

# SEACOW(r) for code repositories

> [!note] Stub. PRs welcome — see [CONTRIBUTING.md](../CONTRIBUTING.md).

How to apply SEACOW(r) to a Git code repository. This repo (the SEACOW(r)
meta-framework KB) is itself an instance — a docs-only repo organized via
SEACOW(r). For an alternate worked example, see [cybersader/agentic-workflow-and-tech-stack](https://github.com/cybersader/agentic-workflow-and-tech-stack).

## Git-repo primitives

- **Directories** — hierarchical, like any file system.
- **File names** — sortable; naming conventions vary.
- **Frontmatter** in markdown files (publish flags, status, types, etc.).
- **Branches** — encode some Activities (feature branches = Work; main = Output).
- **Commits + tags** — encode time and lifecycle.
- **README files** at any depth — by convention, navigation hubs.
- **Issues + PRs** — async Capture and Relate surfaces (often Work).
- **CODEOWNERS, CONTRIBUTING, LICENSE** — System / Entity configuration files.

## Mapping SEACOW(r) → code repo

| Component | Code-repo primitives |
|---|---|
| **System** | Git itself + the language ecosystem (`package.json`, `Cargo.toml`, `pyproject.toml`); CI/CD; `.github/`, `.gitlab/` |
| **Entity** | CODEOWNERS; PR reviewers; downstream consumers (users / package consumers); AI agents (CLAUDE.md, AGENTS.md) |
| **Capture** | Issues; `docs/ADRs/`; raw notes in `docs/scratch/` (if used) |
| **Work** | `src/`, `tests/`, feature branches, `docs/drafts/` |
| **Output** | `dist/`, `build/`, `docs/api/`, releases, GitHub Pages, README at root |
| **relation** | Imports / requires; references across files; cross-links in markdown docs |

## The numbered-folder pattern (this repo)

This repo uses `00-start-here/`, `01-framework/`, ..., `06-applications/`,
`INDEXES/` to embody SEACOW(r) directly:

| Folder | SEACOW(r) component(s) |
|---|---|
| `00-start-here/` | OUTPUT (entry-point for newcomers) |
| `01-framework/` | SYSTEM (definitional) + OUTPUT (canonical reference) |
| `02-tools/` | SYSTEM (affordances) |
| `03-examples/` | OUTPUT (worked examples for an Entity = practitioner) |
| `04-comparisons/` | relation (mappings to other frameworks) |
| `05-deep-dives/` | WORK (long-form synthesis still being refined) |
| `06-applications/` | OUTPUT for specific Entities (Obsidian users, Notion users, etc.) |
| `INDEXES/` | relation (alternate navigations of the same content) |

## When to add a `knowledge-base/` folder

For long-lived projects that need multi-session persistence, add a
`knowledge-base/` folder with the [temperature gradient](../01-framework/design-principles.md#7-the-temperature-gradient-when-used).
Pair with a `knowledge-curator` skill so AI assistants respect the cooling
discipline.

For docs-only projects (like this one), you can skip the gradient — the whole
repo is already cooled Output.

## See also

- [Claude Code projects application](claude-code-projects.md) — for the `.claude/` directory specifically.
- [The KB-as-the-project's-brain principle](../01-framework/design-principles.md#appendix-knowledge-base-as-the-projects-brain).
- This repo's [AGENTS.md](../AGENTS.md) and [CLAUDE.md](../CLAUDE.md) — concrete examples of agent instructions for a docs repo.
